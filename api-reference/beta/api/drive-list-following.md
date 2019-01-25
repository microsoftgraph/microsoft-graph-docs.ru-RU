---
author: chackman
ms.author: chackman
title: Число элементов списка
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: df38a11a09f4ec86eb029f236030cc4565e5d939
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523311"
---
# <a name="list-followed-items"></a><span data-ttu-id="9acce-102">Число элементов списка</span><span class="sxs-lookup"><span data-stu-id="9acce-102">List followed items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9acce-103">Список [элементов](../resources/driveitem.md) , следуют выполнен вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="9acce-103">List the [items](../resources/driveitem.md) that have been followed by the signed in user.</span></span>
<span data-ttu-id="9acce-104">Данная коллекция включает элементов, находящихся в диске компьютера пользователя, а также элементы, которые получают доступ из других дисков.</span><span class="sxs-lookup"><span data-stu-id="9acce-104">This collection includes items that are in the user's drive as well as items they have access to from other drives.</span></span>

## <a name="permissions"></a><span data-ttu-id="9acce-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9acce-105">Permissions</span></span>

<span data-ttu-id="9acce-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9acce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9acce-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9acce-108">Permission type</span></span>      | <span data-ttu-id="9acce-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9acce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9acce-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9acce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9acce-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9acce-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9acce-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9acce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9acce-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9acce-113">Not supported.</span></span>    |
|<span data-ttu-id="9acce-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9acce-114">Application</span></span> | <span data-ttu-id="9acce-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9acce-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9acce-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9acce-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-followed-items", "scopes": "files.read" } -->

```http
GET /me/drive/following
```

## <a name="response"></a><span data-ttu-id="9acce-117">Ответ</span><span class="sxs-lookup"><span data-stu-id="9acce-117">Response</span></span>

<span data-ttu-id="9acce-118">Этот метод возвращает коллекцию ресурсов [driveItem](../resources/driveitem.md) для элементов, которые выполнив владельца диска.</span><span class="sxs-lookup"><span data-stu-id="9acce-118">This method returns a collection of [driveItem](../resources/driveitem.md) resources for items which the owner of the drive is following.</span></span>
<span data-ttu-id="9acce-119">Если не найдено элементов, возвращается пустая коллекция.</span><span class="sxs-lookup"><span data-stu-id="9acce-119">If no items were found, an empty collection is returned.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "List the items a user is following.",
  "keywords": "drive,onedrive.drive,list followed items",
  "section": "documentation",
  "tocPath": "Drives/List followed items",
  "suppressions": [
    "Error: /api-reference/beta/api/drive-list-following.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
