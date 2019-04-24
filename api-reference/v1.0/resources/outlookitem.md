---
title: Тип ресурса outlookItem
description: Ниже этот ресурс представлен в формате JSON.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 3bbfe6119d279a1a708b44128a7d134664d7b040
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462643"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="3a218-103">Тип ресурса outlookItem</span><span class="sxs-lookup"><span data-stu-id="3a218-103">outlookItem resource type</span></span>



## <a name="json-representation"></a><span data-ttu-id="3a218-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3a218-104">JSON representation</span></span>

<span data-ttu-id="3a218-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="3a218-105">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="3a218-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3a218-106">Properties</span></span>
| <span data-ttu-id="3a218-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a218-107">Property</span></span>     | <span data-ttu-id="3a218-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3a218-108">Type</span></span>   |<span data-ttu-id="3a218-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3a218-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a218-110">categories</span><span class="sxs-lookup"><span data-stu-id="3a218-110">categories</span></span>|<span data-ttu-id="3a218-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3a218-111">String collection</span></span>|<span data-ttu-id="3a218-112">Категории, связанные с элементом</span><span class="sxs-lookup"><span data-stu-id="3a218-112">The categories associated with the item</span></span>|
|<span data-ttu-id="3a218-113">changeKey</span><span class="sxs-lookup"><span data-stu-id="3a218-113">changeKey</span></span>|<span data-ttu-id="3a218-114">String</span><span class="sxs-lookup"><span data-stu-id="3a218-114">String</span></span>|<span data-ttu-id="3a218-115">Определяет версию элемента.</span><span class="sxs-lookup"><span data-stu-id="3a218-115">Identifies the version of the item.</span></span> <span data-ttu-id="3a218-116">Каждый раз при изменении элемента Чанжекэй также изменяются.</span><span class="sxs-lookup"><span data-stu-id="3a218-116">Every time the item is changed, changeKey changes as well.</span></span> <span data-ttu-id="3a218-117">Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="3a218-117">This allows Exchange to apply changes to the correct version of the object.</span></span> <span data-ttu-id="3a218-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3a218-118">Read-only.</span></span>|
|<span data-ttu-id="3a218-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a218-119">createdDateTime</span></span>|<span data-ttu-id="3a218-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a218-120">DateTimeOffset</span></span>|<span data-ttu-id="3a218-p102">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3a218-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3a218-123">id</span><span class="sxs-lookup"><span data-stu-id="3a218-123">id</span></span>|<span data-ttu-id="3a218-124">String</span><span class="sxs-lookup"><span data-stu-id="3a218-124">String</span></span>| <span data-ttu-id="3a218-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3a218-125">Read-only.</span></span>|
|<span data-ttu-id="3a218-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a218-126">lastModifiedDateTime</span></span>|<span data-ttu-id="3a218-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a218-127">DateTimeOffset</span></span>|<span data-ttu-id="3a218-p103">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3a218-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a218-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="3a218-130">Relationships</span></span>
<span data-ttu-id="3a218-131">Нет</span><span class="sxs-lookup"><span data-stu-id="3a218-131">None</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
