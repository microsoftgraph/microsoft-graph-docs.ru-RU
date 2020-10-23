---
title: Удаление Конверсатионмембер
description: Удаление Конверсатионмембер из канала.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6eb295dc9bc9f62172513e9d55c43394d36093ec
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700902"
---
# <a name="delete-conversationmember"></a>Удаление Конверсатионмембер

Пространство имен: microsoft.graph

Удаление [конверсатионмембер](../resources/conversationmember.md) из [канала](../resources/channel.md).


## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|---------|-------------|
|Делегированные (рабочая или учебная учетная запись)| Чаннелмембер. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений| Чаннелмембер. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL |

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

## <a name="response"></a>Отклик

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
DELETE https://graph.microsoft.com/V1.0/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[C#](#tab/csharp)

# <a name="javascript"></a>[JavaScript](#tab/javascript)

# <a name="objective-c"></a>[Objective-C](#tab/objc)

---

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
