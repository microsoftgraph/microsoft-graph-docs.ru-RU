---
title: Тип ресурса onPremisesPublishing
description: Представляет объект Application Proxy onPremisesPublishing.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 74ecc94c88990b042e35a7a2701d7a1cd50b1199
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134886"
---
# <a name="onpremisespublishing-resource-type"></a>Тип ресурса onPremisesPublishing

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Локальное приложение, опубликованное через прокси приложения [Azure AD,](https://aka.ms/whyappproxy) представлено объектом приложения и связанным с ним **свойством onPremisesPublishing.** [](application.md) Прокси приложения обеспечивает безопасный удаленный доступ к локальному приложению.

Объект **onPremisesPublishing** представляет набор свойств для настройки прокси приложения для локального [приложения.](application.md) 

После [создания пользовательского](../api/applicationtemplate-instantiate.md) приложения [](../api/application-post-applications.md)или создания приложения можно настроить параметры прокси приложения, обновив свойства [приложения](../api/application-update.md) onPremisesPublishing.

Руководство по настройке прокси приложения см. в руководстве по автоматизации настройки прокси приложения [с помощью API Microsoft Graph.](/graph/application-proxy-configure-api)

## <a name="properties"></a>Свойства

| Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|alternateUrl|Строка| Если диспетчер трафика настраивается перед несколькими приложениями-прокси приложениями, alternateUrl — это пользовательский URL-адрес, который будет ссылаться на диспетчер трафика. |
|applicationServerTimeout|Строка| Время ожидания ответа от приложения перед закрытием подключения соединитетелем. Возможные значения: `default` , `long` . Если задано значение по умолчанию, время простоя приложения во тыловом приложении составляет 85 секунд. Если установлено длительное время, время простоя для тылов увеличивается до 180 секунд. Используйте, если сервер отвечает на запросы более 85 секунд, или если вы не можете получить доступ к приложению, а состояние ошибки — "Время отклика серверной `long` части". Значение по умолчанию: `default`. |
|applicationType|String| Указывает, является ли это приложение настроенным прокси-сервером приложения. Это предварительно заданной системой. Только для чтения. |
|externalAuthenticationType|Строка| Сведения о параметре предварительной проверки подлинности для приложения. При предварительной проверке подлинности пользователи должны пройти проверку подлинности перед доступом к приложению. Passthru не требует проверки подлинности. Возможные значения: `passthru`, `aadPreAuthentication`. |
|externalUrl|Строка| Опубликованный внешний URL-адрес приложения. Например, https://intranet-contoso.msappproxy.net/.  |
|internalUrl|Строка| Внутренний URL-адрес приложения. Например, https://intranet/. |
|isHttpOnlyCookieEnabled|Boolean| Указывает, следует ли устанавливать флаг cookie HTTPOnly в загонах http-ответа. Установите для этого значения, чтобы файлы cookie прокси приложения включали `true` флаг HTTPOnly в загонах HTTP-ответа. При использовании служб удаленных рабочих столов установите для этого значения значение False. Значение по умолчанию: `false`. |
|isOnPremPublishingEnabled|Boolean| Указывает, публикуется ли приложение в настоящее время через прокси-сервер приложения. Это предварительно заданной системой. Только для чтения. |
|isPersistentCookieEnabled|Boolean| Указывает, следует ли устанавливать флаг Persistent cookie в http-ответах. Оохраняем это значение. `false` Используйте этот параметр только для приложений, которые не могут совместно использовать файлы cookie между процессами. Дополнительные сведения о параметрах файлов cookie см. в параметрах cookie для доступа к локальному приложению [в Azure Active Directory.](/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings) Значение по умолчанию: `false`. |
|isSecureCookieEnabled|Boolean| Указывает, следует ли установить флаг "Безопасный файл cookie" в http-ответах. Установите это значение, чтобы передавать файлы cookie по защищенному каналу, например `true` зашифрованному HTTPS-запросу. Значение по умолчанию: `true`.|
|isTranslateHostHeaderEnabled|Boolean| Указывает, должно ли приложение переводить URL-адреса в загонах реответов. Одерывляйте это значение, если приложению не требуется исходный загон `true` хоста в запросе на проверку подлинности. Значение по умолчанию: `true`.|
|isTranslateLinksInBodyEnabled|Boolean| Указывает, должно ли приложение переводить URL-адреса в тексте приложения. Одерывляйте это значение, если у вас нет жестко заданной HTML-ссылок на другие локальное приложение и не `false` используете настраиваемые домены. Дополнительные сведения см. в [переводе ссылок с помощью прокси приложения.](/azure/active-directory/manage-apps/application-proxy-configure-hard-coded-link-translation) Значение по умолчанию: `false`.|
|singleSignOnSettings|[onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md)| Представляет конфигурацию единого входов для локального приложения. |
|verifiedCustomDomainCertificatesMetadata|[verifiedCustomDomainCertificatesMetadata](verifiedcustomdomaincertificatesmetadata.md)| Сведения о сертификате, связанном с приложением при использовании пользовательского домена. `null` при использовании домена по умолчанию. Только для чтения.|
|verifiedCustomDomainKeyCredential|[keyCredential](keycredential.md)| Связанные учетные данные ключа для пользовательского домена. |
|verifiedCustomDomainPasswordCredential|[passwordCredential](passwordcredential.md)| Связанные учетные данные пароля для пользовательского домена. |



## <a name="json-representation"></a>Представление в формате JSON

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


