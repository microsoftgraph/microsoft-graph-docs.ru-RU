---
title: Тип ресурса outlookItem
description: Ниже представлено описание ресурса в формате JSON.
author: angelgolfer-ms
ms.openlocfilehash: 4d375606a5104d48955561df3b904922a5daf042
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315024"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="8e007-103">Тип ресурса outlookItem</span><span class="sxs-lookup"><span data-stu-id="8e007-103">outlookItem resource type</span></span>

> <span data-ttu-id="8e007-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8e007-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e007-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e007-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e007-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e007-106">JSON representation</span></span>

<span data-ttu-id="8e007-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="8e007-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="8e007-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e007-108">Properties</span></span>
| <span data-ttu-id="8e007-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e007-109">Property</span></span>     | <span data-ttu-id="8e007-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8e007-110">Type</span></span>   |<span data-ttu-id="8e007-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8e007-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e007-112">categories</span><span class="sxs-lookup"><span data-stu-id="8e007-112">categories</span></span>|<span data-ttu-id="8e007-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8e007-113">String collection</span></span>||
|<span data-ttu-id="8e007-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="8e007-114">changeKey</span></span>|<span data-ttu-id="8e007-115">String</span><span class="sxs-lookup"><span data-stu-id="8e007-115">String</span></span>||
|<span data-ttu-id="8e007-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e007-116">createdDateTime</span></span>|<span data-ttu-id="8e007-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e007-117">DateTimeOffset</span></span>|<span data-ttu-id="8e007-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8e007-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8e007-120">id</span><span class="sxs-lookup"><span data-stu-id="8e007-120">id</span></span>|<span data-ttu-id="8e007-121">Строка</span><span class="sxs-lookup"><span data-stu-id="8e007-121">String</span></span>| <span data-ttu-id="8e007-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e007-122">Read-only.</span></span>|
|<span data-ttu-id="8e007-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e007-123">lastModifiedDateTime</span></span>|<span data-ttu-id="8e007-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e007-124">DateTimeOffset</span></span>|<span data-ttu-id="8e007-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8e007-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e007-127">Связи</span><span class="sxs-lookup"><span data-stu-id="8e007-127">Relationships</span></span>
<span data-ttu-id="8e007-128">Нет</span><span class="sxs-lookup"><span data-stu-id="8e007-128">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->