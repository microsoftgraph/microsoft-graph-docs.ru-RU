---
title: Обновление identityProvider
description: Обновление свойств в существующий identityProvider.
ms.openlocfilehash: b89b0f50ef2f62625a1707c3e77c32865adaec67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077509"
---
# <a name="update-identityprovider"></a>Обновление identityProvider

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Обновление свойств в существующий [identityProvider](../resources/identityprovider.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|IdentityProvider.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается.|
|Для приложений|Не поддерживается.|

Трудовые или школы учетной записи необходимо быть глобальным администратором клиента.

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

Предоставить объект JSON в тексте запроса одно или несколько свойств, которые должны быть обновлены.

|Свойство|Тип|Description|
|:---------------|:--------|:----------|
|clientId|String|Идентификатор клиента для приложения. Это идентификатор клиента, полученные при регистрации приложения с поставщиком удостоверений.|
|clientSecret|String|Секрет клиента для приложения. Это секрет клиента, полученные при регистрации приложения с поставщиком удостоверений.|
|name|String|Отображаемое имя поставщика удостоверений.|

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В случае неудачи `4xx` будут возвращены с подробные сведения об ошибке.

## <a name="example"></a>Пример

В следующем примере происходит обновление определения срока жизни маркера **identityProvider** и устанавливает ее в качестве организации по умолчанию.

##### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "update_identityprovider"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
Content-type: application/json
Content-length: 41

{
    "clientSecret": "1111111111111"
}
```

##### <a name="response"></a>Ответ

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->