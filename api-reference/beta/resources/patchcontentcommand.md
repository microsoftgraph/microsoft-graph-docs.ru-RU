---
title: Тип ресурса patchContentCommand
description: Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.
localization_priority: Normal
ms.openlocfilehash: d0d8f320d22a8b3466ddd53deee5bcb7955ff3d1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523885"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="a530f-103">Тип ресурса patchContentCommand</span><span class="sxs-lookup"><span data-stu-id="a530f-103">patchContentCommand resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a530f-104">Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.</span><span class="sxs-lookup"><span data-stu-id="a530f-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a530f-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a530f-105">JSON representation</span></span>

<span data-ttu-id="a530f-106">Ниже показано представление ресурса в формате JSON, которое отправляется в теле запроса [PATCH pages/{id}\`](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="a530f-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}-->

```json
{
  "action": "String",
  "content": "string",
  "position": "String",
  "target": "string"
}

```

## <a name="properties"></a><span data-ttu-id="a530f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a530f-107">Properties</span></span>
| <span data-ttu-id="a530f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a530f-108">Property</span></span>     | <span data-ttu-id="a530f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a530f-109">Type</span></span>   |<span data-ttu-id="a530f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a530f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a530f-111">action</span><span class="sxs-lookup"><span data-stu-id="a530f-111">action</span></span>|<span data-ttu-id="a530f-112">String</span><span class="sxs-lookup"><span data-stu-id="a530f-112">String</span></span>|<span data-ttu-id="a530f-p101">Действие, которое необходимо выполнить над целевым элементом. Возможные значения: `replace`, `append`, `delete`, `insert` или `prepend`.</span><span class="sxs-lookup"><span data-stu-id="a530f-p101">The action to perform on the target element. Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="a530f-115">content</span><span class="sxs-lookup"><span data-stu-id="a530f-115">content</span></span>|<span data-ttu-id="a530f-116">String</span><span class="sxs-lookup"><span data-stu-id="a530f-116">String</span></span>|<span data-ttu-id="a530f-p102">Строка правильно оформленного HTML-кода, который необходимо добавить на страницу, а также двоичные данные любого изображения или файла. Если контент содержит двоичные данные, необходимо отправить запрос с использованием типа контента `multipart/form-data` с частью Commands.</span><span class="sxs-lookup"><span data-stu-id="a530f-p102">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="a530f-119">position</span><span class="sxs-lookup"><span data-stu-id="a530f-119">position</span></span>|<span data-ttu-id="a530f-120">String</span><span class="sxs-lookup"><span data-stu-id="a530f-120">String</span></span>|<span data-ttu-id="a530f-p103">Расположение относительно целевого элемента, куда необходимо добавить указанный контент. Возможные значения: `after` (используется по умолчанию) или `before`.</span><span class="sxs-lookup"><span data-stu-id="a530f-p103">The location to add the supplied content, relative to the target element. Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="a530f-123">target</span><span class="sxs-lookup"><span data-stu-id="a530f-123">target</span></span>|<span data-ttu-id="a530f-124">String</span><span class="sxs-lookup"><span data-stu-id="a530f-124">String</span></span>|<span data-ttu-id="a530f-p104">Элемент для обновления. Значение этого свойства должно представлять собой `#<data-id>`, созданный идентификатор `<id>` элемента либо ключевое слово `body` или `title`.</span><span class="sxs-lookup"><span data-stu-id="a530f-p104">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/patchcontentcommand.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
