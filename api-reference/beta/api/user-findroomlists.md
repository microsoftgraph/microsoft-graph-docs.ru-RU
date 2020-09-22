---
title: 'user: findRoomLists'
description: Получение списка помещений, определенных в клиенте.
author: vrod9429
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0f1772b852844710b767ab646c9241782797a448
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017152"
---
# <a name="user-findroomlists"></a>user: findRoomLists

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка помещений, определенных в клиенте, в соответствии с представлением в их объектах [emailAddress](../resources/emailaddress.md).

Клиенты могут упорядочивать помещения для собраний в списках помещений. В этом API каждое помещение для собрания и список помещений представлены экземпляром [emailAddress](../resources/emailaddress.md).
Можно получить все списки помещений в клиенте, [получить все помещения](user-findrooms.md) в клиенте или [получить все помещения](user-findrooms.md) в определенном списке помещений.


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.ReadBasic.All, User.Read.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | User.Read.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/{id}/findRoomLists

```

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание |
|:---------------|:----------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |
| Content-Type  | string  | application/json. Обязательный. |


## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [emailAddress](../resources/emailaddress.md) в тексте отклика.

Если в клиенте не определены списки, возвращается пустой массив.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/findRoomLists
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-room-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-room-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-room-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
Ниже приведен пример отклика. 

Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "name": "user_get_room_lists",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAddress",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAddress)",
    "value": [
        {
            "name": "Building 1 Rooms",
            "address": "Building1Rooms@contoso.onmicrosoft.com"
        },
        {
            "name": "Building 2 Rooms",
            "address": "Building2Rooms@contoso.onmicrosoft.com"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: findRoomLists",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


