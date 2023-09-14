<template>
    <div class="signin">
        <div class="container">
            <h1>Welcome, please sign in</h1>
            <div class="costomInput">
                <input type="email">
                <span>Email</span>
            </div>
            <div class="costomInput">
                <input type="password">
                <span>Password</span>
            </div>
            <RouterLink to="/"><button>Sign in</button></RouterLink>
            <a href="#">Forgot Password?</a>
        </div>
    </div>
</template>

<script setup>

</script>

<style scoped>
.signin {
    width: 100%;
    min-height: 100vh;
    background: #F4F4F0;
    display: flex;
    align-items: center;
    justify-content: center;
}

.container {
    width: 409px;
    height: 347px;
    border-radius: 20px;
    background: #FFF;
    box-shadow: 0px 2px 3px 0px rgba(0, 0, 0, 0.25);
    padding: 0 65px;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.container h1 {
    align-self: flex-start;
    color: #3C91F4;
    font-family: Inter;
    font-size: 18px;
    font-style: normal;
    font-weight: 600;
    line-height: 48px;
    /* 266.667% */
    margin-top: 21px;
}

.costomInput {
    width: 100%;
    color: #333;
    position: relative;
    margin-top: 19px;
}

.costomInput input {
    padding-left: 28px;
    width: 100%;
    height: 48px;
    border: 1px solid rgba(51, 51, 51, 0.50);
    outline: none;
    border-radius: 5px;
    font-family: Inter;
    font-size: 14px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;

}

.costomInput span {
    position: absolute;
    left: 28px;
    top: 15px;
    transition: .3s;
    color: #333333c3;
    font-family: Inter;
    font-size: 14px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    background-color: white;
}

input:focus+span {
    top: -10px;
}

.container button {
    align-self: center;
    width: 165.143px;
    height: 48px;
    border-radius: 5px;
    background: #3C91F4;
    color: #FFF;
    text-align: center;
    font-family: Inter;
    font-size: 18px;
    font-style: normal;
    font-weight: 500;
    line-height: 24px;
    /* 133.333% */
    letter-spacing: -0.18px;
    margin-top: 21px;
}

.container a {
    color: #3C91F4;
    font-family: Inter;
    font-size: 12px;
    font-style: normal;
    font-weight: 400;
    line-height: 48px;
    /* 400% */
    align-self: center;
}</style>