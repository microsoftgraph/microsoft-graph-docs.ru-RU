---
title: Тип ресурса Патчконтенткомманд
description: Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: cd7033ba271ba777d35f2469984662edbd7ffe53
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807183"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="c7e6a-103">Тип ресурса Патчконтенткомманд</span><span class="sxs-lookup"><span data-stu-id="c7e6a-103">patchContentCommand resource type</span></span>

<span data-ttu-id="c7e6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7e6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7e6a-105">Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.</span><span class="sxs-lookup"><span data-stu-id="c7e6a-105">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7e6a-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c7e6a-106">JSON representation</span></span>

<span data-ttu-id="c7e6a-107">Ниже показано представление ресурса в формате JSON, которое отправляется в теле запроса [Patch Pages/{ID} '](../api/page-update.md) .</span><span class="sxs-lookup"><span data-stu-id="c7e6a-107">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c7e6a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7e6a-108">Properties</span></span>
| <span data-ttu-id="c7e6a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7e6a-109">Property</span></span>     | <span data-ttu-id="c7e6a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c7e6a-110">Type</span></span>   |<span data-ttu-id="c7e6a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c7e6a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7e6a-112">action</span><span class="sxs-lookup"><span data-stu-id="c7e6a-112">action</span></span>|<span data-ttu-id="c7e6a-113">String</span><span class="sxs-lookup"><span data-stu-id="c7e6a-113">String</span></span>|<span data-ttu-id="c7e6a-114">Действие, которое необходимо выполнить для целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="c7e6a-114">The action to perform on the target element.</span></span> <span data-ttu-id="c7e6a-115">Возможные значения: `replace`, `append`, `delete`, `insert` и `prepend`.</span><span class="sxs-lookup"><span data-stu-id="c7e6a-115">Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="c7e6a-116">content</span><span class="sxs-lookup"><span data-stu-id="c7e6a-116">content</span></span>|<span data-ttu-id="c7e6a-117">String</span><span class="sxs-lookup"><span data-stu-id="c7e6a-117">String</span></span>|<span data-ttu-id="c7e6a-118">Строка правильно оформленного HTML-кода, который нужно добавить на страницу, а также двоичные данные изображения или файла.</span><span class="sxs-lookup"><span data-stu-id="c7e6a-118">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="c7e6a-119">Если содержимое содержит двоичные данные, необходимо отправить запрос, используя `multipart/form-data` тип контента с частью "Commands".</span><span class="sxs-lookup"><span data-stu-id="c7e6a-119">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="c7e6a-120">position</span><span class="sxs-lookup"><span data-stu-id="c7e6a-120">position</span></span>|<span data-ttu-id="c7e6a-121">String</span><span class="sxs-lookup"><span data-stu-id="c7e6a-121">String</span></span>|<span data-ttu-id="c7e6a-122">Место для добавления предоставленного контента относительно целевого элемента.</span><span class="sxs-lookup"><span data-stu-id="c7e6a-122">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="c7e6a-123">Возможные значения: `after` (по умолчанию) или `before` .</span><span class="sxs-lookup"><span data-stu-id="c7e6a-123">Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="c7e6a-124">target</span><span class="sxs-lookup"><span data-stu-id="c7e6a-124">target</span></span>|<span data-ttu-id="c7e6a-125">String</span><span class="sxs-lookup"><span data-stu-id="c7e6a-125">String</span></span>|<span data-ttu-id="c7e6a-126">Обновляемый элемент.</span><span class="sxs-lookup"><span data-stu-id="c7e6a-126">The element to update.</span></span> <span data-ttu-id="c7e6a-127">Должен быть `#<data-id>` либо сгенерированным `{id}` элементом, либо `body` `title` ключевым словом or.</span><span class="sxs-lookup"><span data-stu-id="c7e6a-127">Must be the `#<data-id>` or the generated `{id}` of the element, or the `body` or `title` keyword.</span></span>|

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
