---
title: onPremisesPublishing resource type
description: Представляет прокси-сервер приложения на объектеPremisesPublishing.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 5b884d6f1aadb43d682cba1434ed4d31e0ae1e70
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956927"
---
# <a name="onpremisespublishing-resource-type"></a>onPremisesPublishing resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Локальное приложение, опубликованное через [Прокси-сервер приложения Azure AD,](https://aka.ms/whyappproxy) представлено объектом приложения и связанным с ним **свойствомPremisesPublishing.** [](application.md) Application Proxy предоставляет безопасный удаленный доступ к локальному приложению.

Объект **onPremisesPublishing** представляет набор свойств для настройки прокси-сервера приложения для локального [приложения.](application.md) 

После [мгновенного](../api/applicationtemplate-instantiate.md) обновления настраиваемой программы или создания приложения параметры прокси-сервера приложения можно настроить, обновив свойства приложения onPremisesPublishing. [](../api/application-post-applications.md) [](../api/application-update.md)

Руководство по настройке прокси-сервера приложений см. в руководстве [Automate the configuration of Application Proxy using the Microsoft Graph API.](/graph/application-proxy-configure-api)

## <a name="properties"></a>Свойства

| Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|alternateUrl|Строка| При настройке диспетчера трафика перед несколькими приложениями прокси-приложения app альтернативный URL-адрес, который будет указать диспетчеру трафика. |
|applicationServerTimeout|Строка| Время, в течение времени, которое соединитатель будет ждать ответа от приложения-спинки перед закрытием подключения. Возможные значения `default` : `long` . Если установлено значение по умолчанию, время, заданное по умолчанию, имеет длину 85 секунд. Если задана длинная настройка, время отодвигаемого времени увеличивается до 180 секунд. Используйте, если серверу требуется более 85 секунд для ответа на запросы или если вы не можете получить доступ к приложению, а состояние ошибки — "Время отыскки". `long` Значение по умолчанию: `default`. |
|applicationType|String| Указывает, является ли это приложение приложением прокси-сервера приложения. Это заранее заданной системой. Только для чтения. |
|externalAuthenticationType|externalAuthenticationType| Сведения о параметре предварительной проверки подлинности для приложения. Предварительная проверка подлинности обеспечивает, чтобы пользователи должны пройти проверку подлинности перед доступом к приложению. Passthru не требует проверки подлинности. Возможные значения: `passthru`, `aadPreAuthentication`. |
|externalUrl|Строка| Опубликованный внешний URL-адрес приложения. Например, https://intranet-contoso.msappproxy.net/.  |
|internalUrl|Строка| Внутренний URL-адрес приложения. Например, https://intranet/. |
|isHttpOnlyCookieEnabled|Boolean| Указывает, следует ли установить флаг cookie HTTPOnly в загонах ответов HTTP. Установите это значение, `true` чтобы cookie-файлы прокси-серверов приложений включали флаг HTTPOnly в заглавных главах ответов HTTP. Если используется служба удаленного рабочего стола, установите это значение false. Значение по умолчанию: `false`. |
|isOnPremPublishingEnabled|Boolean| Указывает, публикуется ли приложение в настоящее время с помощью прокси-сервера приложения или нет. Это заранее заданной системой. Только для чтения. |
|isPersistentCookieEnabled|Boolean| Указывает, следует ли установить флаг сохраняемой файлы cookie в загонах http-ответа. Сохраняй это `false` значение. Используйте этот параметр только для приложений, которые не могут обмениваться файлами cookie между процессами. Дополнительные сведения о параметрах cookie см. в приложении Cookie для доступа к локальному приложению [в Azure Active Directory.](/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings) Значение по умолчанию: `false`. |
|isSecureCookieEnabled|Boolean| Указывает, следует ли установить флаг "Безопасное cookie" в загонах http-ответа. Установите это значение для `true` передачи файлов cookie по защищенному каналу, например зашифрованному запросу HTTPS. Значение по умолчанию: `true`.|
|isTranslateHostHeaderEnabled|Boolean| Указывает, следует ли приложению переводить URL-адреса в загонах reponse. Храните это значение так, как если в запросе на проверку подлинности вашему приложению не требуется исходный загон `true` хост. Значение по умолчанию: `true`.|
|isTranslateLinksInBodyEnabled|Boolean| Указывает, следует ли приложению переводить URL-адреса в теле приложения. Храните это значение как если у вас нет жестких HTML-ссылок на другие локальное приложение и не `false` используйте настраиваемые домены. Дополнительные сведения см. в [приложении Link translation with Application Proxy.](/azure/active-directory/manage-apps/application-proxy-configure-hard-coded-link-translation) Значение по умолчанию: `false`.|
|singleSignOnSettings|[onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md)| Представляет единую конфигурацию входов для локального приложения. |
|verifiedCustomDomainCertificatesMetadata|[verifiedCustomDomainCertificatesMetadata](verifiedcustomdomaincertificatesmetadata.md)| Сведения о сертификате, связанном с приложением при использовании настраиваемого домена. `null` при использовании домена по умолчанию. Только для чтения.|
|verifiedCustomDomainKeyCredential|[keyCredential](keycredential.md)| Связанные учетные данные ключей для используемой настраиваемой области. |
|verifiedCustomDomainPasswordCredential|[passwordCredential](passwordcredential.md)| Связанные учетные данные паролей для используемой настраиваемой области. |



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
  "isHttpOnlyCookieEnabled": true,
  "isOnPremPublishingEnabled": true,
  "isPersistentCookieEnabled": true,
  "isSecureCookieEnabled": true,
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


