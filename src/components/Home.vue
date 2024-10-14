<template>
    <div class="home">
        <h1>Welcome To IE Bank 2024</h1>
        <button @click="goToAccounts">Go to Accounts</button>
    </div>
</template>

<script>
export default {
    name: 'Home',
    methods: {
        goToAccounts() {
            this.$router.push({ name: 'AppAccounts' });
        }
    }
}
</script>

<style scoped>
.home {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
    text-align: center;
}

button {
    padding: 10px 20px;
    font-size: 16px;
    cursor: pointer;
    margin-top: 20px;
}
</style>