---
title: 'cloudCommunications: getPresencesByUserId'
description: Получите сведения о присутствии для нескольких пользователей.
author: ananmishr
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 0a545df4e1195d057e5155ab18f5bcfe17de9102
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059914"
---
# <a name="cloudcommunications-getpresencesbyuserid"></a>cloudCommunications: getPresencesByUserId

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите сведения [о](../resources/presence.md) присутствии для нескольких пользователей.

## <a name="permissions"></a>Разрешения
Для вызова этих API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения | Разрешения (в порядке повышения привилегий)                  |
| :-------------- | :----------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Presence.Read.All                         |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                         |
| Приложение                            | Не поддерживается.                                  |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /communications/getPresencesByUserId
```

## <a name="request-headers"></a>Запрашивать заглавные
| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {токен}. Обязательный. |
|Content-Type | application/json. Обязательный. |


## <a name="request-body"></a>Текст запроса

В теле запроса укажи объект JSON со следующим параметром.

| Параметр      | Тип    |Описание|
|:---------------|:--------|:----------|
|ids|Коллекция String|ID объекта пользователя.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` присутствия в тексте ответа. [](../resources/presence.md)


## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже показан пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-presence-multiple-users"
}-->

```http
POST https://graph.microsoft.com/beta/communications/getPresencesByUserId
Content-Type: application/json

{
  "ids": ["fa8bf3dc-eca7-46b7-bad1-db199b62afc3", "66825e03-7ef5-42da-9069-724602c31f6b"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-presence-multiple-users-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-presence-multiple-users-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-presence-multiple-users-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-presence-multiple-users-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик
Ниже приводится пример отклика.

> **Примечание:** Объекты отклика могут быть сокращены для читаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "name": "get-presence-multiple-users",
  "truncated": "true",
  "@odata.type": "microsoft.graph.presence"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
   "value":[
      {
         "id":"fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
         "availability":"Busy",
         "activity":"InAMeeting",
         "outOfOfficeSettings":{
            "message":null,
            "isOutOfOffice":false
         }
      },
      {
         "id":"66825e03-7ef5-42da-9069-724602c31f6b",
         "availability":"Away",
         "activity":"Away",
         "outOfOfficeSettings":{
            "message":null,
            "isOutOfOffice":true
         }
      }
   ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List Presence Information",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


