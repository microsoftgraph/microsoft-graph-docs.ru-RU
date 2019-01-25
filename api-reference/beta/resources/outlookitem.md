---
title: Тип ресурса outlookItem
description: Ниже представлено описание ресурса в формате JSON.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 8a44f9a2e568991c6803ebf72baf5f712f39ba64
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528293"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="27aab-103">Тип ресурса outlookItem</span><span class="sxs-lookup"><span data-stu-id="27aab-103">outlookItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="27aab-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27aab-104">JSON representation</span></span>

<span data-ttu-id="27aab-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="27aab-105">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="27aab-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="27aab-106">Properties</span></span>
| <span data-ttu-id="27aab-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="27aab-107">Property</span></span>     | <span data-ttu-id="27aab-108">Тип</span><span class="sxs-lookup"><span data-stu-id="27aab-108">Type</span></span>   |<span data-ttu-id="27aab-109">Описание</span><span class="sxs-lookup"><span data-stu-id="27aab-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27aab-110">categories</span><span class="sxs-lookup"><span data-stu-id="27aab-110">categories</span></span>|<span data-ttu-id="27aab-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="27aab-111">String collection</span></span>||
|<span data-ttu-id="27aab-112">changeKey</span><span class="sxs-lookup"><span data-stu-id="27aab-112">changeKey</span></span>|<span data-ttu-id="27aab-113">String</span><span class="sxs-lookup"><span data-stu-id="27aab-113">String</span></span>||
|<span data-ttu-id="27aab-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27aab-114">createdDateTime</span></span>|<span data-ttu-id="27aab-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27aab-115">DateTimeOffset</span></span>|<span data-ttu-id="27aab-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="27aab-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="27aab-118">id</span><span class="sxs-lookup"><span data-stu-id="27aab-118">id</span></span>|<span data-ttu-id="27aab-119">String</span><span class="sxs-lookup"><span data-stu-id="27aab-119">String</span></span>| <span data-ttu-id="27aab-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="27aab-120">Read-only.</span></span>|
|<span data-ttu-id="27aab-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27aab-121">lastModifiedDateTime</span></span>|<span data-ttu-id="27aab-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27aab-122">DateTimeOffset</span></span>|<span data-ttu-id="27aab-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="27aab-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="27aab-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="27aab-125">Relationships</span></span>
<span data-ttu-id="27aab-126">Нет</span><span class="sxs-lookup"><span data-stu-id="27aab-126">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlookitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
