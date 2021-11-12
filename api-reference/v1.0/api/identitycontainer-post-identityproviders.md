---
title: Создание identityProvider
description: Создание нового объекта identityProvider.
ms.localizationpriority: medium
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 9c4c349ed366052ffc9fe5f422bb6fa536eb3357
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60891202"
---
# <a name="create-identityprovider"></a>Создание identityProvider
Пространство имен: microsoft.graph

Создайте ресурс поставщика удостоверений, который имеет тип, указанный в теле запроса.

Среди типов поставщиков, полученных из identityProviderBase, в настоящее время можно создать ресурс [socialIdentityProvider](../resources/socialidentityprovider.md) в Azure AD. В Azure AD B2C эта операция может создать [socialIdentityProvider](../resources/socialidentityprovider.md)или [ресурс appleManagedIdentityProvider.](../resources/applemanagedidentityprovider.md)

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
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Основной текст запроса

В теле запроса укажи JSON представление [объекта socialIdentityProvider](../resources/socialidentityprovider.md) в Azure AD.

В Azure AD B2C предоставляется JSON-представление [socialIdentityProvider](../resources/socialidentityprovider.md)или [объекта appleManagedIdentityProvider.](../resources/applemanagedidentityprovider.md)

### <a name="socialidentityprovider-object"></a>объект socialIdentityProvider

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|clientId|String|Идентификатор клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений.|
|clientSecret|String|Секрет клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений. Только для записи. Операция чтения возвращает `****`.|
|displayName|String|Отображаемое имя поставщика удостоверений.|
|identityProviderType|Строка|Возможные значения для сценария B2B: `Google`, `Facebook`. Возможные значения для сценария B2C: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`, `QQ`, `WeChat`.|
|scope|String|Область определяет сведения и разрешения, которые вы хотите получить от настраиваемого поставщика удостоверений.|

### <a name="appleidentityprovider-object"></a>объект appleIdentityProvider

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|displayName|String|Отображаемое имя поставщика удостоверений.|
|developerId|Строка|Идентификатор разработчика Apple.|
|serviceId|Строка|Идентификатор службы Apple.|
|keyId|Строка|Идентификатор ключа Apple.|
|certificateData|Строка|Данные сертификата, являющиеся длинной строкой текста из сертификата. Могут иметь значение NULL.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и представление JSON объекта `201 Created` [socialIdentityProvider](../resources/socialidentityprovider.md) в тексте ответа для клиента Azure AD.

Для клиента Azure AD B2C этот метод возвращает код отклика и представление JSON объекта `201 Created` [socialIdentityProvider](../resources/socialidentityprovider.md)или [объекта appleManagedIdentityProvider](../resources/applemanagedidentityprovider.md) в тексте ответа.

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

Ниже приведен пример ответа.

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

### <a name="example-2-retrieves-apple-identity-provider-only-for-azure-ad-b2c"></a>Пример 2. Извлечение поставщика удостоверений Apple (только для Azure AD B2C)

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "create_applemanagedidentityprovider_from_identityproviderbase"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identity/identityProviders
Content-type: application/json

{
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider",
  "displayName": "Sign in with Apple",
  "developerId": "UBF8T346G9",
  "serviceId": "com.microsoft.rts.b2c.test.client",
  "keyId": "99P6D879C4",
  "certificateData": "******"
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider",
  "id": "Apple-Managed-OIDC",
  "displayName": "Sign in with Apple",
  "developerId": "UBF8T346G9",
  "serviceId": "com.microsoft.rts.b2c.test.client",
  "keyId": "99P6D879C4",
  "certificateData": "******"
}
```
