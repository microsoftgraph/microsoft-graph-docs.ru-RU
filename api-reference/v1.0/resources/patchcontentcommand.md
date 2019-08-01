---
title: Тип ресурса Патчконтенткомманд
description: Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fb6ea7d5ba18e91685de3a883f7060d0fa83b729
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035576"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="5585f-103">Тип ресурса Патчконтенткомманд</span><span class="sxs-lookup"><span data-stu-id="5585f-103">patchContentCommand resource type</span></span>

<span data-ttu-id="5585f-104">Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.</span><span class="sxs-lookup"><span data-stu-id="5585f-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5585f-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5585f-105">JSON representation</span></span>

<span data-ttu-id="5585f-106">Ниже показано представление ресурса в формате JSON, которое отправляется в теле запроса [Patch Pages/{ID} '](../api/page-update.md) .</span><span class="sxs-lookup"><span data-stu-id="5585f-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="5585f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5585f-107">Properties</span></span>
| <span data-ttu-id="5585f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5585f-108">Property</span></span>     | <span data-ttu-id="5585f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5585f-109">Type</span></span>   |<span data-ttu-id="5585f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5585f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5585f-111">action</span><span class="sxs-lookup"><span data-stu-id="5585f-111">action</span></span>|<span data-ttu-id="5585f-112">Оненотепатчактионтипе</span><span class="sxs-lookup"><span data-stu-id="5585f-112">onenotePatchActionType</span></span>|<span data-ttu-id="5585f-113">Действие, которое необходимо выполнить для целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="5585f-113">The action to perform on the target element.</span></span> <span data-ttu-id="5585f-114">Возможные значения: `replace`, `append`, `delete`, `insert`, или. `prepend`</span><span class="sxs-lookup"><span data-stu-id="5585f-114">The possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="5585f-115">content</span><span class="sxs-lookup"><span data-stu-id="5585f-115">content</span></span>|<span data-ttu-id="5585f-116">String</span><span class="sxs-lookup"><span data-stu-id="5585f-116">String</span></span>|<span data-ttu-id="5585f-117">Строка правильно оформленного HTML-кода, который нужно добавить на страницу, а также двоичные данные изображения или файла.</span><span class="sxs-lookup"><span data-stu-id="5585f-117">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="5585f-118">Если содержимое содержит двоичные данные, необходимо отправить запрос, используя тип `multipart/form-data` контента с частью "Commands".</span><span class="sxs-lookup"><span data-stu-id="5585f-118">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="5585f-119">position</span><span class="sxs-lookup"><span data-stu-id="5585f-119">position</span></span>|<span data-ttu-id="5585f-120">Оненотепатчинсертпоситион</span><span class="sxs-lookup"><span data-stu-id="5585f-120">onenotePatchInsertPosition</span></span>|<span data-ttu-id="5585f-121">Место для добавления предоставленного контента относительно целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="5585f-121">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="5585f-122">Возможные значения: `after` (по умолчанию) или `before`.</span><span class="sxs-lookup"><span data-stu-id="5585f-122">The possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="5585f-123">target</span><span class="sxs-lookup"><span data-stu-id="5585f-123">target</span></span>|<span data-ttu-id="5585f-124">String</span><span class="sxs-lookup"><span data-stu-id="5585f-124">String</span></span>|<span data-ttu-id="5585f-125">Обновляемый элемент.</span><span class="sxs-lookup"><span data-stu-id="5585f-125">The element to update.</span></span> <span data-ttu-id="5585f-126">Должен быть `#<data-id>` либо сгенерированным `<id>` элементом, либо ключевым словом `body` or. `title`</span><span class="sxs-lookup"><span data-stu-id="5585f-126">Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
