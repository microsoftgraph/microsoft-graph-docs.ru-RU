---
author: chackman
ms.author: chackman
title: Список отслеживаемых элементов
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0c7f7a072fb7960b1bc160c06367252fd183f9e4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260335"
---
# <a name="list-followed-items"></a>Список отслеживаемых элементов

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Список [элементов](../resources/driveitem.md) , за которыми подписан пользователь, вошедшего в систему.
Эта коллекция содержит элементы, которые находятся на диске пользователя, а также элементы, к которым у него есть доступ с других дисков.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```

## <a name="response"></a>Отклик

Этот метод возвращает коллекцию ресурсов [driveItem](../resources/driveitem.md) для элементов, которые подписаны владельцем диска.
Если не будет найдено ни одного элемента, то будет возвращена пустая коллекция.

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.driveItem)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "name": "March Proposal.docx",
      "size": 19121,
      "lastModifiedDateTime": "2017-12-12T10:40:59Z"
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "size": 37810,
      "lastModifiedDateTime": "2016-10-18T10:40:59Z"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get-followed-items-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-followed-items-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-followed-items-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "List the items a user is following.",
  "keywords": "drive,onedrive.drive,list followed items",
  "section": "documentation",
  "tocPath": "Drives/List followed items",
  "suppressions": [
    "Error: /api-reference/beta/api/drive-list-following.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/drive-list-following.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-list-following.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
