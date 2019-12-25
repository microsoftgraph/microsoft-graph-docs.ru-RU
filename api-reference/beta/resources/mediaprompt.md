---
title: Тип ресурса Медиапромпт
description: Содержит сведения о звуковом файле, который необходимо воспроизвести, и другие дополнительные параметры.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ba04bda06fa4adfe158046e5e0b251e770e5ee38
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866709"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="900ed-103">Тип ресурса Медиапромпт</span><span class="sxs-lookup"><span data-stu-id="900ed-103">mediaPrompt resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="900ed-104">Содержит сведения о звуковом файле, который необходимо воспроизвести, и другие дополнительные параметры.</span><span class="sxs-lookup"><span data-stu-id="900ed-104">Contains information about the audio file to be played and other additional settings.</span></span>

## <a name="properties"></a><span data-ttu-id="900ed-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="900ed-105">Properties</span></span>

| <span data-ttu-id="900ed-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="900ed-106">Property</span></span>    | <span data-ttu-id="900ed-107">Тип</span><span class="sxs-lookup"><span data-stu-id="900ed-107">Type</span></span>                      | <span data-ttu-id="900ed-108">Описание</span><span class="sxs-lookup"><span data-stu-id="900ed-108">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="900ed-109">медиаинфо</span><span class="sxs-lookup"><span data-stu-id="900ed-109">mediaInfo</span></span>   | [<span data-ttu-id="900ed-110">медиаинфо</span><span class="sxs-lookup"><span data-stu-id="900ed-110">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="900ed-111">Сведения о мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="900ed-111">The media information.</span></span>                                                          |

## <a name="json-representation"></a><span data-ttu-id="900ed-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="900ed-112">JSON representation</span></span>

<span data-ttu-id="900ed-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="900ed-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

## <a name="example"></a><span data-ttu-id="900ed-114">Пример</span><span class="sxs-lookup"><span data-stu-id="900ed-114">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->
```json
{
  "@odata.type": "#microsoft.graph.mediaPrompt",
  "mediaInfo": {
    "@odata.type": "#microsoft.graph.mediaInfo",
    "uri": "https://cdn.contoso.com/beep.wav",
    "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
