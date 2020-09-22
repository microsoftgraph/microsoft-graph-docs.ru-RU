---
title: Тип ресурса Медиапромпт
description: Содержит сведения о звуковом файле, который необходимо воспроизвести, и другие дополнительные параметры.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5b97e385cb14eb0315e9312c82e0ffd606adde2f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971748"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="1fed0-103">Тип ресурса Медиапромпт</span><span class="sxs-lookup"><span data-stu-id="1fed0-103">mediaPrompt resource type</span></span>

<span data-ttu-id="1fed0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fed0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fed0-105">Содержит сведения о звуковом файле, который необходимо воспроизвести, и другие дополнительные параметры.</span><span class="sxs-lookup"><span data-stu-id="1fed0-105">Contains information about the audio file to be played and other additional settings.</span></span>

## <a name="properties"></a><span data-ttu-id="1fed0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1fed0-106">Properties</span></span>

| <span data-ttu-id="1fed0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1fed0-107">Property</span></span>    | <span data-ttu-id="1fed0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1fed0-108">Type</span></span>                      | <span data-ttu-id="1fed0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1fed0-109">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="1fed0-110">медиаинфо</span><span class="sxs-lookup"><span data-stu-id="1fed0-110">mediaInfo</span></span>   | [<span data-ttu-id="1fed0-111">медиаинфо</span><span class="sxs-lookup"><span data-stu-id="1fed0-111">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="1fed0-112">Сведения о мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="1fed0-112">The media information.</span></span>                                                          |

## <a name="json-representation"></a><span data-ttu-id="1fed0-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1fed0-113">JSON representation</span></span>

<span data-ttu-id="1fed0-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1fed0-114">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="1fed0-115">Пример</span><span class="sxs-lookup"><span data-stu-id="1fed0-115">Example</span></span>

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


