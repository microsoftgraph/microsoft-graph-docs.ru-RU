---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Создание записи в списке SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1af6162fd12c9c3dfc470b97e42a25d0cad8ebea
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482415"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="6b4b8-102">Создание элемента в списке</span><span class="sxs-lookup"><span data-stu-id="6b4b8-102">Create a new item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b4b8-103">Создание элемента [listItem][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="6b4b8-103">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="6b4b8-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b4b8-104">Permissions</span></span>

<span data-ttu-id="6b4b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b4b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b4b8-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b4b8-107">Permission type</span></span>      | <span data-ttu-id="6b4b8-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b4b8-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b4b8-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b4b8-109">Delegated (work or school account)</span></span> | <span data-ttu-id="6b4b8-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b4b8-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6b4b8-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b4b8-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b4b8-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b4b8-112">Not supported.</span></span>    |
|<span data-ttu-id="6b4b8-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b4b8-113">Application</span></span> | <span data-ttu-id="6b4b8-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b4b8-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b4b8-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b4b8-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="6b4b8-116">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6b4b8-116">Request body</span></span>

<span data-ttu-id="6b4b8-117">В теле запроса укажите представление ресурса [listItem][], который необходимо создать, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b4b8-117">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="6b4b8-118">Пример</span><span class="sxs-lookup"><span data-stu-id="6b4b8-118">Example</span></span>

<span data-ttu-id="6b4b8-119">В примере ниже показано, как создать элемент списка общего назначения.</span><span class="sxs-lookup"><span data-stu-id="6b4b8-119">Here is an example of how to create a new generic list item.</span></span>

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
POST https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
Content-Type: application/json

{
  "fields": {
    "Title": "Widget",
    "Color": "Purple",
    "Weight": 32
  }
}
```

## <a name="response"></a><span data-ttu-id="6b4b8-120">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b4b8-120">Response</span></span>

<span data-ttu-id="6b4b8-121">При успешном выполнении этот метод возвращает объект [listItem][] для созданного элемента списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6b4b8-121">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "20",
  "createdDateTime": "2016-08-30T08:26:00Z",
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  },
  "lastModifiedDateTime": "2016-08-30T08:26:00Z",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  }
}
```

<span data-ttu-id="6b4b8-122">**Примечание.** Ответ усечен для наглядности.</span><span class="sxs-lookup"><span data-stu-id="6b4b8-122">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="6b4b8-123">При фактическом вызове будут возвращены свойства, используемые по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6b4b8-123">Default properties will be returned from the actual call.</span></span>

[списке]: ../resources/list.md
[list]: ../resources/list.md
[listItem]: ../resources/listitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Add a new item to a SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Create",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
