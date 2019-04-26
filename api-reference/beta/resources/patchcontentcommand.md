---
title: Тип ресурса Патчконтенткомманд
description: Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.
localization_priority: Normal
ms.openlocfilehash: d0d8f320d22a8b3466ddd53deee5bcb7955ff3d1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568481"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="831e5-103">Тип ресурса Патчконтенткомманд</span><span class="sxs-lookup"><span data-stu-id="831e5-103">patchContentCommand resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="831e5-104">Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.</span><span class="sxs-lookup"><span data-stu-id="831e5-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="831e5-105">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="831e5-105">JSON representation</span></span>

<span data-ttu-id="831e5-106">Ниже показано представление ресурса в формате JSON, которое отправляется в теле запроса [Patch Pages/{ID} '](../api/page-update.md) .</span><span class="sxs-lookup"><span data-stu-id="831e5-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="831e5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="831e5-107">Properties</span></span>
| <span data-ttu-id="831e5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="831e5-108">Property</span></span>     | <span data-ttu-id="831e5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="831e5-109">Type</span></span>   |<span data-ttu-id="831e5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="831e5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="831e5-111">action</span><span class="sxs-lookup"><span data-stu-id="831e5-111">action</span></span>|<span data-ttu-id="831e5-112">String</span><span class="sxs-lookup"><span data-stu-id="831e5-112">String</span></span>|<span data-ttu-id="831e5-113">Действие, которое необходимо выполнить для целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="831e5-113">The action to perform on the target element.</span></span> <span data-ttu-id="831e5-114">Возможные значения: `replace`, `append`, `delete`, `insert` и `prepend`.</span><span class="sxs-lookup"><span data-stu-id="831e5-114">Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="831e5-115">content</span><span class="sxs-lookup"><span data-stu-id="831e5-115">content</span></span>|<span data-ttu-id="831e5-116">String</span><span class="sxs-lookup"><span data-stu-id="831e5-116">String</span></span>|<span data-ttu-id="831e5-117">Строка правильно оформленного HTML-кода, который нужно добавить на страницу, а также двоичные данные изображения или файла.</span><span class="sxs-lookup"><span data-stu-id="831e5-117">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="831e5-118">Если содержимое содержит двоичные данные, необходимо отправить запрос, используя тип `multipart/form-data` контента с частью "Commands".</span><span class="sxs-lookup"><span data-stu-id="831e5-118">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="831e5-119">position</span><span class="sxs-lookup"><span data-stu-id="831e5-119">position</span></span>|<span data-ttu-id="831e5-120">String</span><span class="sxs-lookup"><span data-stu-id="831e5-120">String</span></span>|<span data-ttu-id="831e5-121">Место для добавления предоставленного контента относительно целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="831e5-121">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="831e5-122">Возможные значения: `after` (по умолчанию) `before`или.</span><span class="sxs-lookup"><span data-stu-id="831e5-122">Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="831e5-123">target</span><span class="sxs-lookup"><span data-stu-id="831e5-123">target</span></span>|<span data-ttu-id="831e5-124">String</span><span class="sxs-lookup"><span data-stu-id="831e5-124">String</span></span>|<span data-ttu-id="831e5-125">Обновляемый элемент.</span><span class="sxs-lookup"><span data-stu-id="831e5-125">The element to update.</span></span> <span data-ttu-id="831e5-126">Должен быть `#<data-id>` либо сгенерированным `<id>` элементом, либо ключевым словом `body` or. `title`</span><span class="sxs-lookup"><span data-stu-id="831e5-126">Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

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
