<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Merchant & Newsletter</title>
    
    <!-- Fonts & Styles -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css">
    <style type="text/css">@import url("https://assets.mlcdn.com/fonts.css?version=1755584");</style>
    
    <style>
        /* Loader & Newsletter Styles */
        .ml-form-embedSubmitLoad { display: inline-block; width: 20px; height: 20px; }
        .g-recaptcha { transform: scale(1); -webkit-transform: scale(1); transform-origin: 0 0; -webkit-transform-origin: 0 0; }
        .sr-only { position: absolute; width: 1px; height: 1px; padding: 0; margin: -1px; overflow: hidden; clip: rect(0,0,0,0); border: 0; }
        .ml-form-embedSubmitLoad:after {
            content: " ";
            display: block;
            width: 11px;
            height: 11px;
            margin: 1px;
            border-radius: 50%;
            border: 4px solid #fff;
            border-color: #ffffff #ffffff #ffffff transparent;
            animation: ml-form-embedSubmitLoad 1.2s linear infinite;
        }
        @keyframes ml-form-embedSubmitLoad {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }

        /* You can paste all the remaining CSS from your snippet here */
        /* For brevity, I'm keeping it compact */
    </style>

    <!-- Basic AI Merchant Landing Page Styles -->
    <style>
        body { font-family: Arial, sans-serif; margin: 0; padding: 0; background: #f5f5f5; }
        header { background: #000; color: #fff; padding: 20px; text-align: center; }
        main { padding: 40px 20px; max-width: 1200px; margin: auto; }
        .section { background: #fff; padding: 20px; margin-bottom: 20px; border-radius: 8px; box-shadow: 0 2px 10px rgba(0,0,0,0.1); }
        button { padding: 10px 20px; border: none; border-radius: 5px; background: #000; color: #fff; cursor: pointer; }
        button:hover { background: #333; }
        input, textarea { width: 100%; padding: 10px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px; }
    </style>
</head>
<body>

<header>
    <h1>AI Merchant</h1>
    <p>Automated E-commerce with AI</p>
</header>

<main>
    <section class="section">
        <h2>Product Scout</h2>
        <p>Discover profitable products with AI recommendations.</p>
        <button onclick="alert('Product suggestion coming soon!')">Suggest Product</button>
    </section>

    <section class="section">
        <h2>Inventory Management</h2>
        <p>Automatically manage stock levels with AI tracking.</p>
    </section>

    <section class="section">
        <h2>Pricing Automation</h2>
        <p>Optimize pricing using AI-driven market analysis.</p>
    </section>

    <!-- Newsletter Embed -->
    <div id="mlb2-30058241" class="ml-form-embedContainer ml-subscribe-form ml-subscribe-form-30058241">
        <div class="ml-form-align-center ">
            <div class="ml-form-embedWrapper embedForm">
                <div class="ml-form-embedBody ml-form-embedBodyDefault row-form">
                    <div class="ml-form-embedContent">
                        <h4>Newsletter</h4>
                        <p>Signup for news and special offers!</p>
                    </div>
                    <form class="ml-block-form" action="https://assets.mailerlite.com/jsonp/1660733/forms/163743863189538168/subscribe" method="post" target="_blank">
                        <div class="ml-form-formContent">
                            <div class="ml-form-fieldRow ml-last-item">
                                <div class="ml-field-group ml-field-email ml-validate-email ml-validate-required">
                                    <input aria-label="email" aria-required="true" type="email" class="form-control" name="fields[email]" placeholder="Email" autocomplete="email">
                                </div>
                            </div>
                        </div>
                        <input type="hidden" name="ml-submit" value="1">
                        <div class="ml-form-embedSubmit">
                            <button type="submit" class="primary">Subscribe</button>
                            <button disabled="disabled" style="display: none;" type="button" class="loading">
                                <div class="ml-form-embedSubmitLoad"></div>
                                <span class="sr-only">Loading...</span>
                            </button>
                        </div>
                        <input type="hidden" name="anticsrf" value="true">
                    </form>
                </div>
                <div class="ml-form-successBody row-success" style="display: none">
                    <div class="ml-form-successContent">
                        <h4>Thank you!</h4>
                        <p>You have successfully joined our subscriber list.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</main>

<!-- Scripts -->
<script>
    function ml_webform_success_30058241() {
        var $ = ml_jQuery || jQuery;
        $('.ml-subscribe-form-30058241 .row-success').show();
        $('.ml-subscribe-form-30058241 .row-form').hide();
    }
</script>
<script src="https://groot.mailerlite.com/js/w/webforms.min.js?v176e10baa5e7ed80d35ae235be3d5024" type="text/javascript"></script>
<script>
    fetch("https://assets.mailerlite.com/jsonp/1660733/forms/163743863189538168/takel")
</script>

</body>
</html>
