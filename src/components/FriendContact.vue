<template>
    <li>
        <h2> {{friends.name}} </h2>
        <button @click="toggleDetails"> show Details </button>

        <ul v-if="detailAreVisible">
            <li> <strong> Phone: </strong> {{ friends.phone}} </li>
            <li> <strong> Email: </strong> {{ friends.email}} </li>
        </ul>    
    </li>    
</template>


<script>
export default {
    data() {
        return{
          detailAreVisible: false,
          friends:  {
          id: 'manuel',
          name: 'ivan',
          phone: '123456789',
          email: 'manuel@gmail.com'
        },
        }
    },
    methods: {
        toggleDetails() {
            this.detailAreVisible = !this.detailAreVisible;
        }
    }
}
</script>