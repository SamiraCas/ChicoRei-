<script setup>
import InputGroup from '../components/InputGroup.vue';


import { computed, reactive } from 'vue';

import useValidate from '@vuelidate/core'
import { required, email, minLength, alpha } from '@vuelidate/validators'



const cartState = reactive({ quantity: 1 })

const cart = {
    name: 'Camiseta Chicorei',
    image: 'https://chicorei.imgix.net/49528/701f48d3-dfb0-11ed-98d9-771d50299ea6.jpg?auto=compress,format&q=65&w=550&h=824&fit=crop&crop=top',
    price: 79,
    quantity: cartState.quantity
}

const incrementQuantity = () => {
    formData.carrinho.quantidade++
}
const decrementQuantity = () => {
    if (formData.carrinho.quantidade > 1) {

        formData.carrinho.quantidade--
    }
}

const formData = reactive({
    contato: {
        email: '',
        telefone: '',
    },
    endereco: {
        cep: '',
        rua: '',
        numero: '',
        bairro: '',
        cidade: '',
        estado: ''
    },
    cartao: {
        numero: '',
        titular: '',
        dataVencimento: '',
        cvc: ''
    },
    carrinho: {
        quantidade: 1
    }
})

const rules = computed(() => {
    return {
        contato: {
            email: { required, email },
            telefone: { required, minLength: minLength(16) },
        },
        endereco: {
            cep: { required, minLength: minLength(9) },
            rua: { required },
            numero: { required },
            bairro: { required },
            cidade: { required },
            estado: { required, alpha }
        },
        cartao: {
            numero: { required, minLength: minLength(19) },
            titular: { required },
            dataVencimento: { required, minLength: minLength(7) },
            cvc: { required, minLength: minLength(3) }
        }
    }
})


const v$ = useValidate(rules, formData)

const finalOrder = reactive({
    produto: {
        nome: cart.name,
        preco: cart.price,
    },
    informações: formData
})




const submitForm = async () => {
    const result = await v$.value.$validate();
    if (result) {
        alert("Compra realizada")
        console.log(finalOrder)
    } else {
        console.log(v$)
    }
}

</script>

<template>
   
</template>


</style>