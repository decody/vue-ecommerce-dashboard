
<template>
    <div class="logobox">
        <div class="logo">
            <svg width="10" height="12" viewBox="0 0 10 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M6 0L0 7H4V12L10 5H6V0Z" fill="white"/>
            </svg>
        </div>
    </div>
</template>

<script>

export default {
    name: 'Logobox',
    components: {
		
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
</style>
