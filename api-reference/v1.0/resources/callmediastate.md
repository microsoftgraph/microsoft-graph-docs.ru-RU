---
title: тип ресурса callMediaState
description: Представляет состояние мультимедиа для вызова.
author: ananmishr
ms.prod: cloud-communications
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: f8797aadf7e35000d799c4c8b879ef2ed6da6409
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952538"
---
# <a name="callmediastate-resource-type"></a><span data-ttu-id="78b0b-103">тип ресурса callMediaState</span><span class="sxs-lookup"><span data-stu-id="78b0b-103">callMediaState resource type</span></span>

<span data-ttu-id="78b0b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78b0b-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="78b0b-105">Представляет состояние мультимедиа для [вызова.](call.md)</span><span class="sxs-lookup"><span data-stu-id="78b0b-105">Represents the media state for a [call](call.md).</span></span>

## <a name="properties"></a><span data-ttu-id="78b0b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="78b0b-106">Properties</span></span>

| <span data-ttu-id="78b0b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="78b0b-107">Property</span></span>            | <span data-ttu-id="78b0b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="78b0b-108">Type</span></span>    | <span data-ttu-id="78b0b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="78b0b-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="78b0b-110">audio</span><span class="sxs-lookup"><span data-stu-id="78b0b-110">audio</span></span>           | <span data-ttu-id="78b0b-111">mediaState</span><span class="sxs-lookup"><span data-stu-id="78b0b-111">mediaState</span></span>  | <span data-ttu-id="78b0b-112">Состояние аудио мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="78b0b-112">The audio media state.</span></span> <span data-ttu-id="78b0b-113">Возможные значения: `active`, `inactive`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="78b0b-113">Possible values are: `active`, `inactive`, `unknownFutureValue`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="78b0b-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78b0b-114">JSON representation</span></span>

<span data-ttu-id="78b0b-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78b0b-115">The following is a JSON representation of the resource.</span></span>

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

