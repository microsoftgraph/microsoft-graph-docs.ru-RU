---
title: Обновление identityProvider
description: Обновление свойств identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 985a6d4c80187decd5770eca150f501786222a1c
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491120"
---
# <a name="update-identityprovider"></a>Обновление identityProvider
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [socialIdentityProvider](../resources/socialidentityprovider.md) в Azure AD.

В Azure AD B2C обновим свойства [объекта socialIdentityProvider,](../resources/socialidentityprovider.md) [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) или [объекта appleIdentityProvider.](../resources/appleidentityprovider.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|IdentityProvider.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Приложение| IdentityProvider.ReadWrite.All|

Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:

* Глобальный администратор
* Администратор внешнего поставщика удостоверений

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/identityProviders/{id}
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---------------|:----------|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса укажи объект JSON одним или более свойствами, которые необходимо обновить для объекта [socialIdentityProvider](../resources/socialidentityprovider.md) в клиенте Azure AD.

В Azure AD B2C предоставить объекту JSON одно или несколько свойств, которые необходимо обновить для [socialIdentityProvider,](../resources/socialidentityprovider.md) [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) или [объекта appleIdentityProvider.](../resources/appleidentityprovider.md)

### <a name="socialidentityprovider-object"></a>объект socialIdentityProvider

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|clientId|String|Идентификатор клиента для приложения, полученного при регистрации приложения с поставщиком удостоверений.|
|clientSecret|String|Секрет клиента для приложения, полученного при регистрации приложения у поставщика удостоверений. Только для записи. Операция чтения возвращается \* \* \* \* ".|
|displayName|String|Отображаемое имя поставщика удостоверений.|

### <a name="openidconnectidentityprovider-object"></a>объект openIdConnectIdentityProvider

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|clientId|String|Идентификатор клиента для приложения, полученного при регистрации приложения с поставщиком удостоверений.|
|clientSecret|Строка|Секрет клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений. ClientSecret имеет зависимость от **responseType**. <ul><li>Когда **responseType** — это секрет, необходимый `code` для обмена кодами auth.</li><li>Когда **responseType** `id_token` является секретом, не требуется, так как не существует обмена кодом. Ответ id_token возвращается непосредственно из ответа авторизации.</li></ul>|
|displayName|String|Отображаемое имя поставщика удостоверений.|
|domainHint|String|Подсказку домена можно использовать для перехода непосредственно на вход на страницу указанного поставщика удостоверений вместо того, чтобы пользователь вошел в список доступных поставщиков удостоверений.|
|claimsMapping|[claimsMapping](../resources/claimsmapping.md)|После того как поставщик OIDC отправляет маркер ID обратно в Azure AD, Azure AD должна иметь возможность составить карту утверждений от полученного маркера к утверждениям, которые Azure AD распознает и использует. Этот сложный тип захватывает это сопоставление.|
|metadataUrl|String|URL-адрес документа метаданных поставщика удостоверений OpenID Connect. Каждый поставщик удостоверений OpenID Connect описывает документ метаданных, содержащий большую часть сведений, необходимых для выполнения входных данных. К ним относятся такие сведения, как URL-адреса для использования и расположение общедоступных ключей подписи службы. Документ метаданных OpenID Connect всегда расположен в конечной точке, в которую заканчивается `.well-known/openid-configuration` . Укажет URL-адрес метаданных для поставщика удостоверений OpenID Connect, который вы добавляете.|
|responseMode|String|Режим ответа определяет метод, используемый для отправки данных из пользовательского поставщика удостоверений в Azure AD B2C. Возможные значения: `form_post` , `query` .|
|responseType|String|Тип ответа описывает тип сведений, отосланных во время первоначального вызова authorization_endpoint поставщика пользовательских удостоверений. Возможные значения: `code` `id_token` , `token` .|
|scope|String|Область определяет сведения и разрешения, которые вы хотите получить от настраиваемого поставщика удостоверений.|

### <a name="applemanagedidentityprovider-object"></a>объект appleManagedIdentityProvider

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|displayName|String|Отображаемое имя поставщика удостоверений.|
|developerId|String|Идентификатор разработчика Apple.|
|serviceId|String|Идентификатор разработчика Apple.|
|keyId|String|Идентификатор Ключа Apple.|
|certificateData|String|Данные сертификата, которые является длинной строкой текста из сертификата, могут быть null.|

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. В случае неудачи возвращается ошибка `4xx` с подробностями.

## <a name="examples"></a>Примеры

### <a name="example-1-update-a-specific-social-identity-provider-azure-ad-or-azure-ad-b2c"></a>Пример 1. Обновление определенного **поставщика социальных удостоверений** (Azure AD или Azure AD B2C)

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "update_socialidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/Amazon-OAUTH
Content-type: application/json
Content-length: 41

{
  "clientSecret": "1111111111111"
}
```

---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-openid-connect-identity-provider-only-for-azure-ad-b2c"></a>Пример 2. Обновление определенного **поставщика удостоверений OpenID Connect** (только для Azure AD B2C)

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "update_openidconnectprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/OIDC-V1-Nam_AD_Test-3e393390-ed2d-4794-97f6-5c999ccc61f7
Content-type: application/json
Content-length: 41

{
  "responseType": "id_token"
}
```

---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-a-specific-apple-identity-provider-only-for-azure-ad-b2c"></a>Пример 3. Обновление определенного **поставщика удостоверений Apple** (только для Azure AD B2C)

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "update_appleidentityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/identityProviders/Apple-Managed-OIDC
Content-type: application/json
Content-length: 41

{
  "displayName": "Apple"
}
```

---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
