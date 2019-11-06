---
title: Тип ресурса Медиаконфиг
description: Конфигурация мультимедиа, используемая для подключения к вызову.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f42f83923922cdf868dfa39ea3618f7fed2a37c6
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006678"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="e7724-103">Тип ресурса Медиаконфиг</span><span class="sxs-lookup"><span data-stu-id="e7724-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7724-104">Конфигурация мультимедиа, используемая для подключения к вызову.</span><span class="sxs-lookup"><span data-stu-id="e7724-104">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="e7724-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7724-105">Properties</span></span>

| <span data-ttu-id="e7724-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7724-106">Property</span></span>       | <span data-ttu-id="e7724-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e7724-107">Type</span></span>    | <span data-ttu-id="e7724-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e7724-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e7724-109">ремовефромдефаултаудиограуп</span><span class="sxs-lookup"><span data-stu-id="e7724-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="e7724-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7724-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="e7724-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e7724-111">JSON representation</span></span>

<span data-ttu-id="e7724-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7724-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
   ],
  "abstract": true,
  "@odata.type": "microsoft.graph.mediaConfig"
}-->
```json
{
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
