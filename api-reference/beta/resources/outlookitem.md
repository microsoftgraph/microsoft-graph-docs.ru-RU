---
title: Тип ресурса outlookItem
description: Ниже показано представление JSON ресурса.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 8a44f9a2e568991c6803ebf72baf5f712f39ba64
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568656"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="8c942-103">Тип ресурса outlookItem</span><span class="sxs-lookup"><span data-stu-id="8c942-103">outlookItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="8c942-104">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8c942-104">JSON representation</span></span>

<span data-ttu-id="8c942-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="8c942-105">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="8c942-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c942-106">Properties</span></span>
| <span data-ttu-id="8c942-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c942-107">Property</span></span>     | <span data-ttu-id="8c942-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8c942-108">Type</span></span>   |<span data-ttu-id="8c942-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8c942-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c942-110">categories</span><span class="sxs-lookup"><span data-stu-id="8c942-110">categories</span></span>|<span data-ttu-id="8c942-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8c942-111">String collection</span></span>||
|<span data-ttu-id="8c942-112">changeKey</span><span class="sxs-lookup"><span data-stu-id="8c942-112">changeKey</span></span>|<span data-ttu-id="8c942-113">String</span><span class="sxs-lookup"><span data-stu-id="8c942-113">String</span></span>||
|<span data-ttu-id="8c942-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c942-114">createdDateTime</span></span>|<span data-ttu-id="8c942-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c942-115">DateTimeOffset</span></span>|<span data-ttu-id="8c942-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8c942-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8c942-118">id</span><span class="sxs-lookup"><span data-stu-id="8c942-118">id</span></span>|<span data-ttu-id="8c942-119">String</span><span class="sxs-lookup"><span data-stu-id="8c942-119">String</span></span>| <span data-ttu-id="8c942-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8c942-120">Read-only.</span></span>|
|<span data-ttu-id="8c942-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c942-121">lastModifiedDateTime</span></span>|<span data-ttu-id="8c942-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c942-122">DateTimeOffset</span></span>|<span data-ttu-id="8c942-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8c942-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c942-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="8c942-125">Relationships</span></span>
<span data-ttu-id="8c942-126">Нет</span><span class="sxs-lookup"><span data-stu-id="8c942-126">None</span></span>


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
