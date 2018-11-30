---
title: Тип ресурса outlookItem
description: Ниже представлено описание ресурса в формате JSON.
ms.openlocfilehash: 5f81598b62d2b47230f4a7ce16d17b8056bc9874
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025190"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="c991f-103">Тип ресурса outlookItem</span><span class="sxs-lookup"><span data-stu-id="c991f-103">outlookItem resource type</span></span>



## <a name="json-representation"></a><span data-ttu-id="c991f-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c991f-104">JSON representation</span></span>

<span data-ttu-id="c991f-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="c991f-105">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="c991f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c991f-106">Properties</span></span>
| <span data-ttu-id="c991f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c991f-107">Property</span></span>     | <span data-ttu-id="c991f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c991f-108">Type</span></span>   |<span data-ttu-id="c991f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c991f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c991f-110">categories</span><span class="sxs-lookup"><span data-stu-id="c991f-110">categories</span></span>|<span data-ttu-id="c991f-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c991f-111">String collection</span></span>|<span data-ttu-id="c991f-112">Категории, связанный с элементом</span><span class="sxs-lookup"><span data-stu-id="c991f-112">The categories associated with the item</span></span>|
|<span data-ttu-id="c991f-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="c991f-113">changeKey</span></span>|<span data-ttu-id="c991f-114">String</span><span class="sxs-lookup"><span data-stu-id="c991f-114">String</span></span>|<span data-ttu-id="c991f-115">Определяет версию элемента.</span><span class="sxs-lookup"><span data-stu-id="c991f-115">Identifies the version of the item.</span></span> <span data-ttu-id="c991f-116">Каждый раз при изменении элемента changeKey также изменяется.</span><span class="sxs-lookup"><span data-stu-id="c991f-116">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="c991f-117">Это позволяет Exchange применить изменения к правильную версию объекта.</span><span class="sxs-lookup"><span data-stu-id="c991f-117">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="c991f-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c991f-118">Read-only.</span></span>|
|<span data-ttu-id="c991f-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c991f-119">createdDateTime</span></span>|<span data-ttu-id="c991f-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c991f-120">DateTimeOffset</span></span>|<span data-ttu-id="c991f-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c991f-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c991f-123">id</span><span class="sxs-lookup"><span data-stu-id="c991f-123">id</span></span>|<span data-ttu-id="c991f-124">String</span><span class="sxs-lookup"><span data-stu-id="c991f-124">String</span></span>| <span data-ttu-id="c991f-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c991f-125">Read-only.</span></span>|
|<span data-ttu-id="c991f-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c991f-126">lastModifiedDateTime</span></span>|<span data-ttu-id="c991f-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c991f-127">DateTimeOffset</span></span>|<span data-ttu-id="c991f-p103">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c991f-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="c991f-130">Связи</span><span class="sxs-lookup"><span data-stu-id="c991f-130">Relationships</span></span>
<span data-ttu-id="c991f-131">Нет</span><span class="sxs-lookup"><span data-stu-id="c991f-131">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
