---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Восстановление предыдущей версии элемента списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 20cf0460aa679fc40a4bb11d0887bc4946ddcd74
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482086"
---
# <a name="restore-a-previous-version-of-a-listitem"></a><span data-ttu-id="f3152-102">Восстановление предыдущей версии ресурса ListItem</span><span class="sxs-lookup"><span data-stu-id="f3152-102">Restore a previous version of a ListItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3152-103">Восстановление предыдущей версии ресурса ListItem в качестве текущей версии.</span><span class="sxs-lookup"><span data-stu-id="f3152-103">Restore a previous version of a ListItem to be the current version.</span></span> <span data-ttu-id="f3152-104">При этом будет создана новая версия с тем же содержимым, что и в предыдущей версии, но будут сохранены все существующие версии элемента.</span><span class="sxs-lookup"><span data-stu-id="f3152-104">This will create a new version with the contents of the previous version, but preserves all existing versions of the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3152-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f3152-105">Permissions</span></span>

<span data-ttu-id="f3152-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3152-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="f3152-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3152-108">Permission type</span></span>             |         <span data-ttu-id="f3152-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3152-109">Permissions (from least to most privileged)</span></span>          |
| :------------------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="f3152-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3152-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f3152-111">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="f3152-111">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |
| <span data-ttu-id="f3152-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3152-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3152-113">Н/д</span><span class="sxs-lookup"><span data-stu-id="f3152-113">n/a</span></span>                                                          |
| <span data-ttu-id="f3152-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3152-114">Application</span></span>                            | <span data-ttu-id="f3152-115">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="f3152-115">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3152-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3152-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
POST /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

### <a name="request-body"></a><span data-ttu-id="f3152-117">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3152-117">Request body</span></span>

<span data-ttu-id="f3152-118">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="f3152-118">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="f3152-119">Пример</span><span class="sxs-lookup"><span data-stu-id="f3152-119">Example</span></span>

<span data-ttu-id="f3152-120">В этом примере восстанавливается версия ресурса listItem, указанная пр `{item-id}` и `{version-id}`.</span><span class="sxs-lookup"><span data-stu-id="f3152-120">This example restores a version of a listItem identified by `{item-id}` and `{version-id}`.</span></span>

<!-- { "blockType": "request", "name": "restore-item-version-listItem", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restoreVersion
```

## <a name="response"></a><span data-ttu-id="f3152-121">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3152-121">Response</span></span>

<span data-ttu-id="f3152-122">При успешном выполнении вызова API возвращается отклик `204 No content`.</span><span class="sxs-lookup"><span data-stu-id="f3152-122">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy",
  "suppressions": [
    "Error: /api-reference/beta/api/listitemversion-restore.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
