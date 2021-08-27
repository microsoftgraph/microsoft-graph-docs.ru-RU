---
title: тип ресурса openIdConnectIdentityProvider
description: Представляет поставщики удостоверений OpenIDConnect в клиенте Azure Active Directory B2C.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: bb905d7c8cfa4842e1feb34acaa5b5f7210b50a9
ms.sourcegitcommit: f99dc2b6c8b4cb6f9f74cd780dccc47a2bccfaa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2021
ms.locfileid: "58667894"
---
# <a name="openidconnectidentityprovider-resource-type"></a>тип ресурса openIdConnectIdentityProvider
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет поставщики удостоверений openID Подключение в клиенте Azure Active Directory (Azure AD) B2C.

Настройка поставщика openID Подключение в клиенте Azure AD B2C позволяет пользователям зарегистрироваться и войти в любое приложение с помощью настраиваемого поставщика удостоверений.

Наследуется от [identityProviderBase](../resources/identityproviderbase.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список](../api/identitycontainer-list-identityproviders.md)|[коллекция identityProviderBase](../resources/identityproviderbase.md)|Извлечение всех поставщиков удостоверений, настроенных в клиенте, включая [тип объекта openIdConnectIdidentityProvider.](../resources/openidconnectidentityprovider.md) Нет способа получить только поставщиков удостоверений OpenID Подключение в клиенте.|
|[Create](../api/identitycontainer-post-identityproviders.md)|[openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md)|Создание нового [объекта openIdConnectIdentityProvider.](../resources/openidconnectidentityprovider.md)|
|[получение](../api/identityproviderbase-get.md); |openIdConnectIdentityProvider|Извлечение свойств [объекта openIdConnectIdentityProvider.](../resources/openidconnectidentityprovider.md)|
|[Обновление](../api/identityproviderbase-update.md)|Нет|Обновление [объекта openIdConnectIdentityProvider.](../resources/openidconnectidentityprovider.md)|
|[удаление](../api/identityproviderbase-delete.md);|Нет|Удаление [объекта openIdConnectIdentityProvider.](../resources/openidconnectidentityprovider.md)|
|[Перечисление доступных типов поставщиков](../api/identityproviderbase-availableprovidertypes.md)|Коллекция String|Получение всех типов поставщиков удостоверений, доступных в клиенте.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|clientId|String|Идентификатор клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений. Обязательно.|
|clientSecret|Строка|Секрет клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений. ClientSecret имеет зависимость от **responseType**. <ul><li>Когда **responseType** — это секрет, необходимый `code` для обмена кодами auth.</li><li>Когда **responseType** `id_token` является секретом, не требуется, так как не существует обмена кодом. Ответ id_token возвращается непосредственно из ответа авторизации.</li></ul> Только для записи. Операция чтения возвращает `****`.|
|id|String|Идентификатор поставщика удостоверений. Обязательно. Унаследовано от [identityProviderBase](../resources/identityproviderbase.md). Только для чтения.|
|displayName|String|Отображаемое имя поставщика удостоверений. |
|claimsMapping|[claimsMapping](claimsmapping.md)|После того как поставщик OIDC отправляет маркер ID обратно в Azure AD, Azure AD должна иметь возможность составить карту утверждений от полученного маркера к утверждениям, которые Azure AD распознает и использует. Этот сложный тип захватывает это сопоставление. Обязательный элемент.|
|domainHint|String|Подсказка домена может быть использована для пропуска непосредственно на страницу регистрации указанного поставщика удостоверений вместо того, чтобы пользователь вошел в список доступных поставщиков удостоверений.|
|metadataUrl|String|URL-адрес документа метаданных поставщика удостоверений OpenID Подключение. Каждый поставщик Подключение OpenID описывает документ метаданных, содержащий большую часть сведений, необходимых для выполнения входных данных. К ним относятся такие сведения, как URL-адреса для использования и расположение общедоступных ключей подписи службы. Документ openID Подключение метаданных всегда находится в конечной точке, которая заканчивается `.well-known/openid-configuration` . Указайте URL-адрес метаданных для поставщика удостоверений OpenID Подключение, который вы добавляете. Только для чтения. Обязательный.|
|responseMode|[openIdConnectResponseMode](#openidconnectresponsemode-values)|Режим ответа определяет метод, используемый для отправки данных из пользовательского поставщика удостоверений в Azure AD B2C. Возможные значения: `form_post` , `query` . Обязательный элемент.|
|responseType|[openIdConnectResponseTypes](#openidconnectresponsetypes-values)|Тип ответа описывает тип сведений, отосланных во время первоначального вызова authorization_endpoint поставщика пользовательских удостоверений. Возможные значения: `code` `id_token` , `token` .  Обязательный элемент.|
|scope|String|Область определяет сведения и разрешения, которые вы хотите получить от настраиваемого поставщика удостоверений. Запросы Подключение OpenID должны содержать значение области openid для получения маркера ID от поставщика удостоверений. Без маркера ID пользователи не могут войти в Azure AD B2C с помощью настраиваемого поставщика удостоверений. Другие области могут быть примеся, разделены пробелом. Дополнительные сведения об ограничениях области см. в разделе [RFC6749 Раздел 3.3](https://tools.ietf.org/html/rfc6749#section-3.3). Обязательный элемент.|

### <a name="openidconnectresponsemode-values"></a>значения openIdConnectResponseMode
|Member|Описание|
:--------|:----------|
|form_post|Этот режим реагирования рекомендуется для обеспечения наилучшей безопасности. Ответ передается методом HTTP POST, код или маркер кодируются в теле с помощью формата application/x-www-form-urlencoded.|
|Запрос|Код или маркер возвращаются в качестве параметра запроса.|
|unknownFutureValue|Значение sentinel, чтобы указать будущие значения.|

### <a name="openidconnectresponsetypes-values"></a>значения openIdConnectResponseTypes
|Member|Описание|
:--------|:----------|
|code|В течение потока кода авторизации код возвращается обратно в Azure AD B2C. Azure AD B2C продолжает вызывать token_endpoint, чтобы обменять код на маркер.|
|id_token|Маркер ID возвращается обратно в Azure AD B2C от настраиваемого поставщика удостоверений.|
|token|Маркер доступа возвращается обратно в Azure AD B2C от настраиваемого поставщика удостоверений. (На данный момент это значение не поддерживается Azure AD B2C)|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider",
  "baseType": "microsoft.graph.identityProviderBase",
} -->

```json
{
  "@odata.type": "#microsoft.graph.openIdConnectIdentityProvider",
  "id": "String (identifier)",
  "displayName": "String",
  "clientId": "String",
  "clientSecret": "String",
  "scope": "String",
  "metadataUrl": "String",
  "domainHint": "String",
  "responseType": "String",
  "responseMode": "String",
  "claimsMapping": {
    "@odata.type": "microsoft.graph.claimsMapping"
  }
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
