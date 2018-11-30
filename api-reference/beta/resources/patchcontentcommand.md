---
title: Тип ресурса patchContentCommand
description: Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.
ms.openlocfilehash: fb559a96aa5eef94dd07280b888da0df989b2363
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081607"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="cde86-103">Тип ресурса patchContentCommand</span><span class="sxs-lookup"><span data-stu-id="cde86-103">patchContentCommand resource type</span></span>

> <span data-ttu-id="cde86-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cde86-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cde86-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cde86-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cde86-106">Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.</span><span class="sxs-lookup"><span data-stu-id="cde86-106">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cde86-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cde86-107">JSON representation</span></span>

<span data-ttu-id="cde86-108">Ниже показано представление ресурса в формате JSON, которое отправляется в теле запроса [PATCH pages/{id}\`](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="cde86-108">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="cde86-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="cde86-109">Properties</span></span>
| <span data-ttu-id="cde86-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="cde86-110">Property</span></span>     | <span data-ttu-id="cde86-111">Тип</span><span class="sxs-lookup"><span data-stu-id="cde86-111">Type</span></span>   |<span data-ttu-id="cde86-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cde86-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cde86-113">action</span><span class="sxs-lookup"><span data-stu-id="cde86-113">action</span></span>|<span data-ttu-id="cde86-114">String</span><span class="sxs-lookup"><span data-stu-id="cde86-114">String</span></span>|<span data-ttu-id="cde86-p102">Действие, которое необходимо выполнить над целевым элементом. Возможные значения: `replace`, `append`, `delete`, `insert` или `prepend`.</span><span class="sxs-lookup"><span data-stu-id="cde86-p102">The action to perform on the target element. Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="cde86-117">content</span><span class="sxs-lookup"><span data-stu-id="cde86-117">content</span></span>|<span data-ttu-id="cde86-118">String</span><span class="sxs-lookup"><span data-stu-id="cde86-118">String</span></span>|<span data-ttu-id="cde86-p103">Строка правильно оформленного HTML-кода, который необходимо добавить на страницу, а также двоичные данные любого изображения или файла. Если контент содержит двоичные данные, необходимо отправить запрос с использованием типа контента `multipart/form-data` с частью Commands.</span><span class="sxs-lookup"><span data-stu-id="cde86-p103">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="cde86-121">position</span><span class="sxs-lookup"><span data-stu-id="cde86-121">position</span></span>|<span data-ttu-id="cde86-122">String</span><span class="sxs-lookup"><span data-stu-id="cde86-122">String</span></span>|<span data-ttu-id="cde86-p104">Расположение относительно целевого элемента, куда необходимо добавить указанный контент. Возможные значения: `after` (используется по умолчанию) или `before`.</span><span class="sxs-lookup"><span data-stu-id="cde86-p104">The location to add the supplied content, relative to the target element. Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="cde86-125">target</span><span class="sxs-lookup"><span data-stu-id="cde86-125">target</span></span>|<span data-ttu-id="cde86-126">String</span><span class="sxs-lookup"><span data-stu-id="cde86-126">String</span></span>|<span data-ttu-id="cde86-p105">Элемент для обновления. Значение этого свойства должно представлять собой `#<data-id>`, созданный идентификатор `<id>` элемента либо ключевое слово `body` или `title`.</span><span class="sxs-lookup"><span data-stu-id="cde86-p105">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->