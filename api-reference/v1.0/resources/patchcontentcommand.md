---
title: Тип ресурса patchContentCommand
description: Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.
localization_priority: Normal
ms.openlocfilehash: fb0900490b3fe05e6fb90dc4ab8252620bf43983
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804538"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="01b48-103">Тип ресурса patchContentCommand</span><span class="sxs-lookup"><span data-stu-id="01b48-103">patchContentCommand resource type</span></span>

<span data-ttu-id="01b48-104">Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.</span><span class="sxs-lookup"><span data-stu-id="01b48-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="01b48-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="01b48-105">JSON representation</span></span>

<span data-ttu-id="01b48-106">Ниже показано представление ресурса в формате JSON, которое отправляется в теле запроса [PATCH pages/{id}\`](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="01b48-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="01b48-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="01b48-107">Properties</span></span>
| <span data-ttu-id="01b48-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="01b48-108">Property</span></span>     | <span data-ttu-id="01b48-109">Тип</span><span class="sxs-lookup"><span data-stu-id="01b48-109">Type</span></span>   |<span data-ttu-id="01b48-110">Описание</span><span class="sxs-lookup"><span data-stu-id="01b48-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01b48-111">action</span><span class="sxs-lookup"><span data-stu-id="01b48-111">action</span></span>|<span data-ttu-id="01b48-112">onenotePatchActionType</span><span class="sxs-lookup"><span data-stu-id="01b48-112">onenotePatchActionType</span></span>|<span data-ttu-id="01b48-113">Действие, которое требуется выполнить с целевым элементом.</span><span class="sxs-lookup"><span data-stu-id="01b48-113">The action to perform on the target element.</span></span> <span data-ttu-id="01b48-114">Возможные значения: `replace`, `append`, `delete`, `insert`, или `prepend`.</span><span class="sxs-lookup"><span data-stu-id="01b48-114">The possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="01b48-115">content</span><span class="sxs-lookup"><span data-stu-id="01b48-115">content</span></span>|<span data-ttu-id="01b48-116">String</span><span class="sxs-lookup"><span data-stu-id="01b48-116">String</span></span>|<span data-ttu-id="01b48-p102">Строка правильно оформленного HTML-кода, который необходимо добавить на страницу, а также двоичные данные любого изображения или файла. Если контент содержит двоичные данные, необходимо отправить запрос с использованием типа контента `multipart/form-data` с частью Commands.</span><span class="sxs-lookup"><span data-stu-id="01b48-p102">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="01b48-119">position</span><span class="sxs-lookup"><span data-stu-id="01b48-119">position</span></span>|<span data-ttu-id="01b48-120">onenotePatchInsertPosition</span><span class="sxs-lookup"><span data-stu-id="01b48-120">onenotePatchInsertPosition</span></span>|<span data-ttu-id="01b48-121">Расположение относительно целевого элемента, куда нужно добавить указанное содержимое.</span><span class="sxs-lookup"><span data-stu-id="01b48-121">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="01b48-122">Возможные значения: `after` (по умолчанию) или `before`.</span><span class="sxs-lookup"><span data-stu-id="01b48-122">The possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="01b48-123">target</span><span class="sxs-lookup"><span data-stu-id="01b48-123">target</span></span>|<span data-ttu-id="01b48-124">Строка</span><span class="sxs-lookup"><span data-stu-id="01b48-124">String</span></span>|<span data-ttu-id="01b48-p104">Элемент для обновления. Значение этого свойства должно представлять собой `#<data-id>`, созданный идентификатор `<id>` элемента либо ключевое слово `body` или `title`.</span><span class="sxs-lookup"><span data-stu-id="01b48-p104">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
