---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Список последних файлов
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c0462d98a26ab053ba47f1dda8b739dbd5f4806a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260314"
---
# <a name="list-recent-files"></a>Список последних файлов

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указание набора элементов, которые недавно использовались пользователем, вошедшим в свою учетную запись. Эта коллекция содержит элементы, которые находятся на диске пользователя, а также элементы, к которым у него есть доступ с других дисков.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All    |
|Для приложений | Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "request",
       "name": "view-recent-files", 
       "scopes": "files.read",
       "target": "action" } -->

```http
GET /me/drive/recent
```

## <a name="response"></a>Отклик

Этот метод возвращает коллекцию ресурсов [DriveItem](../resources/driveitem.md) для элементов, к которым владелец объекта drive недавно получал доступ.

<!-- { "blockType": "response",
       "@odata.type": "Collection(microsoft.graph.driveItem)",
       "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1312abc!1231",
      "remoteItem":
      {
        "id": "1991210caf!192",
        "name": "March Proposal.docx",
        "file": { },
        "size": 19121,
        "parentReference": {
          "driveId": "1991210caf",
          "id": "1991210caf!104"
        }
      },
      "fileSystemInfo": {
        "lastAccessedDateTime": "2017-02-20T19:13:00Z"
      }
    },
    {
      "id": "1312def!9943",
      "name": "Vacation.jpg",
      "file": { },
      "size": 37810,
      "parentReference": {
        "driveId": "1312def",
        "id": "1312def!123"
      },
      "fileSystemInfo": {
        "lastAccessedDateTime": "2017-02-20T16:43:21Z"
      }
    }
  ]
}
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/view-recent-files-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/view-recent-files-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/view-recent-files-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a>Замечания

Некоторые элементы driveItem, возвращенные **последним** действием, будут содержать аспект **remoteItem**, который указывает, что это элементы с другого диска. Чтобы получить доступ к исходному объекту driveItem, следует отправить запрос, используя данные, указанные в **remoteItem** в следующем формате:

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!--
{
  "type": "#page.annotation",
  "description": "Retrieve a list of recently used files for the owner of the drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Drives/Recent files",
  "suppressions": [
    "Error: /api-reference/beta/api/drive-recent.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/drive-recent.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-recent.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
