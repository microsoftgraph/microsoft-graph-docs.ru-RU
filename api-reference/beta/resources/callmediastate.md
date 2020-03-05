---
title: Тип ресурса Каллмедиастате
description: Представляет состояние мультимедиа для вызова.
author: ananmishr
ms.prod: cloud-communications
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: c9c55908f62214c386aacee34be76bb11fc318b7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507812"
---
# <a name="callmediastate-resource-type"></a><span data-ttu-id="56307-103">Тип ресурса Каллмедиастате</span><span class="sxs-lookup"><span data-stu-id="56307-103">callMediaState resource type</span></span>

<span data-ttu-id="56307-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="56307-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56307-105">Представляет состояние мультимедиа для [вызова](call.md).</span><span class="sxs-lookup"><span data-stu-id="56307-105">Represents the media state for a [call](call.md).</span></span>

## <a name="properties"></a><span data-ttu-id="56307-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="56307-106">Properties</span></span>

| <span data-ttu-id="56307-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="56307-107">Property</span></span>            | <span data-ttu-id="56307-108">Тип</span><span class="sxs-lookup"><span data-stu-id="56307-108">Type</span></span>    | <span data-ttu-id="56307-109">Описание</span><span class="sxs-lookup"><span data-stu-id="56307-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="56307-110">audio</span><span class="sxs-lookup"><span data-stu-id="56307-110">audio</span></span>           | <span data-ttu-id="56307-111">String</span><span class="sxs-lookup"><span data-stu-id="56307-111">String</span></span>  | <span data-ttu-id="56307-112">Состояние звукового носителя.</span><span class="sxs-lookup"><span data-stu-id="56307-112">The audio media state.</span></span> <span data-ttu-id="56307-113">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="56307-113">Possible values are: `active`, `inactive`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="56307-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56307-114">JSON representation</span></span>

<span data-ttu-id="56307-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56307-115">The following is a JSON representation of the resource.</span></span>

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
