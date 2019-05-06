---
author: chackman
ms.author: chackman
title: Список отслеживаемых элементов
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1892b6c9adac3c41cf99bf755aa8d67d51a0066e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589780"
---
# <a name="list-followed-items"></a><span data-ttu-id="89ea6-102">Список отслеживаемых элементов</span><span class="sxs-lookup"><span data-stu-id="89ea6-102">List followed items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89ea6-103">Список [элементов](../resources/driveitem.md) , за которыми подписан пользователь, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="89ea6-103">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="89ea6-104">Эта коллекция содержит элементы, которые находятся на диске пользователя, а также элементы, к которым у него есть доступ с других дисков.</span><span class="sxs-lookup"><span data-stu-id="89ea6-104">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="89ea6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89ea6-105">Permissions</span></span>

<span data-ttu-id="89ea6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89ea6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89ea6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89ea6-108">Permission type</span></span>      | <span data-ttu-id="89ea6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89ea6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89ea6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89ea6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="89ea6-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89ea6-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="89ea6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89ea6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89ea6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89ea6-113">Not supported.</span></span>    |
|<span data-ttu-id="89ea6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89ea6-114">Application</span></span> | <span data-ttu-id="89ea6-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89ea6-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89ea6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89ea6-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```

## <a name="response"></a><span data-ttu-id="89ea6-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="89ea6-117">Response</span></span>

<span data-ttu-id="89ea6-118">Этот метод возвращает коллекцию ресурсов [driveItem](../resources/driveitem.md) для элементов, которые подписаны владельцем диска.</span><span class="sxs-lookup"><span data-stu-id="89ea6-118">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="89ea6-119">Если не будет найдено ни одного элемента, то будет возвращена пустая коллекция.</span><span class="sxs-lookup"><span data-stu-id="89ea6-119">If no items were found, an empty collection is returned.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="89ea6-120">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="89ea6-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="89ea6-121">Языках</span><span class="sxs-lookup"><span data-stu-id="89ea6-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-followed-items-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="89ea6-122">Язык</span><span class="sxs-lookup"><span data-stu-id="89ea6-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-followed-items-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/drive-list-following.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-list-following.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
