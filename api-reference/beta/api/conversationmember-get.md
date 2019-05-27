---
title: Получение conversationMember
description: Получение участника чата.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: a2c539b7240060a6434f5ece01dc242ae948a5f4
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2019
ms.locfileid: "34379304"
---
# <a name="get-conversationmember"></a>Получение conversationMember

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение объекта [conversationMember](../resources/conversationmember.md) из [чата](../resources/chat.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|---------|-------------|
|Делегированные (рабочая или учебная учетная запись)|Chat.Read, Chat.ReadWrite|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Для приложений |Chat.Read.All, Chat.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/chats/{id}/members/{id}
```

##### <a name="response"></a>Отклик

Ниже приведен пример отклика. 

>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "display-name-value"
}
```