---
title: Тип ресурса outlookItem
description: Ниже представлено описание ресурса в формате JSON.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: aa5e4af03171029e8557e38d3a75062161435318
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534104"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="3e7cc-103">Тип ресурса outlookItem</span><span class="sxs-lookup"><span data-stu-id="3e7cc-103">outlookItem resource type</span></span>

<span data-ttu-id="3e7cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e7cc-104">Namespace: microsoft.graph</span></span>



## <a name="json-representation"></a><span data-ttu-id="3e7cc-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e7cc-105">JSON representation</span></span>

<span data-ttu-id="3e7cc-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="3e7cc-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="3e7cc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e7cc-107">Properties</span></span>
| <span data-ttu-id="3e7cc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e7cc-108">Property</span></span>     | <span data-ttu-id="3e7cc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3e7cc-109">Type</span></span>   |<span data-ttu-id="3e7cc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3e7cc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e7cc-111">categories</span><span class="sxs-lookup"><span data-stu-id="3e7cc-111">categories</span></span>|<span data-ttu-id="3e7cc-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3e7cc-112">String collection</span></span>|<span data-ttu-id="3e7cc-113">Категории, связанные с элементом</span><span class="sxs-lookup"><span data-stu-id="3e7cc-113">The categories associated with the item</span></span>|
|<span data-ttu-id="3e7cc-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="3e7cc-114">changeKey</span></span>|<span data-ttu-id="3e7cc-115">Строка</span><span class="sxs-lookup"><span data-stu-id="3e7cc-115">String</span></span>|<span data-ttu-id="3e7cc-116">Определяет версию элемента.</span><span class="sxs-lookup"><span data-stu-id="3e7cc-116">Identifies the version of the item.</span></span> <span data-ttu-id="3e7cc-117">Каждый раз при изменении элемента Чанжекэй также изменяются.</span><span class="sxs-lookup"><span data-stu-id="3e7cc-117">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="3e7cc-118">Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="3e7cc-118">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="3e7cc-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e7cc-119">Read-only.</span></span>|
|<span data-ttu-id="3e7cc-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e7cc-120">createdDateTime</span></span>|<span data-ttu-id="3e7cc-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e7cc-121">DateTimeOffset</span></span>|<span data-ttu-id="3e7cc-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3e7cc-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3e7cc-124">id</span><span class="sxs-lookup"><span data-stu-id="3e7cc-124">id</span></span>|<span data-ttu-id="3e7cc-125">String</span><span class="sxs-lookup"><span data-stu-id="3e7cc-125">String</span></span>| <span data-ttu-id="3e7cc-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3e7cc-126">Read-only.</span></span>|
|<span data-ttu-id="3e7cc-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e7cc-127">lastModifiedDateTime</span></span>|<span data-ttu-id="3e7cc-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e7cc-128">DateTimeOffset</span></span>|<span data-ttu-id="3e7cc-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3e7cc-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e7cc-131">Связи</span><span class="sxs-lookup"><span data-stu-id="3e7cc-131">Relationships</span></span>
<span data-ttu-id="3e7cc-132">Нет</span><span class="sxs-lookup"><span data-stu-id="3e7cc-132">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
