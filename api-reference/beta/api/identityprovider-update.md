---
title: Обновление identityProvider
description: Обновление свойств объекта identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6bd2944211312c1b5440390f7a1c7a84de205e9f
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509702"
---
# <a name="update-identityprovider"></a>Обновление identityProvider

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [identityProvider](../resources/identityprovider.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|IdentityProvider.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Для приложений| IdentityProvider.ReadWrite.All|

Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:
* Глобальный администратор
* Администратор внешнего поставщика удостоверений

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /identityProviders/{id}
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---------------|:----------|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите объект JSON с одним или несколькими свойствами, которые необходимо обновить для объекта [identityProvider](../resources/identityprovider.md) или [опенидконнектпровидер](../resources/openidconnectprovider.md) (только для Azure AD B2C).

### <a name="identityprovider-object"></a>Объект identityProvider

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|clientId|String|Идентификатор клиента для приложения. Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.|
|clientSecret|String|Секрет клиента для приложения. Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.|
|name|String|Отображаемое имя поставщика удостоверений.|
|type|String|Тип поставщика удостоверений<ul>Для сценария B2B:<li/>Google<li/>Facebook</ul><ul>Для сценария B2C:<li/>Microsoft<li/>Google<li/>Amazon<li/>LinkedIn<li/>Facebook<li/>GitHub<li/>Twitter<li/>Weibo<li/>QQ<li/>WeChat<li/>опенидконнект</ul>|

### <a name="openidconnectprovider-object"></a>Объект Опенидконнектпровидер

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|clientId|String|Идентификатор клиента для приложения. Это идентификатор клиента, полученный при регистрации приложения с помощью поставщика удостоверений.|
|clientSecret|String|Секрет клиента для приложения. Это секрет клиента, полученный при регистрации приложения с помощью поставщика удостоверений.|
|name|String|Отображаемое имя поставщика удостоверений.|
|type|String|Тип поставщика удостоверений Значение должно быть `OpenIdConnect` .|
|клаимсмаппинг|[клаимсмаппинг](../resources/claimsmapping.md)|После того как поставщик ОИДК отправит токен ID обратно в Azure AD, Azure AD должен сопоставить утверждения из полученного маркера с утверждениями, которые служба Azure AD распознает и использует. Этот сложный тип захватывает это сопоставление.|
|domainHint|Строка|Подсказка домена может быть использована для пропуска непосредственно к странице входа указанного поставщика удостоверений вместо того, чтобы пользователь выделе выбор среди доступных поставщиков удостоверений.|
|metadataUrl|Строка|URL-адрес документа метаданных поставщика удостоверений подключения Open ID.|
|респонсемоде|Строка|Определяет метод, который должен использоваться для отправки данных обратно от настраиваемого поставщика удостоверений в Azure AD B2C. Можно использовать следующие режимы ответа: <ul><li/>`form_post`: Этот режим ответа рекомендуется для обеспечения лучшей безопасности. Ответ передается через HTTP-метод POST с кодом или маркером, закодированным в теле, с помощью формата Application/x-www-Form-урленкодед.<li/>`query`: Код или маркер возвращается в виде параметра запроса.</ul>|
|responseType|Строка|Описывает тип сведений, которые отправляются обратно при первом вызове authorization_endpoint настраиваемого поставщика удостоверений. Можно использовать следующие типы ответов:<ul><li/> `code`: В соответствии с процессом кода авторизации код вернется обратно в Azure AD B2C. B2C Azure AD выполняет вызов token_endpoint для обмена кодом для маркера.<li/> `id_token`: Токен ID возвращается обратно в Azure AD B2C из настраиваемого поставщика удостоверений. <li/>`token`: Маркер доступа возвращается обратно в Azure AD B2C из настраиваемого поставщика удостоверений. (В настоящее время это значение не поддерживается в Azure AD B2C)</ul>|
|scope|Строка|Область определяет сведения и разрешения, которые вы собираетесь получить от настраиваемого поставщика удостоверений.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В случае неудачи возвращается ошибка `4xx` с подробностями.

## <a name="examples"></a>Примеры

### <a name="example-1-update-a-specific-identityprovider"></a>Пример 1: обновление конкретной **identityProvider**

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "update_identityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
  "clientSecret": "1111111111111"
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-2-update-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a>Пример 2: обновление конкретной **опенидконнектпровидер** (только для Azure AD B2C)

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "update_openidconnectprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identityProviders/OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a
Content-type: application/json
Content-length: 41

{
  "responseType": "id_token"
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
