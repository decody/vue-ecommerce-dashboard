
<template>
    <div class="login-container">
        <div class="login-wrap">
            <div class="login-header">
                <Logobox />
                <h1 class="roboto font-700">Shopify Admin</h1>
            </div>
            <div class="login-form">
                <dl class="input-form">
                    <dt>
                        <label for="" class="roboro font-700">Email</label>
                    </dt>
                    <dd>
                        <input type="text" />
                    </dd>
                </dl>
                <dl class="input-form">
                    <dt>
                        <label for="" class="roboro font-700">Password</label>
                    </dt>
                    <dd>
                        <input type="text" />
                    </dd>
                </dl>
            </div>
            <div class="login-bottom">
                <button type="submit" class="btn-primary roboto font-400">Sign In</button>
            </div>
        </div>
    </div>
</template>

<script>
import Logobox from '@/components/common/Logobox.vue';

export default {
    components: {
		Logobox
	},
	data() {
		return {
			
		}
	},
	created() {
	},
	mounted() {
	},
	methods: {
	},
}
</script>

<style lang="scss" scoped>
.login-container {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100vw;
    height: 100vh;
}
.login-wrap {
    width: 325px;
    margin: 0 auto;
    min-height: 500px;
}
.login-header {
    display: flex;
    align-items: center;
    justify-content: left;
    margin-bottom: 50px;
    padding: 15px 0;
    border-bottom: solid 1px #000;

    h1 {
        padding-left: 15px;
        font-size: 20px;
    }
}
.login-bottom {
    margin-top: 40px;
}
.logobox {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 40px;
    height: 40px;
    background-color: #017EFA;
    border-radius: 5px;

    .logo {
        display: flex;
        align-items: center;
        justify-content: center;
        width: 24px;
        height: 24px;
        border-radius: 50%;
        border: solid 3px #fff;
    }
}
.input-form {
    dt {
        padding-bottom: 10px;
    }

    label {
        color: #111;
        font-size: 16px;
    }
    input {
        width: 100%;
        height: 58px;
        padding: 16px;
        color: #707070;
        border: solid 1px #CFCFCF;
        border-radius: 5px;
    }

    & + .input-form {
        padding-top: 20px;
    }
}
.btn-primary {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 58px;
    font-size: 16px;
    color: #fff;
    border-radius: 5px;
    background-color: #017EFA;
}

</style>
