---
title: Тип ресурса onPremisesPublishing
description: Представляет объект Application Proxy onPremisesPublishing.
ms.localizationpriority: medium
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 453bf7f0ab0f0d13e5c333375d74518251b3f115
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246792"
---
# <a name="onpremisespublishing-resource-type"></a>Тип ресурса onPremisesPublishing

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Локальное приложение, опубликованное с помощью [Azure AD Application Proxy](/azure/active-directory/app-proxy/what-is-application-proxy), представлено объектом приложения и связанным с ним [](application.md) **свойством onPremisesPublishing**. Application Proxy обеспечивает безопасный удаленный доступ к локальным приложениям.

Объект **onPremisesPublishing** представляет набор свойств для настройки Application Proxy для локального [приложения](application.md). 

После [создания пользовательского](../api/applicationtemplate-instantiate.md) приложения или создания приложения [](../api/application-post-applications.md)можно настроить параметры Application Proxy для приложения, обновив [свойства onPremisesPublishing](../api/application-update.md) приложения.

Руководство по настройке Application Proxy см. в статье "Автоматизация настройки Application Proxy [с помощью microsoft API Graph](/graph/application-proxy-configure-api)..

## <a name="properties"></a>Свойства

| Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|alternateUrl|String| Если диспетчер трафика настраивается перед несколькими приложениями Прокси приложения, то alternateUrl — это понятный URL-адрес, указывающий на диспетчер трафика. |
|applicationServerTimeout|String| Продолжительность ожидания ответа от серверного приложения соединителем перед закрытием подключения. Возможные значения:`default``long` Если задано значение по умолчанию, время ожидания внутреннего приложения составляет 85 секунд. Если задано значение long, время ожидания серверной части увеличивается до 180 секунд. Используйте `long` , если сервер отвечает на запросы более 85 секунд или не удается получить доступ к приложению, а состояние ошибки — "Время ожидания серверной части". Значение по умолчанию — `default`. |
|applicationType|String| Указывает, является ли это приложение Application Proxy настроенным приложением. Это предварительно задано системой. Только для чтения. |
|externalAuthenticationType|externalAuthenticationType| Сведения о параметре предварительной проверки подлинности для приложения. Предварительная проверка подлинности требует, чтобы пользователи должны выполнить проверку подлинности перед доступом к приложению. Сквозная проверка подлинности не требуется. Возможные значения: `passthru`, `aadPreAuthentication`. |
|externalUrl|String| Опубликованный внешний URL-адрес приложения. Например, https://intranet-contoso.msappproxy.net/.  |
|Internalurl|String| Внутренний URL-адрес приложения. Например, https://intranet/. |
|isBackendCertificateValidationEnabled|Boolean| Указывает, включена ли проверка SSL-сертификата серверной части для приложения. Для всех новых Application Proxy свойству будет задано значение по `true` умолчанию. Для всех существующих приложений свойству будет задано значение `false`. |
|isHttpOnlyCookieEnabled|Boolean| Указывает, следует ли задать флаг cookie HTTPOnly в заголовках http-ответа. Задайте это значение`true`, чтобы Application Proxy файлы cookie включают флаг HTTPOnly в заголовках http-ответа. При использовании служб удаленных рабочих столов задайте для этого параметра значение False. Значение по умолчанию — `false`. |
|isOnPremPublishingEnabled|Boolean| Указывает, публикуется ли приложение через Application Proxy или нет. Это предварительно задано системой. Только для чтения. |
|isPersistentCookieEnabled|Boolean| Указывает, следует ли задать флаг постоянного файла cookie в заголовках http-ответа. Оставьте для этого значения значение `false`. Используйте этот параметр только для приложений, которые не могут совместно использовать файлы cookie между процессами. Дополнительные сведения о параметрах файлов cookie см. в разделе параметров cookie для доступа к локальным приложениям [в Azure Active Directory](/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings). Значение по умолчанию — `false`. |
|isSecureCookieEnabled|Boolean| Указывает, следует ли задать флаг безопасного файла cookie в заголовках http-ответа. Задайте это значение для `true` передачи файлов cookie по защищенному каналу, такому как зашифрованный HTTPS-запрос. Значение по умолчанию — `true`.|
|isStateSessionEnabled|Boolean| Указывает, включена ли проверка параметра состояния, если клиент использует поток предоставления кода авторизации OAuth 2.0. Этот параметр позволяет администраторам указать, следует ли включить защиту CSRF для своих приложений. |
|isTranslateHostHeaderEnabled|Boolean| Указывает, должно ли приложение переводить URL-адреса в заголовках ответа. Сохраните это значение, `true` если приложению не требуется исходный заголовок узла в запросе на проверку подлинности. Значение по умолчанию — `true`.|
|isTranslateLinksInBodyEnabled|Boolean| Указывает, должно ли приложение переводить URL-адреса в тексте приложения. Сохраните это значение, `false` если у вас нет жестко закодированных HTML-ссылок на другие локальные приложения и не используете личных доменов. Дополнительные сведения см. в разделе ["Преобразование ссылок с помощью Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-hard-coded-link-translation)". Значение по умолчанию — `false`.|
|singleSignOnSettings|[onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md)| Представляет конфигурацию единого входа для локального приложения. |
|verifiedCustomDomainCertificatesMetadata|[verifiedCustomDomainCertificatesMetadata](verifiedcustomdomaincertificatesmetadata.md)| Сведения о сертификате, связанном с приложением при использовании личного домена. `null` при использовании домена по умолчанию. Только для чтения.|
|verifiedCustomDomainKeyCredential|[keyCredential](keycredential.md)| Связанные учетные данные ключа для используемого личного домена. |
|verifiedCustomDomainPasswordCredential|[passwordCredential](passwordcredential.md)| Связанные учетные данные пароля для используемого личного домена. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishing"
}-->

```json
{
  "alternateUrl": "String",
  "applicationServerTimeout": "String",
  "applicationType": "String",
  "externalAuthenticationType": "String",
  "externalUrl": "String",
  "internalUrl": "String",
  "isBackendCertificationValidationEnabled": true,
  "isHttpOnlyCookieEnabled": true,
  "isOnPremPublishingEnabled": true,
  "isPersistentCookieEnabled": true,
  "isSecureCookieEnabled": true,
  "isStateSessionEnabled": true,
  "isTranslateHostHeaderEnabled": true,
  "isTranslateLinksInBodyEnabled": true,
  "singleSignOnSettings": {"@odata.type": "microsoft.graph.onPremisesPublishingSingleSignOn"},
  "verifiedCustomDomainCertificatesMetadata": {"@odata.type": "microsoft.graph.verifiedCustomDomainCertificatesMetadata"},
  "verifiedCustomDomainKeyCredential": {"@odata.type": "microsoft.graph.keyCredential"},
  "verifiedCustomDomainPasswordCredential": {"@odata.type": "microsoft.graph.passwordCredential"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2019-02-04 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
