---
title: Тип ресурса patchContentCommand
description: Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.
localization_priority: Normal
ms.openlocfilehash: 2e94f67a2a4e2e549d7367f0c48e31745d3bf659
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842730"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="4572d-103">Тип ресурса patchContentCommand</span><span class="sxs-lookup"><span data-stu-id="4572d-103">patchContentCommand resource type</span></span>

> <span data-ttu-id="4572d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4572d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4572d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4572d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4572d-106">Изменения, которые необходимо внести на страницу OneNote в запросе PATCH.</span><span class="sxs-lookup"><span data-stu-id="4572d-106">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4572d-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4572d-107">JSON representation</span></span>

<span data-ttu-id="4572d-108">Ниже показано представление ресурса в формате JSON, которое отправляется в теле запроса [PATCH pages/{id}\`](../api/page-update.md).</span><span class="sxs-lookup"><span data-stu-id="4572d-108">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="4572d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4572d-109">Properties</span></span>
| <span data-ttu-id="4572d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4572d-110">Property</span></span>     | <span data-ttu-id="4572d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4572d-111">Type</span></span>   |<span data-ttu-id="4572d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4572d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4572d-113">action</span><span class="sxs-lookup"><span data-stu-id="4572d-113">action</span></span>|<span data-ttu-id="4572d-114">String</span><span class="sxs-lookup"><span data-stu-id="4572d-114">String</span></span>|<span data-ttu-id="4572d-p102">Действие, которое необходимо выполнить над целевым элементом. Возможные значения: `replace`, `append`, `delete`, `insert` или `prepend`.</span><span class="sxs-lookup"><span data-stu-id="4572d-p102">The action to perform on the target element. Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="4572d-117">content</span><span class="sxs-lookup"><span data-stu-id="4572d-117">content</span></span>|<span data-ttu-id="4572d-118">String</span><span class="sxs-lookup"><span data-stu-id="4572d-118">String</span></span>|<span data-ttu-id="4572d-p103">Строка правильно оформленного HTML-кода, который необходимо добавить на страницу, а также двоичные данные любого изображения или файла. Если контент содержит двоичные данные, необходимо отправить запрос с использованием типа контента `multipart/form-data` с частью Commands.</span><span class="sxs-lookup"><span data-stu-id="4572d-p103">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="4572d-121">position</span><span class="sxs-lookup"><span data-stu-id="4572d-121">position</span></span>|<span data-ttu-id="4572d-122">String</span><span class="sxs-lookup"><span data-stu-id="4572d-122">String</span></span>|<span data-ttu-id="4572d-p104">Расположение относительно целевого элемента, куда необходимо добавить указанный контент. Возможные значения: `after` (используется по умолчанию) или `before`.</span><span class="sxs-lookup"><span data-stu-id="4572d-p104">The location to add the supplied content, relative to the target element. Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="4572d-125">target</span><span class="sxs-lookup"><span data-stu-id="4572d-125">target</span></span>|<span data-ttu-id="4572d-126">Строка</span><span class="sxs-lookup"><span data-stu-id="4572d-126">String</span></span>|<span data-ttu-id="4572d-p105">Элемент для обновления. Значение этого свойства должно представлять собой `#<data-id>`, созданный идентификатор `<id>` элемента либо ключевое слово `body` или `title`.</span><span class="sxs-lookup"><span data-stu-id="4572d-p105">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
