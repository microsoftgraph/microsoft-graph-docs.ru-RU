---
title: Тип ресурса Каллмедиастате
description: Представляет состояние мультимедиа для вызова.
author: VinodRavichandran
ms.prod: cloud-communications
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: 01e2e8017d89ddf96997d1d5bef729f9e9dc439d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871402"
---
# <a name="callmediastate-resource-type"></a><span data-ttu-id="da607-103">Тип ресурса Каллмедиастате</span><span class="sxs-lookup"><span data-stu-id="da607-103">callMediaState resource type</span></span>


<span data-ttu-id="da607-104">Представляет состояние мультимедиа для [вызова](call.md).</span><span class="sxs-lookup"><span data-stu-id="da607-104">Represents the media state for a [call](call.md).</span></span>

## <a name="properties"></a><span data-ttu-id="da607-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="da607-105">Properties</span></span>

| <span data-ttu-id="da607-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="da607-106">Property</span></span>            | <span data-ttu-id="da607-107">Тип</span><span class="sxs-lookup"><span data-stu-id="da607-107">Type</span></span>    | <span data-ttu-id="da607-108">Описание</span><span class="sxs-lookup"><span data-stu-id="da607-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="da607-109">audio</span><span class="sxs-lookup"><span data-stu-id="da607-109">audio</span></span>           | <span data-ttu-id="da607-110">String</span><span class="sxs-lookup"><span data-stu-id="da607-110">String</span></span>  | <span data-ttu-id="da607-111">Состояние звукового носителя.</span><span class="sxs-lookup"><span data-stu-id="da607-111">The audio media state.</span></span> <span data-ttu-id="da607-112">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="da607-112">Possible values are: `active`, `inactive`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="da607-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da607-113">JSON representation</span></span>

<span data-ttu-id="da607-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da607-114">The following is a JSON representation of the resource.</span></span>

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
