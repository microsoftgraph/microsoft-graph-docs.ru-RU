---
title: Тип ресурса outlookItem
description: Ниже этот ресурс представлен в формате JSON.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 77741fa05f356418e688cdc4a45c5a4750604c3c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009281"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="c0671-103">Тип ресурса outlookItem</span><span class="sxs-lookup"><span data-stu-id="c0671-103">outlookItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="c0671-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0671-104">JSON representation</span></span>

<span data-ttu-id="c0671-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="c0671-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookItem"
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
## <a name="properties"></a><span data-ttu-id="c0671-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0671-106">Properties</span></span>
| <span data-ttu-id="c0671-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0671-107">Property</span></span>     | <span data-ttu-id="c0671-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c0671-108">Type</span></span>   |<span data-ttu-id="c0671-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c0671-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0671-110">categories</span><span class="sxs-lookup"><span data-stu-id="c0671-110">categories</span></span>|<span data-ttu-id="c0671-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c0671-111">String collection</span></span>||
|<span data-ttu-id="c0671-112">changeKey</span><span class="sxs-lookup"><span data-stu-id="c0671-112">changeKey</span></span>|<span data-ttu-id="c0671-113">String</span><span class="sxs-lookup"><span data-stu-id="c0671-113">String</span></span>||
|<span data-ttu-id="c0671-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c0671-114">createdDateTime</span></span>|<span data-ttu-id="c0671-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0671-115">DateTimeOffset</span></span>|<span data-ttu-id="c0671-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c0671-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c0671-118">id</span><span class="sxs-lookup"><span data-stu-id="c0671-118">id</span></span>|<span data-ttu-id="c0671-119">String</span><span class="sxs-lookup"><span data-stu-id="c0671-119">String</span></span>| <span data-ttu-id="c0671-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c0671-120">Read-only.</span></span>|
|<span data-ttu-id="c0671-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c0671-121">lastModifiedDateTime</span></span>|<span data-ttu-id="c0671-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0671-122">DateTimeOffset</span></span>|<span data-ttu-id="c0671-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c0671-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0671-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="c0671-125">Relationships</span></span>
<span data-ttu-id="c0671-126">Нет</span><span class="sxs-lookup"><span data-stu-id="c0671-126">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
