
<script>
    const params = new URLSearchParams(window.location.search);
    const code = params.get("code");
    if (code) {
        window.location.href = "https://yourbackend.com/oauth/callback?code=" + code;
    } else {
        document.body.innerHTML = "<h1>Invalid Redirect</h1>";
    }
</script>