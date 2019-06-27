---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Список последних файлов
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1e1f376606eeefc9ee599992e6432c0b2830dd51
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35279095"
---
# <a name="list-recent-files"></a><span data-ttu-id="7f4c9-102">Список последних файлов</span><span class="sxs-lookup"><span data-stu-id="7f4c9-102">List recent files</span></span>

<span data-ttu-id="7f4c9-p101">Указание набора элементов, которые недавно использовались пользователем, вошедшим в свою учетную запись. Эта коллекция содержит элементы, которые находятся на диске пользователя, а также элементы, к которым у него есть доступ с других дисков.</span><span class="sxs-lookup"><span data-stu-id="7f4c9-p101">List a set of items that have been recently used by the signed in user. This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f4c9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f4c9-105">Permissions</span></span>

<span data-ttu-id="7f4c9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f4c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f4c9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f4c9-108">Permission type</span></span>      | <span data-ttu-id="7f4c9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f4c9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f4c9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f4c9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7f4c9-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4c9-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f4c9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f4c9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f4c9-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4c9-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f4c9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f4c9-114">Application</span></span> | <span data-ttu-id="7f4c9-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4c9-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f4c9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f4c9-116">HTTP request</span></span>

<!-- { "blockType": "request",
       "name": "view-recent-files", 
       "scopes": "files.read",
       "tags": "service.graph",
       "target": "action" } -->

```http
GET /me/drive/recent
```

## <a name="response"></a><span data-ttu-id="7f4c9-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f4c9-117">Response</span></span>

<span data-ttu-id="7f4c9-118">Этот метод возвращает коллекцию ресурсов [DriveItem](../resources/driveitem.md) для элементов, к которым владелец объекта drive недавно получал доступ.</span><span class="sxs-lookup"><span data-stu-id="7f4c9-118">This method returns a collection of [DriveItem](../resources/driveitem.md) resources for items which the owner of the drive has recently accessed.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7f4c9-119">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="7f4c9-119">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7f4c9-120">C#</span><span class="sxs-lookup"><span data-stu-id="7f4c9-120">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/view-recent-files-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f4c9-121">Javascript</span><span class="sxs-lookup"><span data-stu-id="7f4c9-121">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/view-recent-files-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7f4c9-122">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7f4c9-122">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/view-recent-files-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="7f4c9-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="7f4c9-123">Remarks</span></span>

<span data-ttu-id="7f4c9-p103">Некоторые элементы driveItem, возвращенные **последним** действием, будут содержать аспект **remoteItem**, который указывает, что это элементы с другого диска. Чтобы получить доступ к исходному объекту driveItem, следует отправить запрос, используя данные, указанные в **remoteItem** в следующем формате:</span><span class="sxs-lookup"><span data-stu-id="7f4c9-p103">Some driveItems returned from the **recent** action will include the **remoteItem** facet which indicates they are items from another drive. To access the original driveItem object, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

<!-- { "blockType": "ignored", "name": "drives-get-remoteitem" } -->

```http
GET /drives/{remoteItem-driveId}/items/{remoteItem-id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of recently used files for the owner of the drive.",
  "keywords": "drive,onedrive.drive,default drive",
  "section": "documentation",
  "tocPath": "Drives/Recent files",
  "suppressions": [
    "Error: /api-reference/v1.0/api/drive-recent.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/drive-recent.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-recent.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
