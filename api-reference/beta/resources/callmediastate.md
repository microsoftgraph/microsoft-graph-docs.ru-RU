---
title: Тип ресурса Каллмедиастате
description: Представляет состояние мультимедиа для вызова.
author: VinodRavichandran
ms.prod: cloud-communications
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: 29402e813f6816ebea02ad2bb86c403408c2ff81
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006749"
---
# <a name="callmediastate-resource-type"></a><span data-ttu-id="04118-103">Тип ресурса Каллмедиастате</span><span class="sxs-lookup"><span data-stu-id="04118-103">callMediaState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04118-104">Представляет состояние мультимедиа для [вызова](call.md).</span><span class="sxs-lookup"><span data-stu-id="04118-104">Represents the media state for a [call](call.md).</span></span>

## <a name="properties"></a><span data-ttu-id="04118-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="04118-105">Properties</span></span>

| <span data-ttu-id="04118-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="04118-106">Property</span></span>            | <span data-ttu-id="04118-107">Тип</span><span class="sxs-lookup"><span data-stu-id="04118-107">Type</span></span>    | <span data-ttu-id="04118-108">Описание</span><span class="sxs-lookup"><span data-stu-id="04118-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="04118-109">audio</span><span class="sxs-lookup"><span data-stu-id="04118-109">audio</span></span>           | <span data-ttu-id="04118-110">String</span><span class="sxs-lookup"><span data-stu-id="04118-110">String</span></span>  | <span data-ttu-id="04118-111">Состояние звукового носителя.</span><span class="sxs-lookup"><span data-stu-id="04118-111">The audio media state.</span></span> <span data-ttu-id="04118-112">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="04118-112">Possible values are: `active`, `inactive`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="04118-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04118-113">JSON representation</span></span>

<span data-ttu-id="04118-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04118-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callMediaState"
}-->
```json
{
  "audio": "active | inactive",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callMediaState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
