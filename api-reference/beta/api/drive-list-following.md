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
# <a name="list-followed-items"></a><span data-ttu-id="14d6c-102">Список отслеживаемых элементов</span><span class="sxs-lookup"><span data-stu-id="14d6c-102">List followed items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14d6c-103">Список [элементов](../resources/driveitem.md) , за которыми подписан пользователь, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="14d6c-103">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="14d6c-104">Эта коллекция содержит элементы, которые находятся на диске пользователя, а также элементы, к которым у него есть доступ с других дисков.</span><span class="sxs-lookup"><span data-stu-id="14d6c-104">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="14d6c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14d6c-105">Permissions</span></span>

<span data-ttu-id="14d6c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14d6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14d6c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14d6c-108">Permission type</span></span>      | <span data-ttu-id="14d6c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14d6c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14d6c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14d6c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="14d6c-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14d6c-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="14d6c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14d6c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14d6c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14d6c-113">Not supported.</span></span>    |
|<span data-ttu-id="14d6c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14d6c-114">Application</span></span> | <span data-ttu-id="14d6c-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14d6c-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14d6c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14d6c-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```

## <a name="response"></a><span data-ttu-id="14d6c-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="14d6c-117">Response</span></span>

<span data-ttu-id="14d6c-118">Этот метод возвращает коллекцию ресурсов [driveItem](../resources/driveitem.md) для элементов, которые подписаны владельцем диска.</span><span class="sxs-lookup"><span data-stu-id="14d6c-118">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="14d6c-119">Если не будет найдено ни одного элемента, то будет возвращена пустая коллекция.</span><span class="sxs-lookup"><span data-stu-id="14d6c-119">If no items were found, an empty collection is returned.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="14d6c-120">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="14d6c-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="14d6c-121">C#</span><span class="sxs-lookup"><span data-stu-id="14d6c-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-followed-items-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="14d6c-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="14d6c-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-followed-items-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="14d6c-123">Цель — C</span><span class="sxs-lookup"><span data-stu-id="14d6c-123">Objective-C</span></span>](#tab/objective-c)
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
