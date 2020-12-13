<script>
    export let loading;
    import { onMount } from "svelte";
    setTimeout(() => {
        loading = false;
    }, 600);
</script>

<style>
    .spinner-overlay {
        background-color: #000000fa;
        position: fixed;
        top: 0;
        right: 0;
        width: 100%;
        height: 100%;
        z-index: 9999;
        color: #fff;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .loader,
    .loader:before,
    .loader:after {
        background: #ffffff;
        -webkit-animation: load1 1s infinite ease-in-out;
        animation: load1 1s infinite ease-in-out;
        width: 1em;
        height: 4em;
    }
    .loader {
        color: #ffffff;
        text-indent: -9999em;
        margin: 88px auto;
        position: relative;
        font-size: 11px;
        -webkit-transform: translateZ(0);
        -ms-transform: translateZ(0);
        transform: translateZ(0);
        -webkit-animation-delay: -0.16s;
        animation-delay: -0.16s;
    }
    .loader:before,
    .loader:after {
        position: absolute;
        top: 0;
        content: "";
    }
    .loader:before {
        left: -1.5em;
        -webkit-animation-delay: -0.32s;
        animation-delay: -0.32s;
    }
    .loader:after {
        left: 1.5em;
    }
    @-webkit-keyframes load1 {
        0%,
        80%,
        100% {
            box-shadow: 0 0;
            height: 4em;
        }
        40% {
            box-shadow: 0 -2em;
            height: 5em;
        }
    }
    @keyframes load1 {
        0%,
        80%,
        100% {
            box-shadow: 0 0;
            height: 4em;
        }
        40% {
            box-shadow: 0 -2em;
            height: 5em;
        }
    }
    .spinner-overlay.loaded {
        display: none;
        z-index: -9999;
    }
</style>

<div class="spinner-overlay" class:loaded={loading === false} {loading}>
    <div class="loader">Loading...</div>
</div>
