---
title: Создание identityProvider
description: Создание нового объекта identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: b2ed83bb828ae7b9d78572c8601e311bd4d10a7f
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491115"
---
# <a name="create-identityprovider"></a>Создание identityProvider

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового [объекта socialIdentityProvider](../resources/socialidentityprovider.md) в Azure AD.

В Azure AD B2C создайте новый [объект socialIdentityProvider,](../resources/socialidentityprovider.md) [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) или [объект appleIdentityProvider.](../resources/appleidentityprovider.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|IdentityProvider.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Приложение|IdentityProvider.ReadWrite.All|

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

В теле запроса укажи JSON представление [объекта socialIdentityProvider](../resources/socialidentityprovider.md) в Azure AD.

В Azure AD B2C предоставляют JSON представление [socialIdentityProvider,](../resources/socialidentityprovider.md) [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) или [объекта appleIdentityProvider.](../resources/appleidentityprovider.md)

Все свойства, перечисленные в приведенной ниже таблице, являются обязательными.

### <a name="socialidentityprovider-object"></a>объект socialIdentityProvider

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|clientId|String|Идентификатор клиента для приложения, полученного при регистрации приложения с поставщиком удостоверений.|
|clientSecret|String|Секрет клиента для приложения, полученного при регистрации приложения у поставщика удостоверений. Только для записи. Операция чтения возвращается \* \* \* \* ".|
|displayName|String|Отображаемое имя поставщика удостоверений.|
|identityProviderType|String|Для сценария B2B возможные значения: `Google` , `Facebook` . Для сценария B2C возможные значения: `Microsoft` , , , , , , , , `Google` , `Amazon` `LinkedIn` `Facebook` `GitHub` `Twitter` `Weibo` `QQ` `WeChat` .|

### <a name="openidconnectidentityprovider-object"></a>объект openIdConnectIdentityProvider

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|clientId|String|Идентификатор клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений.|
|clientSecret|Строка|Секрет клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений. ClientSecret имеет зависимость от **responseType**. <ul><li>Когда **responseType** — это секрет, необходимый `code` для обмена кодами auth.</li><li>Когда **responseType** является секретом, не требуется, так как не существует обмена кодом id_token возвращается непосредственно `id_token` из ответа авторизации.</li></ul>|
|displayName|String|Отображаемое имя поставщика удостоверений.|
|domainHint|String|Подсказку домена можно использовать для перехода непосредственно на вход на страницу указанного поставщика удостоверений вместо того, чтобы пользователь вошел в список доступных поставщиков удостоверений.|
|claimsMapping|[claimsMapping](../resources/claimsmapping.md)|После того как поставщик OIDC отправляет маркер ID обратно в Azure AD, Azure AD должна иметь возможность составить карту утверждений от полученного маркера к утверждениям, которые Azure AD распознает и использует. Этот сложный тип захватывает это сопоставление.|
|metadataUrl|String|URL-адрес документа метаданных поставщика удостоверений OpenID Connect. Каждый поставщик удостоверений OpenID Connect описывает документ метаданных, содержащий большую часть сведений, необходимых для выполнения входных данных. К ним относятся такие сведения, как URL-адреса для использования и расположение общедоступных ключей подписи службы. Документ метаданных OpenID Connect всегда расположен в конечной точке, в которую заканчивается `.well-known/openid-configuration` . Укажет URL-адрес метаданных для поставщика удостоверений OpenID Connect, который вы добавляете.|
|responseMode|String|Режим ответа определяет метод, используемый для отправки данных из пользовательского поставщика удостоверений в Azure AD B2C. Возможные значения: `form_post` , `query` .|
|responseType|String|Тип ответа описывает тип сведений, отосланных во время первоначального вызова authorization_endpoint поставщика пользовательских удостоверений. Возможные значения: `code` `id_token` , `token` .|
|scope|String|Область определяет сведения и разрешения, которые вы хотите получить от настраиваемого поставщика удостоверений.|

### <a name="appleidentityprovider-object"></a>объект appleIdentityProvider

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|displayName|String|Отображаемое имя поставщика удостоверений.|
|developerId|String|Идентификатор разработчика Apple.|
|serviceId|String|Идентификатор разработчика Apple.|
|keyId|String|Идентификатор Ключа Apple.|
|certificateData|String|Данные сертификата, которые является длинной строкой текста из сертификата, могут быть null.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и представление JSON объекта `201 Created` [socialIdentityProvider](../resources/socialidentityprovider.md) в тексте ответа для клиента Azure AD.

Для клиента Azure AD B2C этот метод возвращает код отклика и представление JSON для `201 Created` [socialIdentityProvider,](../resources/socialidentityprovider.md) [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) или [объекта appleIdentityProvider](../resources/appleidentityprovider.md) в тексте ответа.

В случае неудачи возвращается ошибка `4xx` с подробностями.

## <a name="examples"></a>Примеры

### <a name="example-1-create-a-specific-social-identity-provider-azure-ad-and-azure-ad-b2c"></a>Пример 1. Создание конкретного **поставщика социальных удостоверений** (Azure AD и Azure AD B2C)

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "create_socialidentityprovider_from_identityproviderbase"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/identityProviders
Content-type: application/json
Content-length: 154

{
  "@odata.type": "microsoft.graph.socialIdentityProvider",
  "displayName": "Login with Amazon",
  "identityProviderType": "Amazon",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "000000000000"
}
```

---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

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

### <a name="example-2-create-a-specific-openid-connect-identity-provider-only-for-azure-ad-b2c"></a>Пример 2. Создание конкретного **поставщика удостоверений OpenID Connect** (только для Azure AD B2C)

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "create_openidconnectidentityprovider_from_identityproviderbase"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/identityProviders
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider",
    "displayName": "Login with the Contoso identity provider",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "12345",
    "claimsMapping": {
        "userId": "myUserId",
        "givenName": "myGivenName",
        "surname": "mySurname",
        "email": "myEmail",
        "displayName": "myDisplayName"
    },
    "domainHint": "mycustomoidc",
    "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
    "responseMode": "form_post",
    "responseType": "code",
    "scope": "openid"
}

```

---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider",
  "id": "OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a",
  "displayName": "Login with the Contoso identity provider",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "12345",
  "claimsMapping": {
      "userId": "myUserId",
      "givenName": "myGivenName",
      "surname": "mySurname",
      "email": "myEmail",
      "displayName": "myDisplayName"
  },
  "domainHint": "mycustomoidc",
  "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
  "responseMode": "form_post",
  "responseType": "code",
  "scope": "openid"
}
```

### <a name="example-3-retrieves-apple-identity-provider-only-for-azure-ad-b2c"></a>Пример 3. Извлечение поставщика удостоверений Apple (только для Azure AD B2C)

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "create_applemanagedidentityprovider_from_identityproviderbase"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/identityProviders
Content-type: application/json
Content-length: 154

{
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider",
  "displayName": "Sign in with Apple",
  "developerId": "UBF8T346G9",
  "serviceId": "com.microsoft.rts.b2c.test.client",
  "keyId": "99P6D879C4",
  "certificateData": "******"
}
```

---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

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
