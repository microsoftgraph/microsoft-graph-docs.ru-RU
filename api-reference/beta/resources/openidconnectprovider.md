---
title: тип ресурса openIdConnectProvider
description: Представляет поставщики удостоверений OpenIDConnect в клиенте Azure Active Directory B2C.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 47541ddb79d71068ed974d6095ef2f8572bd9e5c
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "53580858"
---
# <a name="openidconnectprovider-resource-type-deprecated"></a>тип ресурса openIdConnectProvider (неподготовленный)
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

Представляет поставщики удостоверений Подключение OpenID в клиенте Azure Active Directory B2C.

Настройка поставщика openID Подключение в клиенте B2C позволяет пользователям зарегистрироваться и войти в использование настраиваемого поставщика удостоверений в приложении.

Наследует [от identityProvider](../resources/identityprovider.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление](../api/identityprovider-list.md)|Коллекция объектов identityProvider|Получение всех поставщиков удостоверений, настроенных в клиенте.|
|[Создание](../api/identityprovider-post-identityproviders.md)|openIdConnectProvider|Создание нового поставщика удостоверений Подключение OpenID.|
|[Получение](../api/identityprovider-get.md) |openIdConnectProvider|Извлечение свойств поставщика удостоверений Подключение OpenID.|
|[Обновление](../api/identityprovider-update.md)|Нет|Обновление поставщика удостоверений Подключение OpenID.|
|[Удаление](../api/identityprovider-delete.md)|Нет|Удаление поставщика удостоверений Подключение OpenID.|
|[Перечисление доступных типов поставщиков](../api/identityprovider-list-availableprovidertypes.md)|Коллекция String|Получение всех доступных типов поставщиков удостоверений.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|clientId|String|Идентификатор клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений. Унаследованный от [identityProvider](../resources/identityprovider.md). Это обязательное свойство.|
|clientSecret|Строка|Секрет клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений. ClientSecret имеет зависимость от **responseType**. Когда **responseType** — это секрет, необходимый `code` для обмена кодами auth. Когда **responseType** является секретом, не требуется, так как нет обмена кодом, возвращается непосредственно `id_token` из ответа `id_token` авторизации. Только для записи. Операция чтения возвращает "\*\*\*\*". Унаследованный от [identityProvider](../resources/identityprovider.md).|
|id|String|Идентификатор поставщика удостоверений. Это обязательное свойство, считывалось только после создания.|
|name|String|Отображаемое имя поставщика удостоверений. Это обязательное свойство, считывалось только после создания.|
|type|String|Тип поставщика удостоверений Это должно быть `OpenIDConnect` . Это обязательное свойство, считывалось только после создания.|
|claimsMapping|[claimsMapping](../resources/claimsmapping.md)|После того как поставщик OIDC отправляет маркер ID обратно в Azure AD, Azure AD должна иметь возможность составить карту утверждений от полученного маркера к утверждениям, которые Azure AD распознает и использует. Этот сложный тип захватывает это сопоставление. Это обязательное свойство.|
|domainHint|String|Подсказка домена может быть использована для пропуска непосредственно на страницу регистрации указанного поставщика удостоверений вместо того, чтобы пользователь вошел в список доступных поставщиков удостоверений.|
|metadataUrl|String|URL-адрес документа метаданных поставщика удостоверений OpenID Подключение. Каждый поставщик Подключение OpenID описывает документ метаданных, содержащий большую часть сведений, необходимых для выполнения входных данных. К ним относятся такие сведения, как URL-адреса для использования и расположение общедоступных ключей подписи службы. Документ Подключение openID всегда расположен в конечной точке, которая заканчивается конфигурацией .well-known/openid-configuration. Для поставщика удостоверений OpenID Подключение, который вы хотите добавить, необходимо предоставить URL-адрес метаданных. Это обязательное свойство, считывалось только после создания.|
|responseMode|openIdConnectResponseMode|Режим ответа определяет метод, который следует использовать для отправки данных из настраиваемого поставщика удостоверений в Azure AD B2C. Можно использовать следующие режимы ответа: `form_post` , `query` . `query` Режим ответа означает, что код или маркер возвращаются в качестве параметра запроса. `form_post` Режим ответа рекомендуется для обеспечения наилучшей безопасности. Ответ передается методом HTTP POST, код или маркер кодируются в теле с помощью формата application/x-www-form-urlencoded. Это обязательное свойство.|
|responseType|[openIdConnectResponseTypes](#openidconnectresponsetypes-values)| Тип ответа описывает, какие сведения отправляются обратно в начальном вызове authorization_endpoint поставщика пользовательских удостоверений. Можно использовать следующие типы ответов: `code` , `id_token` `token` . Это обязательное свойство.|
|scope|String|Область определяет сведения и разрешения, которые вы хотите получить от настраиваемого поставщика удостоверений. Запросы Подключение OpenID должны содержать значение области openid для получения маркера ID от поставщика удостоверений. Без маркера ID пользователи не могут войти в Azure AD B2C с помощью настраиваемого поставщика удостоверений. Другие области могут быть разделены пространством. Дополнительные сведения об ограничениях области см. в разделе [RFC6749 Раздел 3.3](https://tools.ietf.org/html/rfc6749#section-3.3). Это обязательное свойство.|

### <a name="openidconnectresponsetypes-values"></a>значения openIdConnectResponseTypes

|Member|Описание|
|:---|:---|
|code|В течение потока кода авторизации код возвращается обратно в Azure AD B2C. Azure AD B2C продолжает вызывать token_endpoint, чтобы обменять код на маркер.|
|id_token|Маркер ID возвращается обратно в Azure AD B2C от настраиваемого поставщика удостоверений. |
|token|Маркер доступа возвращается обратно в Azure AD B2C от настраиваемого поставщика удостоверений. В настоящее время не поддерживается Azure AD B2C. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.openIdConnectProvider"
} -->

```json
{
  "id": "String",
  "name": "String",
  "type": "String",
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
