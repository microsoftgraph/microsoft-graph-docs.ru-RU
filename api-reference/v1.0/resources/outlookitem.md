---
title: Тип ресурса outlookItem
description: Ниже представлено описание ресурса в формате JSON.
author: angelgolfer-ms
ms.openlocfilehash: 750239156e6f4e2874783ae160a7018fb58e259d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332517"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="84bff-103">Тип ресурса outlookItem</span><span class="sxs-lookup"><span data-stu-id="84bff-103">outlookItem resource type</span></span>



## <a name="json-representation"></a><span data-ttu-id="84bff-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84bff-104">JSON representation</span></span>

<span data-ttu-id="84bff-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="84bff-105">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="84bff-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="84bff-106">Properties</span></span>
| <span data-ttu-id="84bff-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="84bff-107">Property</span></span>     | <span data-ttu-id="84bff-108">Тип</span><span class="sxs-lookup"><span data-stu-id="84bff-108">Type</span></span>   |<span data-ttu-id="84bff-109">Описание</span><span class="sxs-lookup"><span data-stu-id="84bff-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84bff-110">categories</span><span class="sxs-lookup"><span data-stu-id="84bff-110">categories</span></span>|<span data-ttu-id="84bff-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="84bff-111">String collection</span></span>|<span data-ttu-id="84bff-112">Категории, связанный с элементом</span><span class="sxs-lookup"><span data-stu-id="84bff-112">The categories associated with the item</span></span>|
|<span data-ttu-id="84bff-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="84bff-113">changeKey</span></span>|<span data-ttu-id="84bff-114">Строка</span><span class="sxs-lookup"><span data-stu-id="84bff-114">String</span></span>|<span data-ttu-id="84bff-115">Определяет версию элемента.</span><span class="sxs-lookup"><span data-stu-id="84bff-115">Identifies the version of the item.</span></span> <span data-ttu-id="84bff-116">Каждый раз при изменении элемента changeKey также изменяется.</span><span class="sxs-lookup"><span data-stu-id="84bff-116">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="84bff-117">Это позволяет Exchange применить изменения к правильную версию объекта.</span><span class="sxs-lookup"><span data-stu-id="84bff-117">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="84bff-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84bff-118">Read-only.</span></span>|
|<span data-ttu-id="84bff-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84bff-119">createdDateTime</span></span>|<span data-ttu-id="84bff-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84bff-120">DateTimeOffset</span></span>|<span data-ttu-id="84bff-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="84bff-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="84bff-123">id</span><span class="sxs-lookup"><span data-stu-id="84bff-123">id</span></span>|<span data-ttu-id="84bff-124">Строка</span><span class="sxs-lookup"><span data-stu-id="84bff-124">String</span></span>| <span data-ttu-id="84bff-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84bff-125">Read-only.</span></span>|
|<span data-ttu-id="84bff-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84bff-126">lastModifiedDateTime</span></span>|<span data-ttu-id="84bff-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84bff-127">DateTimeOffset</span></span>|<span data-ttu-id="84bff-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="84bff-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="84bff-130">Связи</span><span class="sxs-lookup"><span data-stu-id="84bff-130">Relationships</span></span>
<span data-ttu-id="84bff-131">Нет</span><span class="sxs-lookup"><span data-stu-id="84bff-131">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
