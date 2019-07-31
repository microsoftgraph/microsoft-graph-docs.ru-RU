---
title: Тип ресурса Метадатаентри
description: Метаданные для данного объекта.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 55b686bc04ccf869ddf9d6dc6029c6206f7b2274
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964844"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="ddefe-103">Тип ресурса Метадатаентри</span><span class="sxs-lookup"><span data-stu-id="ddefe-103">metadataEntry resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddefe-104">Метаданные для данного объекта.</span><span class="sxs-lookup"><span data-stu-id="ddefe-104">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="ddefe-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ddefe-105">Properties</span></span>
| <span data-ttu-id="ddefe-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ddefe-106">Property</span></span>     | <span data-ttu-id="ddefe-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ddefe-107">Type</span></span>   |<span data-ttu-id="ddefe-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ddefe-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ddefe-109">key</span><span class="sxs-lookup"><span data-stu-id="ddefe-109">key</span></span>|<span data-ttu-id="ddefe-110">String</span><span class="sxs-lookup"><span data-stu-id="ddefe-110">String</span></span>|<span data-ttu-id="ddefe-111">Имя свойства метаданных.</span><span class="sxs-lookup"><span data-stu-id="ddefe-111">Name of the metadata property.</span></span>|
|<span data-ttu-id="ddefe-112">value</span><span class="sxs-lookup"><span data-stu-id="ddefe-112">value</span></span>|<span data-ttu-id="ddefe-113">String</span><span class="sxs-lookup"><span data-stu-id="ddefe-113">String</span></span>|<span data-ttu-id="ddefe-114">Значение свойства метаданных.</span><span class="sxs-lookup"><span data-stu-id="ddefe-114">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ddefe-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ddefe-115">JSON representation</span></span>

<span data-ttu-id="ddefe-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ddefe-116">The following is a JSON representation of the resource.</span></span>

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
