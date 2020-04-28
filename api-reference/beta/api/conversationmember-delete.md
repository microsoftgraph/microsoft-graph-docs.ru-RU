---
title: Удаление Конверсатионмембер
description: Удаление Конверсатионмембер из канала.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0a6ac8b72f5dea24c0f60062b91dac7648b91e85
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436568"
---
# <a name="delete-conversationmember"></a>Удаление Конверсатионмембер

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаление [конверсатионмембер](../resources/conversationmember.md) из [канала](../resources/channel.md).

> [!NOTE]
> Эта операция поддерживается только для каналов с [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) `private`. Вызовы с любым другим [чаннелмембершиптипе](../resources/enums.md#channelmembershiptype-values) будут возвращать `400 Bad Request` ответ.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|---------|-------------|
|Делегированные (рабочая или учебная учетная запись)|Для ресурса **user** или **chat**:<br/>Chat.Read, Chat.ReadWrite<br/><br/>Для ресурса **channel**:<br/>Group.Read.All, Group.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение| Для ресурса **user** или **chat**:<br/>Chat.Read.All, Chat.ReadWrite.All<br/><br/>Для ресурса **channel**:<br/>Group.Read.All, Group.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Ответ

Ниже приведен пример отклика.

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
