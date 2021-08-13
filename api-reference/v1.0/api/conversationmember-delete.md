---
title: Удаление conversationMember
description: Удаление conversationMember из канала.
author: akjo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fb06950403e6f49421fdc600fd5b3d47023b00f12145bf77fab78b08b3ae3691
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54172612"
---
# <a name="delete-conversationmember"></a>Удаление conversationMember

Пространство имен: microsoft.graph

Удаление [conversationMember из](../resources/conversationmember.md) [канала](../resources/channel.md).


## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|---------|-------------|
|Делегированные (рабочая или учебная учетная запись)| ChannelMember.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение| ChannelMember.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса

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
