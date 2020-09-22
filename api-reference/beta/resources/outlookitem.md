---
title: Тип ресурса outlookItem
description: Ниже этот ресурс представлен в формате JSON.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0d0303e3a80e0231487701d66076ef8fa52be358
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998380"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="a4ef5-103">Тип ресурса outlookItem</span><span class="sxs-lookup"><span data-stu-id="a4ef5-103">outlookItem resource type</span></span>

<span data-ttu-id="a4ef5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4ef5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="a4ef5-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a4ef5-105">JSON representation</span></span>

<span data-ttu-id="a4ef5-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="a4ef5-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="a4ef5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4ef5-107">Properties</span></span>
| <span data-ttu-id="a4ef5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4ef5-108">Property</span></span>     | <span data-ttu-id="a4ef5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a4ef5-109">Type</span></span>   |<span data-ttu-id="a4ef5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a4ef5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4ef5-111">categories</span><span class="sxs-lookup"><span data-stu-id="a4ef5-111">categories</span></span>|<span data-ttu-id="a4ef5-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a4ef5-112">String collection</span></span>||
|<span data-ttu-id="a4ef5-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="a4ef5-113">changeKey</span></span>|<span data-ttu-id="a4ef5-114">String</span><span class="sxs-lookup"><span data-stu-id="a4ef5-114">String</span></span>||
|<span data-ttu-id="a4ef5-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4ef5-115">createdDateTime</span></span>|<span data-ttu-id="a4ef5-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4ef5-116">DateTimeOffset</span></span>|<span data-ttu-id="a4ef5-p101">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a4ef5-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a4ef5-119">id</span><span class="sxs-lookup"><span data-stu-id="a4ef5-119">id</span></span>|<span data-ttu-id="a4ef5-120">String</span><span class="sxs-lookup"><span data-stu-id="a4ef5-120">String</span></span>| <span data-ttu-id="a4ef5-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a4ef5-121">Read-only.</span></span>|
|<span data-ttu-id="a4ef5-122">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4ef5-122">lastModifiedDateTime</span></span>|<span data-ttu-id="a4ef5-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4ef5-123">DateTimeOffset</span></span>|<span data-ttu-id="a4ef5-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a4ef5-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4ef5-126">Связи</span><span class="sxs-lookup"><span data-stu-id="a4ef5-126">Relationships</span></span>
<span data-ttu-id="a4ef5-127">Нет</span><span class="sxs-lookup"><span data-stu-id="a4ef5-127">None</span></span>


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


