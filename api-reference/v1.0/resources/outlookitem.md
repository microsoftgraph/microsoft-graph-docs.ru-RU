---
title: Тип ресурса outlookItem
description: Ниже этот ресурс представлен в формате JSON.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 7b04d84019cbb38f78ef1df63e4e39480c4d949b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035660"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="97afb-103">Тип ресурса outlookItem</span><span class="sxs-lookup"><span data-stu-id="97afb-103">outlookItem resource type</span></span>



## <a name="json-representation"></a><span data-ttu-id="97afb-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97afb-104">JSON representation</span></span>

<span data-ttu-id="97afb-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="97afb-105">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
## <a name="properties"></a><span data-ttu-id="97afb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="97afb-106">Properties</span></span>
| <span data-ttu-id="97afb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="97afb-107">Property</span></span>     | <span data-ttu-id="97afb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="97afb-108">Type</span></span>   |<span data-ttu-id="97afb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="97afb-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97afb-110">categories</span><span class="sxs-lookup"><span data-stu-id="97afb-110">categories</span></span>|<span data-ttu-id="97afb-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="97afb-111">String collection</span></span>|<span data-ttu-id="97afb-112">Категории, связанные с элементом</span><span class="sxs-lookup"><span data-stu-id="97afb-112">The categories associated with the item</span></span>|
|<span data-ttu-id="97afb-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="97afb-113">changeKey</span></span>|<span data-ttu-id="97afb-114">String</span><span class="sxs-lookup"><span data-stu-id="97afb-114">String</span></span>|<span data-ttu-id="97afb-115">Определяет версию элемента.</span><span class="sxs-lookup"><span data-stu-id="97afb-115">Identifies the version of the item.</span></span> <span data-ttu-id="97afb-116">Каждый раз при изменении элемента Чанжекэй также изменяются.</span><span class="sxs-lookup"><span data-stu-id="97afb-116">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="97afb-117">Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="97afb-117">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="97afb-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97afb-118">Read-only.</span></span>|
|<span data-ttu-id="97afb-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97afb-119">createdDateTime</span></span>|<span data-ttu-id="97afb-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97afb-120">DateTimeOffset</span></span>|<span data-ttu-id="97afb-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="97afb-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="97afb-123">id</span><span class="sxs-lookup"><span data-stu-id="97afb-123">id</span></span>|<span data-ttu-id="97afb-124">String</span><span class="sxs-lookup"><span data-stu-id="97afb-124">String</span></span>| <span data-ttu-id="97afb-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97afb-125">Read-only.</span></span>|
|<span data-ttu-id="97afb-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97afb-126">lastModifiedDateTime</span></span>|<span data-ttu-id="97afb-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97afb-127">DateTimeOffset</span></span>|<span data-ttu-id="97afb-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="97afb-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="97afb-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="97afb-130">Relationships</span></span>
<span data-ttu-id="97afb-131">Нет</span><span class="sxs-lookup"><span data-stu-id="97afb-131">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
