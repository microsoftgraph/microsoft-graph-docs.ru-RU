---
title: Обновление identityProvider
description: Обновление свойств identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: a88ba5fbac97b501b54e63e60276cb7a4026729d
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535502"
---
# <a name="update-identityprovider"></a>Обновление identityProvider
Пространство имен: microsoft.graph

Обновление свойств объекта [socialIdentityProvider](../resources/socialidentityprovider.md) в Azure AD.

В Azure AD B2C обновим свойства [объекта socialIdentityProvider.](../resources/socialidentityprovider.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|IdentityProvider.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Для приложений| IdentityProvider.ReadWrite.All|

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

В теле запроса укажи тип OData и объект JSON одним или более свойствами, которые необходимо обновить для объекта [socialIdentityProvider](../resources/socialidentityprovider.md) в клиенте Azure AD.

В Azure AD B2C укажи тип OData и объект JSON одним или более свойствами, которые необходимо обновить для [объекта socialIdentityProvider.](../resources/socialidentityprovider.md)

### <a name="socialidentityprovider-object"></a>объект socialIdentityProvider

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|clientId|String|Идентификатор клиентского приложения, полученный при регистрации приложения у поставщика удостоверений.|
|clientSecret|String|Секрет клиента для приложения, полученный при регистрации приложения с помощью поставщика удостоверений. Только для записи. Операция чтения возвращает "\*\*\*\*".|
|displayName|String|Отображаемое имя поставщика удостоверений.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В случае неудачи возвращается ошибка `4xx` с подробностями.

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
PATCH https://graph.microsoft.com/v1.0/identity/identityProviders/Amazon-OAUTH
Content-type: application/json

{
  "@odata.type": "microsoft.graph.socialIdentityProvider",
  "clientSecret": "1111111111111"
}
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```