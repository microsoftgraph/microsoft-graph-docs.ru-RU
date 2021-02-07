---
title: Тип ресурса outlookItem
description: Ниже представлено описание ресурса в формате JSON.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 284a53ab713be49d29c19a6d4b69b3b51047977f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137363"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="5e91d-103">Тип ресурса outlookItem</span><span class="sxs-lookup"><span data-stu-id="5e91d-103">outlookItem resource type</span></span>

<span data-ttu-id="5e91d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e91d-104">Namespace: microsoft.graph</span></span>



## <a name="json-representation"></a><span data-ttu-id="5e91d-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e91d-105">JSON representation</span></span>

<span data-ttu-id="5e91d-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="5e91d-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="5e91d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e91d-107">Properties</span></span>
| <span data-ttu-id="5e91d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e91d-108">Property</span></span>     | <span data-ttu-id="5e91d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5e91d-109">Type</span></span>   |<span data-ttu-id="5e91d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5e91d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e91d-111">categories</span><span class="sxs-lookup"><span data-stu-id="5e91d-111">categories</span></span>|<span data-ttu-id="5e91d-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5e91d-112">String collection</span></span>|<span data-ttu-id="5e91d-113">Категории, связанные с элементом</span><span class="sxs-lookup"><span data-stu-id="5e91d-113">The categories associated with the item</span></span>|
|<span data-ttu-id="5e91d-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="5e91d-114">changeKey</span></span>|<span data-ttu-id="5e91d-115">String</span><span class="sxs-lookup"><span data-stu-id="5e91d-115">String</span></span>|<span data-ttu-id="5e91d-116">Определяет версию элемента.</span><span class="sxs-lookup"><span data-stu-id="5e91d-116">Identifies the version of the item.</span></span> <span data-ttu-id="5e91d-117">При каждом изменении элемента также изменяется элемент changeKey.</span><span class="sxs-lookup"><span data-stu-id="5e91d-117">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="5e91d-118">Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="5e91d-118">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="5e91d-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e91d-119">Read-only.</span></span>|
|<span data-ttu-id="5e91d-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e91d-120">createdDateTime</span></span>|<span data-ttu-id="5e91d-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e91d-121">DateTimeOffset</span></span>|<span data-ttu-id="5e91d-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5e91d-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5e91d-124">id</span><span class="sxs-lookup"><span data-stu-id="5e91d-124">id</span></span>|<span data-ttu-id="5e91d-125">String</span><span class="sxs-lookup"><span data-stu-id="5e91d-125">String</span></span>| <span data-ttu-id="5e91d-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e91d-126">Read-only.</span></span>|
|<span data-ttu-id="5e91d-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e91d-127">lastModifiedDateTime</span></span>|<span data-ttu-id="5e91d-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e91d-128">DateTimeOffset</span></span>|<span data-ttu-id="5e91d-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5e91d-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e91d-131">Связи</span><span class="sxs-lookup"><span data-stu-id="5e91d-131">Relationships</span></span>
<span data-ttu-id="5e91d-132">Нет</span><span class="sxs-lookup"><span data-stu-id="5e91d-132">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

