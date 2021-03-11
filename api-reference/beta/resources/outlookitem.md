---
title: Тип ресурса outlookItem
description: Ниже представлено описание ресурса в формате JSON.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9ed43ccabfbd2b5389525ebec02ecd04edb475b3
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721819"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="050cc-103">Тип ресурса outlookItem</span><span class="sxs-lookup"><span data-stu-id="050cc-103">outlookItem resource type</span></span>

<span data-ttu-id="050cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="050cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="050cc-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="050cc-105">JSON representation</span></span>

<span data-ttu-id="050cc-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="050cc-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="050cc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="050cc-107">Properties</span></span>
| <span data-ttu-id="050cc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="050cc-108">Property</span></span>     | <span data-ttu-id="050cc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="050cc-109">Type</span></span>   |<span data-ttu-id="050cc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="050cc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="050cc-111">categories</span><span class="sxs-lookup"><span data-stu-id="050cc-111">categories</span></span>|<span data-ttu-id="050cc-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="050cc-112">String collection</span></span>||
|<span data-ttu-id="050cc-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="050cc-113">changeKey</span></span>|<span data-ttu-id="050cc-114">String</span><span class="sxs-lookup"><span data-stu-id="050cc-114">String</span></span>||
|<span data-ttu-id="050cc-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="050cc-115">createdDateTime</span></span>|<span data-ttu-id="050cc-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="050cc-116">DateTimeOffset</span></span>|<span data-ttu-id="050cc-117">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="050cc-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="050cc-118">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="050cc-118">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="050cc-119">id</span><span class="sxs-lookup"><span data-stu-id="050cc-119">id</span></span>|<span data-ttu-id="050cc-120">String</span><span class="sxs-lookup"><span data-stu-id="050cc-120">String</span></span>| <span data-ttu-id="050cc-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="050cc-121">Read-only.</span></span>|
|<span data-ttu-id="050cc-122">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="050cc-122">lastModifiedDateTime</span></span>|<span data-ttu-id="050cc-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="050cc-123">DateTimeOffset</span></span>|<span data-ttu-id="050cc-124">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="050cc-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="050cc-125">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="050cc-125">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="050cc-126">Связи</span><span class="sxs-lookup"><span data-stu-id="050cc-126">Relationships</span></span>
<span data-ttu-id="050cc-127">Нет</span><span class="sxs-lookup"><span data-stu-id="050cc-127">None</span></span>


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


