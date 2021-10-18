---
title: Ver la suscripción y el uso de tu cuenta de empresa
intro: 'Puedes ver {% ifversion fpt %}la suscripción, {% endif %}el uso de licencia{% ifversion fpt %}, facturas, historial de pagos y otra información de facturación{% endif %} para {% ifversion fpt %}tu cuenta empresarial{% elsif ghes %}{% data variables.product.product_location_enterprise %}{% endif %}.'
product: '{% data reusables.gated-features.enterprise-accounts %}'
permissions: 'Enterprise owners {% ifversion fpt %}and billing managers {% endif %}can access and manage all billing settings for enterprise accounts.'
redirect_from:
  - /github/setting-up-and-managing-your-enterprise/managing-your-enterprise-account/viewing-the-subscription-and-usage-for-your-enterprise-account
  - /github/setting-up-and-managing-your-enterprise-account/viewing-the-subscription-and-usage-for-your-enterprise-account
  - /articles/viewing-the-subscription-and-usage-for-your-enterprise-account
  - /github/setting-up-and-managing-your-enterprise/viewing-the-subscription-and-usage-for-your-enterprise-account
versions:
  fpt: '*'
  ghes: '*'
topics:
  - Enterprise
shortTitle: Ver la suscripción & uso
---

## Acerca de la facturación para las cuentas de empresa

Puedes ver un resumen de {% ifversion fpt %}tu suscripción y uso de tu {% elsif ghes %}licencia pagada{% endif %} para {% ifversion fpt %}tu{% elsif ghes %}la{% endif %} cuenta empresarial en {% ifversion fpt %}{% data variables.product.prodname_dotcom_the_website %}{% elsif ghes %}{% data variables.product.product_location %}{% endif %}.

Para los clientes de {% data variables.product.prodname_enterprise %} a quienes se factura{% ifversion ghes %} quienes usan tanto {% data variables.product.prodname_ghe_cloud %} como {% data variables.product.prodname_ghe_server %}{% endif %}, cada factura incluye detalles sobre los servicios que se cobran de todos los productos. Por ejemplo, adicionalmente a tu uso de {% ifversion fpt %}{% data variables.product.prodname_ghe_cloud %}{% elsif ghes %}{% data variables.product.product_name %}{% endif %}, puedes tener un uso de {% data variables.product.prodname_GH_advanced_security %}{% ifversion fpt %},{% elsif ghes %}. También puedes tener uso en {% data variables.product.prodname_dotcom_the_website %}, como {% endif %}licencias de pago en organizaciones fuera de tu cuenta empresarial, paquetes de datos para {% data variables.large_files.product_name_long %} o suscripciones en apps dentro de {% data variables.product.prodname_marketplace %}. Para obtener más información sobre las facturas, consulta la sección "{% ifversion fpt %}[Administrar las facturas de tu empresa](/billing/managing-billing-for-your-github-account/managing-invoices-for-your-enterprise)".{% elsif ghes %}<a href="/billing/managing-billing-for-your-github-account/viewing-the-subscription-and-usage-for-your-enterprise-account" class="dotcom-only">Visualizar la suscripción y uso de tu cuenta empresarial</a>" en la documentación de {% data variables.product.prodname_dotcom_the_website %}.{% endif %}

{% ifversion fpt %}

Adicionalmente a los propietarios de empresas, los gerentes de facturación pueden ver la suscripción y el uso de tu cuenta empresarial. Para obtener más información, consulta las secciones "[Roles en una empresa](/github/setting-up-and-managing-your-enterprise/managing-users-in-your-enterprise/roles-in-an-enterprise#billing-manager)" y "[Invitar a las personas para que administren tu empresa](/github/setting-up-and-managing-your-enterprise/inviting-people-to-manage-your-enterprise)".

{% data reusables.enterprise-accounts.billing-microsoft-ea-overview %} Para obtener más información, consulta la sección "[Conectar una suscripción de Azure a tu empresa](/github/setting-up-and-managing-your-enterprise/connecting-an-azure-subscription-to-your-enterprise)".

{% endif %}

{% ifversion ghes %}

Si quieres ver un resumen de tu uso y suscripción de {% data variables.product.prodname_enterprise %} y de cualquier servicio relacionado en {% data variables.product.prodname_dotcom_the_website %}, consulta la sección de "[Ver el uso y suscripción de tu cuenta empresarial](/free-pro-team@latest/billing/managing-billing-for-your-github-account/viewing-the-subscription-and-usage-for-your-enterprise-account)" en la documentación de {% data variables.product.prodname_dotcom_the_website %}.

{% endif %}

## Ver la suscripción y el uso de tu cuenta de empresa

{% data reusables.enterprise-accounts.access-enterprise %}
{% data reusables.enterprise-accounts.settings-tab %}
{% data reusables.enterprise-accounts.license-tab %}
1. En "Licencias de Usuario", ve tus licencias totales, la cantidad de licencias consumidas y la fecha de vencimiento de tu suscripción.
  {% ifversion fpt %}![License and subscription information in enterprise billing settings](/assets/images/help/business-accounts/billing-license-info.png){% else %}
  ![Información de licencia y suscripción en las configuraciones de facturación de la empresa](/assets/images/enterprise/enterprise-server/enterprise-server-billing-license-info.png){% endif %}
1. Opcionalmente, para ver los detalles del uso de licencia o para descargar un archivo {% ifversion fpt %}CSV{% elsif ghes %}JSON{% endif %} con los detalles de la misma{% ifversion fpt %}, a la derecha de "Licencias de Usuario"{% endif %}, haz clic en **Ver {% ifversion fpt %}detalles{% elsif ghes %}usuarios{% endif %}** o {% ifversion fpt %}{% octicon "download" aria-label="The download icon" %}{% elsif ghes %}**Eportar uso de licencia**{% endif %}.{% ifversion fpt %}!["View details" button and button with download icon to the right of "User Licenses"](/assets/images/help/business-accounts/billing-license-info-click-view-details-or-download.png){% endif %}{% ifversion fpt %}
1. Opcionalmente, para ver los detalles de uso de otras características, en la barra lateral izquierda, da clic en **Facturación**. ![Pestaña de facturación en la barra lateral de parámetros de la cuenta de empresa](/assets/images/help/business-accounts/settings-billing-tab.png)
{% endif %}