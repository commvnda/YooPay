#HTML

<div class='heptapaycontainer'>
<input type="number" id="receivedAmount" class="txtAmount" step="1" autoComplete="off" placeholder="RWF" />
<input type="number" id="sendAmount" class="txtAmount" step=".01" min="1" max="500" autoComplete="off" placeholder="USD" />
<input type="hidden" id="note" value="TrxId" />
<input type="hidden" id="payerEmail" value="" />
<span class="hpayres"></span>
<input id="heptapaybtn" type="button" class='btnPay' value="Pay with HeptaPay" onclick="pay()" />
</div>


#CSS

.heptapaycontainer{width:30vw;background-color:#fff}.paymentForm{display:flex;flex-direction:column}.txtAmount{width:48%;padding:8px 10px;margin:8px 0;display:inline-block;border:1px solid #ccc;border-radius:4px;box-sizing:border-box;font-size:1.3em}.btnPay{background-color:#2499cc;padding:5px 20px;border:none;border-radius:6px;text-align:center;text-decoration:none;display:inline-block;font-size:1.2em;color:#fff;width:auto;display:block;margin-left:auto;margin-right:auto}.btnPay:hover{cursor:pointer}@media only screen and (max-width:600px){.heptapaycontainer{width:80vw}}
View Documentation
WooCommerce Plugin

#JS

<script src="https://ap-gateway.mastercard.com/checkout/version/62/checkout.js" data-error="errorCallback" data-cancel="cancelCallback" data-complete="completeCallback"></script>
<script id="hpayPlugin" data-env="prod" data-country="rw" data-phone="0788822427" data-service="Pay" data-account="" data-callback="https://yourwebsite.com/callback" src="https://heptapay.com/static/js/plugin.paypal.hp.js?v=4.0"></script>
View Documentation
WooCommerce Plugin