---
title: тип ресурса openIdConnectIdentityProvider
description: Представляет поставщики удостоверений OpenIDConnect в клиенте Azure Active Directory B2C.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 990deba52cc4c3ff66f4dd36f0fb795497b97af4
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491202"
---
# <a name="openidconnectidentityprovider-resource-type"></a>тип ресурса openIdConnectIdentityProvider
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет поставщики удостоверений OpenID Connect в клиенте Azure Active Directory B2C.

Настройка поставщика OpenID Connect в клиенте B2C позволяет пользователям зарегистрироваться и войти с помощью настраиваемого поставщика удостоверений в приложении.

Этот тип будет наследоваться [от identityProviderBase](../resources/identityproviderbase.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список](../api/identityproviderbase-list.md)|[коллекция identityProviderBase](../resources/identityproviderbase.md)|Извлечение всех поставщиков удостоверений, настроенных в клиенте, включая поставщиков удостоверений OpenID Connect.|
|[Создание](../api/identityproviderbase-post-identityproviders.md)|openIdConnectIdentityProvider|Создание нового поставщика удостоверений OpenID Connect.|
|[получение](../api/identityproviderbase-get.md); |openIdConnectIdentityProvider|Извлечение свойств поставщика удостоверений OpenID Connect.|
|[Обновление](../api/identityproviderbase-update.md)|Нет|Обновление поставщика удостоверений OpenID Connect.|
|[удаление](../api/identityproviderbase-delete.md);|Нет|Удаление поставщика удостоверений OpenID Connect.|
|[Перечисление доступных типов поставщиков](../api/identityproviderbase-list-availableprovidertypes.md)|Коллекция String|Извлечение всех доступных типов поставщика удостоверений, доступных в клиенте.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|clientId|String|Идентификатор клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений. Обязательное.|
|clientSecret|Строка|Секрет клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений. ClientSecret имеет зависимость от **responseType**. <ul><li>Когда **responseType** — это секрет, необходимый `code` для обмена кодами auth.</li><li>Когда **responseType** `id_token` является секретом, не требуется, так как не существует обмена кодом. Ответ id_token возвращается непосредственно из ответа авторизации.</li></ul> Только для записи. Операция чтения возвращается \* \* \* \* ".|
|id|String|Идентификатор поставщика удостоверений. Обязательно. Наследуется [от identityProviderBase](../resources/identityproviderbase.md). Только для чтения.|
|displayName|String|Отображаемое имя поставщика удостоверений. |
|claimsMapping|[claimsMapping](claimsmapping.md)|После того как поставщик OIDC отправляет маркер ID обратно в Azure AD, Azure AD должна иметь возможность составить карту утверждений от полученного маркера к утверждениям, которые Azure AD распознает и использует. Этот сложный тип захватывает это сопоставление. Обязательное.|
|domainHint|String|Подсказка домена может быть использована для пропуска непосредственно на страницу регистрации указанного поставщика удостоверений вместо того, чтобы пользователь вошел в список доступных поставщиков удостоверений.|
|metadataUrl|String|URL-адрес документа метаданных поставщика удостоверений OpenID Connect. Каждый поставщик удостоверений OpenID Connect описывает документ метаданных, содержащий большую часть сведений, необходимых для выполнения входных данных. К ним относятся такие сведения, как URL-адреса для использования и расположение общедоступных ключей подписи службы. Документ метаданных OpenID Connect всегда расположен в конечной точке, в которую заканчивается `.well-known/openid-configuration` . Укажет URL-адрес метаданных для поставщика удостоверений OpenID Connect, который вы добавляете. Только для чтения. Обязательный.|
|responseMode|String|Режим ответа определяет метод, используемый для отправки данных из пользовательского поставщика удостоверений в Azure AD B2C. Возможные значения: `form_post` , `query` . Обязательное.|
|responseType|String|Тип ответа описывает тип сведений, отосланных во время первоначального вызова authorization_endpoint поставщика пользовательских удостоверений. Возможные значения: `code` `id_token` , `token` .  Обязательное.|
|scope|String|Область определяет сведения и разрешения, которые вы хотите получить от настраиваемого поставщика удостоверений. Запросы OpenID Connect должны содержать значение области openid для получения маркера ID от поставщика удостоверений. Без маркера ID пользователи не могут войти в Azure AD B2C с помощью настраиваемого поставщика удостоверений. Другие области могут быть примеся, разделены пробелом. Дополнительные сведения об ограничениях области см. в разделе [RFC6749 Раздел 3.3](https://tools.ietf.org/html/rfc6749#section-3.3). Обязательное.|

### <a name="responsemode-value"></a>значение responseMode
|Значение|Описание|
:--------|:----------|
|form_post|Этот режим реагирования рекомендуется для обеспечения наилучшей безопасности. Ответ передается методом HTTP POST, код или маркер кодируются в теле с помощью формата application/x-www-form-urlencoded.|
|Запрос|Код или маркер возвращаются в качестве параметра запроса.|

### <a name="responsetype-value"></a>значение responseType
|Значение|Описание|
:--------|:----------|
|code|В течение потока кода авторизации код возвращается обратно в Azure AD B2C. Azure AD B2C продолжает вызывать token_endpoint, чтобы обменять код на маркер.|
|id_token|Маркер ID возвращается обратно в Azure AD B2C от настраиваемого поставщика удостоверений.|
|token|Маркер доступа возвращается обратно в Azure AD B2C от настраиваемого поставщика удостоверений. (На данный момент это значение не поддерживается Azure AD B2C)|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider"
} -->

```json
{
  "id": "String",
  "displayName": "String",
  "clientId": "String",
  "clientSecret": "String",
  "claimsMapping": {
      "@odata.type": "#microsoft.graph.claimsMapping",
      "userId": "String",
      "givenName": "String",
      "surname": "String",
      "email": "String",
      "displayName": "String"
  },
  "domainHint": "String",
  "metadataUrl": "String",
  "responseMode": "String",
  "responseType": "String",
  "scope": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-03-30 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "openidconnectIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
