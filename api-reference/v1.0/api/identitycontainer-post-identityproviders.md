---
title: Создание identityProvider
description: Создание нового объекта identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 80e5aa72d878b4869a15cbd3ca127701f52c3470
ms.sourcegitcommit: f99dc2b6c8b4cb6f9f74cd780dccc47a2bccfaa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2021
ms.locfileid: "58668038"
---
# <a name="create-identityprovider"></a>Создание identityProvider
Пространство имен: microsoft.graph

Создайте ресурс поставщика удостоверений, который имеет тип, указанный в теле запроса.

Среди типов поставщиков, полученных из identityProviderBase, в настоящее время можно создать ресурс [socialIdentityProvider](../resources/socialidentityprovider.md) в Azure AD. В Azure AD B2C эта операция в настоящее время может создать [ресурс socialIdentityProvider.](../resources/socialidentityprovider.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|IdentityProvider.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Для приложений|IdentityProvider.ReadWrite.All|

Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:

* Глобальный администратор
* Администратор внешнего поставщика удостоверений

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /identity/identityProviders
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---------------|:----------|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса укажи JSON представление объекта [socialIdentityProvider](../resources/socialidentityprovider.md) в Azure AD.

В Azure AD B2C предоставляется представление JSON объекта [socialIdentityProvider.](../resources/socialidentityprovider.md)

Все свойства, перечисленные в приведенной ниже таблице, являются обязательными.

### <a name="socialidentityprovider-object"></a>объект socialIdentityProvider

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|clientId|String|Идентификатор клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений.|
|clientSecret|String|Секрет клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений. Только для записи. Операция чтения возвращает `****`.|
|displayName|String|Отображаемое имя поставщика удостоверений.|
|identityProviderType|Строка|Возможные значения для сценария B2B: `Google`, `Facebook`. Возможные значения для сценария B2C: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`, `QQ`, `WeChat`.|
|scope|String|Область определяет сведения и разрешения, которые вы хотите получить от настраиваемого поставщика удостоверений.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и представление JSON объекта `201 Created` [socialIdentityProvider](../resources/socialidentityprovider.md) в тексте ответа для клиентов Azure AD и Azure AD B2C.

В случае неудачи возвращается ошибка `4xx` с подробностями.

## <a name="examples"></a>Примеры

### <a name="example-1-create-a-specific-social-identity-provider-azure-ad-and-azure-ad-b2c"></a>Пример 1. Создание конкретного поставщика социальных удостоверений (Azure AD и Azure AD B2C)

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_socialidentityprovider_from_identityproviderbase"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identity/identityProviders
Content-type: application/json

{
  "@odata.type": "microsoft.graph.socialIdentityProvider",
  "displayName": "Login with Amazon",
  "identityProviderType": "Amazon",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "000000000000"
}

```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-socialidentityprovider-from-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-socialidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-socialidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-socialidentityprovider-from-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.socialIdentityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.type": "microsoft.graph.socialIdentityProvider",
    "id": "Amazon-OAUTH",
    "displayName": "Login with Amazon",
    "identityProviderType": "Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "000000000000"
}
```
