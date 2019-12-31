---
title: Тип ресурса Каллмедиастате
description: Представляет состояние мультимедиа для вызова.
author: ananmishr
ms.prod: cloud-communications
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: 14342a6657392dcfd16d32d1b6ce8d5bbf46ddf7
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913326"
---
# <a name="callmediastate-resource-type"></a><span data-ttu-id="9f784-103">Тип ресурса Каллмедиастате</span><span class="sxs-lookup"><span data-stu-id="9f784-103">callMediaState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f784-104">Представляет состояние мультимедиа для [вызова](call.md).</span><span class="sxs-lookup"><span data-stu-id="9f784-104">Represents the media state for a [call](call.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9f784-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f784-105">Properties</span></span>

| <span data-ttu-id="9f784-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f784-106">Property</span></span>            | <span data-ttu-id="9f784-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9f784-107">Type</span></span>    | <span data-ttu-id="9f784-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9f784-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="9f784-109">audio</span><span class="sxs-lookup"><span data-stu-id="9f784-109">audio</span></span>           | <span data-ttu-id="9f784-110">String</span><span class="sxs-lookup"><span data-stu-id="9f784-110">String</span></span>  | <span data-ttu-id="9f784-111">Состояние звукового носителя.</span><span class="sxs-lookup"><span data-stu-id="9f784-111">The audio media state.</span></span> <span data-ttu-id="9f784-112">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="9f784-112">Possible values are: `active`, `inactive`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9f784-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9f784-113">JSON representation</span></span>

<span data-ttu-id="9f784-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f784-114">The following is a JSON representation of the resource.</span></span>

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
