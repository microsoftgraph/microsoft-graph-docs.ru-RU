---
title: тип ресурса openIdConnectProvider
description: Представляет поставщики удостоверений OpenIDConnect в клиенте Azure Active Directory B2C.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: cbc2e95b04ec4ce8ce3c5472a1be61e743a008fa
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444093"
---
# <a name="openidconnectprovider-resource-type"></a>тип ресурса openIdConnectProvider

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет поставщики удостоверений OpenID Connect в клиенте Azure Active Directory B2C. 

Настройка поставщика OpenID Connect в клиенте B2C позволяет пользователям зарегистрироваться и войти с помощью настраиваемого поставщика удостоверений в приложении.

Наследует [от identityProvider](../resources/identityprovider.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление](../api/identityprovider-list.md)|Коллекция объектов identityProvider|Получение всех поставщиков удостоверений, настроенных в клиенте.|
|[Создание](../api/identityprovider-post-identityproviders.md)|identityProvider|Создание нового поставщика удостоверений OpenID Connect.|
|[Получение](../api/identityprovider-get.md) |identityProvider|Извлечение свойств поставщика удостоверений OpenID Connect.|
|[Обновление](../api/identityprovider-update.md)|Нет|Обновление поставщика удостоверений OpenID Connect.|
|[удаление](../api/identityprovider-delete.md);|Нет|Удаление поставщика удостоверений OpenID Connect.|
|[Перечисление доступных типов поставщиков](../api/identityprovider-list-availableprovidertypes.md)|Коллекция String|Получение всех доступных типов поставщиков удостоверений.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|clientId|String|Идентификатор клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений. Унаследованный от [identityProvider](../resources/identityprovider.md). Это обязательное свойство.|
|clientSecret|Строка|Секрет клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений. ClientSecret имеет зависимость от responseType. В случае responseType = code для обмена кодом auth требуется секрет, но в случае responseType = id_token не требуется, так как не существует обмена кодом, id_token возвращается непосредственно из ответа авторизации. Это только для записи. Операция чтения возвращает "\*\*\*\*". Унаследованный от [identityProvider](../resources/identityprovider.md).|
|id|String|Идентификатор поставщика удостоверений. Это обязательное свойство, считывалось только после создания.|
|name|String|Отображаемое имя поставщика удостоверений. Это обязательное свойство, считывалось только после создания.|
|type|String|Тип поставщика удостоверений Это должно быть `OpenIDConnect` . Это обязательное свойство, считывалось только после создания.|
|claimsMapping|[claimsMapping](../resources/claimsmapping.md)|После того как поставщик OIDC отправляет маркер ID обратно в Azure AD, Azure AD должна иметь возможность составить карту утверждений от полученного маркера к утверждениям, которые Azure AD распознает и использует. Этот сложный тип захватывает это сопоставление. Это обязательное свойство.|
|domainHint|String|Подсказку домена можно использовать для перехода непосредственно на вход на страницу указанного поставщика удостоверений вместо того, чтобы пользователь вошел в список доступных поставщиков удостоверений.|
|metadataUrl|String|URL-адрес документа метаданных поставщика удостоверений OpenID Connect. Каждый поставщик удостоверений OpenID Connect описывает документ метаданных, содержащий большую часть сведений, необходимых для выполнения входных данных. К ним относятся такие сведения, как URL-адреса для использования и расположение общедоступных ключей подписи службы. Документ метаданных OpenID Connect всегда расположен в конечной точке, которая заканчивается конфигурацией .well-known/openid-configuration. Для поставщика удостоверений OpenID Connect, который вы хотите добавить, необходимо уложить URL-адрес метаданных. Это обязательное свойство, считывалось только после создания.|
|responseMode|String|Режим ответа определяет метод, который следует использовать для отправки данных из настраиваемого поставщика удостоверений в Azure AD B2C. Можно использовать следующие режимы ответа: <ul><li/>`form_post` . Этот режим ответа рекомендуется для лучшей безопасности. Ответ передается методом HTTP POST, код или маркер кодируются в теле с помощью формата application/x-www-form-urlencoded.<li/>`query` Код или маркер возвращаются в качестве параметра запроса.</ul> Это обязательное свойство.|
|responseType|String|Тип ответа описывает, какие сведения отправляются обратно в начальном вызове authorization_endpoint поставщика пользовательских удостоверений. Можно использовать следующие типы ответов:<ul><li/> `code` . В результате потока кода авторизации код возвращается обратно в Azure AD B2C. Azure AD B2C продолжает вызывать token_endpoint, чтобы обменять код на маркер.<li/> `id_token` . Маркер ID возвращается обратно в Azure AD B2C от настраиваемого поставщика удостоверений. <li/>`token` . Маркер доступа возвращается обратно в Azure AD B2C от настраиваемого поставщика удостоверений. (На данный момент это значение не поддерживается Azure AD B2C)</ul> Это обязательное свойство.|
|scope|String|Область определяет сведения и разрешения, которые вы хотите получить от настраиваемого поставщика удостоверений. Запросы OpenID Connect должны содержать значение области openid для получения маркера ID от поставщика удостоверений. Без маркера ID пользователи не могут войти в Azure AD B2C с помощью настраиваемого поставщика удостоверений. Другие области могут быть разделены пространством. Дополнительные сведения об ограничениях области см. в разделе [RFC6749 Раздел 3.3](https://tools.ietf.org/html/rfc6749#section-3.3). Это обязательное свойство.|

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


