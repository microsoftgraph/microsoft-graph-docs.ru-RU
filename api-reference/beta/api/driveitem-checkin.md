---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Возврат файлов
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 18c06435e4fed868f13998a3724f4b13c0853c20
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861453"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a>Возврат изменений в ресурсе DriveItem

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В этой статье рассказывается, как возвратить извлеченный ресурс DriveItem, чтобы сделать версию документа доступной другим пользователям.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Files.ReadWrite, Files.ReadWrite.All    |
|Для приложений | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a>Тело запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.


|   Имя    | Значение  |                                                Описание                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| checkInAs | string | Необязательно. Желаемое состояние документа после завершения операции возврата. Может иметь значение `published` либо значение может быть не указано. |
| comment   | string | Комментарий к возврату, сопоставленный с версией.                                                   |

## <a name="example"></a>Пример

В этом примере показано, как возвратить файл, идентифицируемый по `{item-id}`.


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/checkin-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/checkin-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Цель — C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/checkin-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/checkin-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a>Отклик

При успешном выполнении вызова API возвращается отклик `204 No content`.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a>Замечания


[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
  ]
}
-->
