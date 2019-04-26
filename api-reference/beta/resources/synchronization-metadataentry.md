---
title: Тип ресурса Метадатаентри
description: Метаданные для данного объекта.
localization_priority: Normal
ms.openlocfilehash: 829dc5fbbf3d73dbabb2e9e69bfff28814cc203a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345604"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="3f26b-103">Тип ресурса Метадатаентри</span><span class="sxs-lookup"><span data-stu-id="3f26b-103">metadataEntry resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f26b-104">Метаданные для данного объекта.</span><span class="sxs-lookup"><span data-stu-id="3f26b-104">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="3f26b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f26b-105">Properties</span></span>
| <span data-ttu-id="3f26b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f26b-106">Property</span></span>     | <span data-ttu-id="3f26b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3f26b-107">Type</span></span>   |<span data-ttu-id="3f26b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3f26b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f26b-109">key</span><span class="sxs-lookup"><span data-stu-id="3f26b-109">key</span></span>|<span data-ttu-id="3f26b-110">String</span><span class="sxs-lookup"><span data-stu-id="3f26b-110">String</span></span>|<span data-ttu-id="3f26b-111">Имя свойства метаданных.</span><span class="sxs-lookup"><span data-stu-id="3f26b-111">Name of the metadata property.</span></span>|
|<span data-ttu-id="3f26b-112">value</span><span class="sxs-lookup"><span data-stu-id="3f26b-112">value</span></span>|<span data-ttu-id="3f26b-113">String</span><span class="sxs-lookup"><span data-stu-id="3f26b-113">String</span></span>|<span data-ttu-id="3f26b-114">Значение свойства метаданных.</span><span class="sxs-lookup"><span data-stu-id="3f26b-114">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3f26b-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3f26b-115">JSON representation</span></span>

<span data-ttu-id="3f26b-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f26b-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataEntry"
}-->

```json
{
  "key": "String",
  "value": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "metadataEntry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
