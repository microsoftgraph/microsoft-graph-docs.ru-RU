---
title: Тип ресурса Метадатаентри
description: Метаданные для данного объекта.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 49c43e502cfb06832172f46c1e790b2a20eb0f08
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620558"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="2369b-103">Тип ресурса Метадатаентри</span><span class="sxs-lookup"><span data-stu-id="2369b-103">metadataEntry resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2369b-104">Метаданные для данного объекта.</span><span class="sxs-lookup"><span data-stu-id="2369b-104">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="2369b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2369b-105">Properties</span></span>
| <span data-ttu-id="2369b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2369b-106">Property</span></span>     | <span data-ttu-id="2369b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2369b-107">Type</span></span>   |<span data-ttu-id="2369b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2369b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2369b-109">key</span><span class="sxs-lookup"><span data-stu-id="2369b-109">key</span></span>|<span data-ttu-id="2369b-110">String</span><span class="sxs-lookup"><span data-stu-id="2369b-110">String</span></span>|<span data-ttu-id="2369b-111">Имя свойства метаданных.</span><span class="sxs-lookup"><span data-stu-id="2369b-111">Name of the metadata property.</span></span>|
|<span data-ttu-id="2369b-112">value</span><span class="sxs-lookup"><span data-stu-id="2369b-112">value</span></span>|<span data-ttu-id="2369b-113">String</span><span class="sxs-lookup"><span data-stu-id="2369b-113">String</span></span>|<span data-ttu-id="2369b-114">Значение свойства метаданных.</span><span class="sxs-lookup"><span data-stu-id="2369b-114">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2369b-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2369b-115">JSON representation</span></span>

<span data-ttu-id="2369b-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2369b-116">The following is a JSON representation of the resource.</span></span>

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
