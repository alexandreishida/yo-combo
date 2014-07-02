yo-combo
========

```html
<div class="yo-combo" style="width:100%"
    data-yo-auto-init="true"
    data-init-display="Iniciando componente...">

    <input name="payment_method" value="<%= params[:payment_method] %>"
        data-url="/payment_method_options"
        data-display="Escolha uma forma de pagamento"
        data-loading-message="Carregando..." />

    <input name="carrier" value="<%= params[:carrier] %>"
        data-url="/carrier_options"
        data-display="Escolha uma convênio"
        data-loading-message="Carregando convênios..."
        data-back-label="Outra" />

    <input name="plan" value="<%= params[:plan] %>"
        data-url="/plan_options?carrier_id={input[1]}"
        data-display="Escolha um plano"
        data-loading-message="Carregando planos..."
        data-back-label="Voltar" />

</div>
```