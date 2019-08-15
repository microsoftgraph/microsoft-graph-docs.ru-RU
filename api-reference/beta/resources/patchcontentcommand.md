---
title: Тип ресурса Патчконтенткомманд
description: Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4cfa6fe84c18d4895e5d709d3ab6254258c1b970
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422284"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="eea31-103">Тип ресурса Патчконтенткомманд</span><span class="sxs-lookup"><span data-stu-id="eea31-103">patchContentCommand resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eea31-104">Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.</span><span class="sxs-lookup"><span data-stu-id="eea31-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eea31-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eea31-105">JSON representation</span></span>

<span data-ttu-id="eea31-106">Ниже показано представление ресурса в формате JSON, которое отправляется в теле запроса [Patch Pages/{ID} '](../api/page-update.md) .</span><span class="sxs-lookup"><span data-stu-id="eea31-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="eea31-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="eea31-107">Properties</span></span>
| <span data-ttu-id="eea31-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="eea31-108">Property</span></span>     | <span data-ttu-id="eea31-109">Тип</span><span class="sxs-lookup"><span data-stu-id="eea31-109">Type</span></span>   |<span data-ttu-id="eea31-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eea31-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eea31-111">action</span><span class="sxs-lookup"><span data-stu-id="eea31-111">action</span></span>|<span data-ttu-id="eea31-112">String</span><span class="sxs-lookup"><span data-stu-id="eea31-112">String</span></span>|<span data-ttu-id="eea31-113">Действие, которое необходимо выполнить для целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="eea31-113">The action to perform on the target element.</span></span> <span data-ttu-id="eea31-114">Возможные значения: `replace`, `append`, `delete`, `insert` и `prepend`.</span><span class="sxs-lookup"><span data-stu-id="eea31-114">Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="eea31-115">content</span><span class="sxs-lookup"><span data-stu-id="eea31-115">content</span></span>|<span data-ttu-id="eea31-116">String</span><span class="sxs-lookup"><span data-stu-id="eea31-116">String</span></span>|<span data-ttu-id="eea31-117">Строка правильно оформленного HTML-кода, который нужно добавить на страницу, а также двоичные данные изображения или файла.</span><span class="sxs-lookup"><span data-stu-id="eea31-117">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="eea31-118">Если содержимое содержит двоичные данные, необходимо отправить запрос, используя тип `multipart/form-data` контента с частью "Commands".</span><span class="sxs-lookup"><span data-stu-id="eea31-118">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="eea31-119">position</span><span class="sxs-lookup"><span data-stu-id="eea31-119">position</span></span>|<span data-ttu-id="eea31-120">String</span><span class="sxs-lookup"><span data-stu-id="eea31-120">String</span></span>|<span data-ttu-id="eea31-121">Место для добавления предоставленного контента относительно целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="eea31-121">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="eea31-122">Возможные значения: `after` (по умолчанию) `before`или.</span><span class="sxs-lookup"><span data-stu-id="eea31-122">Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="eea31-123">target</span><span class="sxs-lookup"><span data-stu-id="eea31-123">target</span></span>|<span data-ttu-id="eea31-124">String</span><span class="sxs-lookup"><span data-stu-id="eea31-124">String</span></span>|<span data-ttu-id="eea31-125">Обновляемый элемент.</span><span class="sxs-lookup"><span data-stu-id="eea31-125">The element to update.</span></span> <span data-ttu-id="eea31-126">Должен быть `#<data-id>` либо сгенерированным `{id}` элементом, либо ключевым словом `body` or. `title`</span><span class="sxs-lookup"><span data-stu-id="eea31-126">Must be the `#<data-id>` or the generated `{id}` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
