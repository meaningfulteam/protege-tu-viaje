# Cómo enviar eventos a GTM:

&nbsp;

## Primeros pasos y eventos del funnel de cotización:

Es importante modificar cada uno de los parámetro de los diferentes objetos de eventos, para agregar el valor correspondiente a la propiedad relacionada. Por ejemplo:

> Tenemos un event construido de la siguiente forma:
>
> ```javascript
> dataLayer.push({
>     event: "event 1",
>     property_1: "",
> });
> ```
>
> Donde el valor de "**property**" se encuentra en la variable "**value**". Para enviar el valor del evento de la forma adecuada, tendremos que enviar algo cómo:
>
> ```javascript
> dataLayer.push({
>     event: "event 1",
>     property_1: value,
> });
> ```
>
> De esa forma tendremos garantizado que nuestro GTM recibirá las propiedades de la forma adecuada.

&nbsp;

### Evento de purchase:

```javascript
dataLayer.push({
    event: "purchase",
    step: "",
    transaction_id: "",
    value: "",
    quoter_name: "",
    order_serial: "",
    quote_code: "",
    order_amount: "",
    currency: "",
});
```

&nbsp;

### Evento de checkout_init:

```javascript
dataLayer.push({
    event: "checkout_init",
    quote_serial: "",
    payment_method: "",
    payment_type: "",
    order_amount: "",
    currency: "",
});
```

&nbsp;

### Evento de completed_passengers_info:

```javascript
dataLayer.push({
    event: "completed_passengers_info",
    local_amount_subtotal: "",
    local_coupon_and_discounts: "",
    local_currency: "",
    order_amount: "",
    order_code: "",
    order_currency: "",
});
```

&nbsp;

### Evento de selected_plan:

```javascript
dataLayer.push({
    event: "selected_plan",
    quote_serial: "",
    first_plan_name: "",
    first_plan_amount: "",
    selected_plan_name: "",
    selected_plan_cost: "",
    selected_plan_id: "",
    selected_plan_code: "",
});
```

&nbsp;

### Evento de completed_passengers_info:

```javascript
dataLayer.push({
    event: "completed_passengers_info",
    local_amount_subtotal: "",
    local_coupon_and_discounts: "",
    local_currency: "",
    order_amount: "",
    order_code: "",
    order_currency: "",
});
```
