---
title: тип ресурса callMediaState
description: Представляет состояние мультимедиа для вызова.
author: ananmishr
ms.prod: cloud-communications
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: 6cbdc4feb50428fb3007b5a61362381d9c55a78a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955020"
---
# <a name="callmediastate-resource-type"></a><span data-ttu-id="84153-103">тип ресурса callMediaState</span><span class="sxs-lookup"><span data-stu-id="84153-103">callMediaState resource type</span></span>

<span data-ttu-id="84153-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84153-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84153-105">Представляет состояние мультимедиа для [вызова.](call.md)</span><span class="sxs-lookup"><span data-stu-id="84153-105">Represents the media state for a [call](call.md).</span></span>

## <a name="properties"></a><span data-ttu-id="84153-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="84153-106">Properties</span></span>

| <span data-ttu-id="84153-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="84153-107">Property</span></span>            | <span data-ttu-id="84153-108">Тип</span><span class="sxs-lookup"><span data-stu-id="84153-108">Type</span></span>    | <span data-ttu-id="84153-109">Описание</span><span class="sxs-lookup"><span data-stu-id="84153-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="84153-110">audio</span><span class="sxs-lookup"><span data-stu-id="84153-110">audio</span></span>           | <span data-ttu-id="84153-111">mediaState</span><span class="sxs-lookup"><span data-stu-id="84153-111">mediaState</span></span>  | <span data-ttu-id="84153-112">Состояние аудио мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="84153-112">The audio media state.</span></span> <span data-ttu-id="84153-113">Возможные значения: `active`, `inactive`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="84153-113">Possible values are: `active`, `inactive`, `unknownFutureValue`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="84153-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84153-114">JSON representation</span></span>

<span data-ttu-id="84153-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84153-115">The following is a JSON representation of the resource.</span></span>

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


