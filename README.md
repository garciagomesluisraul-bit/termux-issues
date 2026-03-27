# termux-issues
Issues for the Google Play build of Termux.

If you have installed Termux from Google Play, please report issues [here](https://github.com/termux-play-store/termux-issues/issues/new/choose) and nowhere else.
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Corazón 3D</title>
<style>
    body {
        margin: 0;
        background: black;
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        overflow: hidden;
    }

    .heart {
        position: relative;
        width: 150px;
        height: 150px;
        transform: rotate(-45deg);
        animation: latido 1s infinite;
    }

    .heart::before,
    .heart::after {
        content: "";
        position: absolute;
        width: 150px;
        height: 150px;
        background: red;
        border-radius: 50%;
    }

    .heart::before {
        top: -75px;
        left: 0;
    }

    .heart::after {
        left: 75px;
        top: 0;
    }

    @keyframes latido {
        0%, 100% {
            transform: scale(1) rotate(-45deg);
        }
