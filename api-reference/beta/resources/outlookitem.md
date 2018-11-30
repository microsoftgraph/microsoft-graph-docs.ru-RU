---
title: Тип ресурса outlookItem
description: Ниже представлено описание ресурса в формате JSON.
ms.openlocfilehash: 6de0b5f9f79f8c3f813cbd876fa22f6b43f71a53
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081416"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="3f76a-103">Тип ресурса outlookItem</span><span class="sxs-lookup"><span data-stu-id="3f76a-103">outlookItem resource type</span></span>

> <span data-ttu-id="3f76a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3f76a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f76a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f76a-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f76a-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f76a-106">JSON representation</span></span>

<span data-ttu-id="3f76a-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="3f76a-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookitem"
}-->

```json
{
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="3f76a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f76a-108">Properties</span></span>
| <span data-ttu-id="3f76a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f76a-109">Property</span></span>     | <span data-ttu-id="3f76a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3f76a-110">Type</span></span>   |<span data-ttu-id="3f76a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3f76a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f76a-112">categories</span><span class="sxs-lookup"><span data-stu-id="3f76a-112">categories</span></span>|<span data-ttu-id="3f76a-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3f76a-113">String collection</span></span>||
|<span data-ttu-id="3f76a-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="3f76a-114">changeKey</span></span>|<span data-ttu-id="3f76a-115">String</span><span class="sxs-lookup"><span data-stu-id="3f76a-115">String</span></span>||
|<span data-ttu-id="3f76a-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f76a-116">createdDateTime</span></span>|<span data-ttu-id="3f76a-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f76a-117">DateTimeOffset</span></span>|<span data-ttu-id="3f76a-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3f76a-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3f76a-120">id</span><span class="sxs-lookup"><span data-stu-id="3f76a-120">id</span></span>|<span data-ttu-id="3f76a-121">String</span><span class="sxs-lookup"><span data-stu-id="3f76a-121">String</span></span>| <span data-ttu-id="3f76a-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f76a-122">Read-only.</span></span>|
|<span data-ttu-id="3f76a-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f76a-123">lastModifiedDateTime</span></span>|<span data-ttu-id="3f76a-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f76a-124">DateTimeOffset</span></span>|<span data-ttu-id="3f76a-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3f76a-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f76a-127">Связи</span><span class="sxs-lookup"><span data-stu-id="3f76a-127">Relationships</span></span>
<span data-ttu-id="3f76a-128">Нет</span><span class="sxs-lookup"><span data-stu-id="3f76a-128">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->