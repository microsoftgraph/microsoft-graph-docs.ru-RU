---
title: Тип ресурса outlookItem
description: Ниже показано представление JSON ресурса.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 37a9d548e0eac3d07a66ca4b28c243c076a743bb
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721539"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="eaf9c-103">Тип ресурса outlookItem</span><span class="sxs-lookup"><span data-stu-id="eaf9c-103">outlookItem resource type</span></span>

<span data-ttu-id="eaf9c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eaf9c-104">Namespace: microsoft.graph</span></span>



## <a name="json-representation"></a><span data-ttu-id="eaf9c-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eaf9c-105">JSON representation</span></span>

<span data-ttu-id="eaf9c-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="eaf9c-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="eaf9c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="eaf9c-107">Properties</span></span>
| <span data-ttu-id="eaf9c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="eaf9c-108">Property</span></span>     | <span data-ttu-id="eaf9c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="eaf9c-109">Type</span></span>   |<span data-ttu-id="eaf9c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eaf9c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eaf9c-111">categories</span><span class="sxs-lookup"><span data-stu-id="eaf9c-111">categories</span></span>|<span data-ttu-id="eaf9c-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="eaf9c-112">String collection</span></span>|<span data-ttu-id="eaf9c-113">Категории, связанные с элементом</span><span class="sxs-lookup"><span data-stu-id="eaf9c-113">The categories associated with the item</span></span>|
|<span data-ttu-id="eaf9c-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="eaf9c-114">changeKey</span></span>|<span data-ttu-id="eaf9c-115">String</span><span class="sxs-lookup"><span data-stu-id="eaf9c-115">String</span></span>|<span data-ttu-id="eaf9c-116">Определяет версию элемента.</span><span class="sxs-lookup"><span data-stu-id="eaf9c-116">Identifies the version of the item.</span></span> <span data-ttu-id="eaf9c-117">Каждый раз, когда элемент изменяется, изменяется и changeKey.</span><span class="sxs-lookup"><span data-stu-id="eaf9c-117">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="eaf9c-118">Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="eaf9c-118">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="eaf9c-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eaf9c-119">Read-only.</span></span>|
|<span data-ttu-id="eaf9c-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eaf9c-120">createdDateTime</span></span>|<span data-ttu-id="eaf9c-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaf9c-121">DateTimeOffset</span></span>|<span data-ttu-id="eaf9c-122">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="eaf9c-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eaf9c-123">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="eaf9c-123">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="eaf9c-124">id</span><span class="sxs-lookup"><span data-stu-id="eaf9c-124">id</span></span>|<span data-ttu-id="eaf9c-125">String</span><span class="sxs-lookup"><span data-stu-id="eaf9c-125">String</span></span>| <span data-ttu-id="eaf9c-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eaf9c-126">Read-only.</span></span>|
|<span data-ttu-id="eaf9c-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eaf9c-127">lastModifiedDateTime</span></span>|<span data-ttu-id="eaf9c-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaf9c-128">DateTimeOffset</span></span>|<span data-ttu-id="eaf9c-129">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="eaf9c-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eaf9c-130">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="eaf9c-130">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="eaf9c-131">Связи</span><span class="sxs-lookup"><span data-stu-id="eaf9c-131">Relationships</span></span>
<span data-ttu-id="eaf9c-132">Нет</span><span class="sxs-lookup"><span data-stu-id="eaf9c-132">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

