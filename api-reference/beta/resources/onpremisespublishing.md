---
title: Тип ресурса Онпремисеспублишинг
description: Представляет объект Онпремисеспублишинг прокси приложения.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8969ac4803d40e76d227355aeb00cb400389ff6c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998672"
---
# <a name="onpremisespublishing-resource-type"></a>Тип ресурса Онпремисеспублишинг

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Локальное приложение, опубликованное с помощью [прокси приложения Azure AD](https://aka.ms/whyappproxy) , представлено объектом [Application](application.md) и связанным свойством **онпремисеспублишинг** . Прокси приложения обеспечивает безопасный удаленный доступ к локальным приложениям.

Объект **онпремисеспублишинг** представляет набор свойств для настройки прокси приложения для локального [приложения](application.md). 

После создания [экземпляра настраиваемого приложения](../api/applicationtemplate-instantiate.md) или [создания приложения](../api/application-post-applications.md)параметры прокси-сервера для приложения можно настроить, обновив свойства онпремисеспублишинг [приложения](../api/application-update.md) .

Руководство по настройке прокси приложения приведено в разделе [Автоматизация настройки прокси приложения с помощью API Microsoft Graph](https://docs.microsoft.com/graph/application-proxy-configure-api).

## <a name="properties"></a>Свойства

| Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|alternateUrl|String| При настройке диспетчера трафика перед несколькими прокси-приложениями приложений alternateUrl — это понятный для пользователя URL-адрес, который указывает на диспетчер трафика. |
|аппликатионсервертимеаут|String| Срок, в течение которого соединитель будет ожидать ответа от внутреннего приложения перед закрытием подключения. Возможные значения: `default` , `long` . Если задано значение по умолчанию, время ожидания для внутреннего приложения составляет 85 секунд. Если задано значение Long, время ожидания для внутреннего сервера увеличивается до 180 секунд. Используйте `long` , если сервер занимает более 85 секунд, чтобы отвечать на запросы, или если у вас нет доступа к приложению, а состояние ошибки — "время ожидания внутренней базы данных". Значение по умолчанию: `default`. |
|applicationType|String| Указывает, является ли это приложение настроенным прокси-сервером приложения. Это предварительно задается системой. Только для чтения. |
|екстерналаусентикатионтипе|String| Подробное описание параметров предварительной проверки подлинности для приложения. Предварительная проверка подлинности обеспечивает проверку подлинности пользователей, прежде чем получить доступ к приложению. PassThru не требует проверки подлинности. Возможные значения: `passthru`, `aadPreAuthentication`. |
|externalUrl|String| Опубликованный внешний URL-адрес приложения. Например, https://intranet-contoso.msappproxy.net/.  |
|internalUrl|String| Внутренний URL-адрес приложения. Например, https://intranet/. |
|ишттпонликукиинаблед|Boolean| Указывает, должен ли устанавливаться флаг файла HTTPOnly в заголовках HTTP-ответа. Присвойте этому параметру значение, чтобы `true` файлы cookie прокси-сервера приложений включали флаг HttpOnly в заголовках HTTP-ответа. Если используется служба удаленных рабочих столов, установите для этого параметра значение false. Значение по умолчанию: `false`. |
|исонпремпублишинженаблед|Boolean| Указывает, публикуется ли приложение через прокси приложения или нет. Это предварительно задается системой. Только для чтения. |
|исперсистенткукиинаблед|Boolean| Указывает, следует ли задать флаг постоянного cookie в заголовках HTTP-ответа. Оставьте значение этого параметра равным `false` . Этот параметр следует использовать только для приложений, которые не могут совместно использовать файлы cookie между процессами. Дополнительные сведения о параметрах файлов cookie можно найти [в разделе Параметры файлов cookie для доступа к локальным приложениям в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings). Значение по умолчанию: `false`. |
|иссекурекукиинаблед|Boolean| Указывает, следует ли устанавливать флаг Secure cookie в заголовках ответа HTTP. Присвойте этому параметру значение `true` для передачи файлов cookie по безопасному каналу, такому как зашифрованный HTTPS – запрос. Значение по умолчанию: `true`.|
|истранслатехоссеадеренаблед|Boolean| Указывает, должно ли приложение транслировать URL-адреса в заголовках ответа. Оставьте это значение, `true` Если ваше приложение не требует в запросе проверки подлинности исходного заголовка узла. Значение по умолчанию: `true`.|
|истранслателинксинбоденаблед|Boolean| Указывает, должно ли приложение транслировать URL-адреса в тексте приложения. Оставьте это значение, `false` Если вы не зажестко HTML-ссылки на другие локальные приложения и не используете пользовательские домены. Дополнительные сведения можно найти [в разделе Преобразование ссылок с помощью прокси-сервера приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-hard-coded-link-translation). Значение по умолчанию: `false`.|
|синглесигнонсеттингс|[онпремисеспублишингсинглесигнон](onpremisespublishingsinglesignon.md)| Представляет конфигурацию единого входа для локального приложения. |
|верифиедкустомдомаинцертификатесметадата|[верифиедкустомдомаинцертификатесметадата](verifiedcustomdomaincertificatesmetadata.md)| Сведения о сертификате, связанном с приложением при использовании настраиваемого домена. `null` При использовании домена по умолчанию. Только для чтения.|
|верифиедкустомдомаинкэйкредентиал|[keyCredential](keycredential.md)| Соответствующие учетные данные ключа для пользовательского домена. |
|верифиедкустомдомаинпассвордкредентиал|[passwordCredential](passwordcredential.md)| Соответствующие учетные данные пароля для пользовательского домена. |



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


