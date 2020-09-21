---
title: Тип ресурса Медиапромпт
description: Этот тип ресурса содержит сведения о звуковом файле, который необходимо воспроизвести, и другие дополнительные параметры.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 37329364ccfcb4b70de04ebfe8344ea407ce2bc7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965521"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="39e6a-103">Тип ресурса Медиапромпт</span><span class="sxs-lookup"><span data-stu-id="39e6a-103">mediaPrompt resource type</span></span>

<span data-ttu-id="39e6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39e6a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="39e6a-105">Этот тип ресурса содержит сведения о звуковом файле, который необходимо воспроизвести, и другие дополнительные параметры.</span><span class="sxs-lookup"><span data-stu-id="39e6a-105">This resource type contains information about the audio file to be played and other additional settings.</span></span>

## <a name="properties"></a><span data-ttu-id="39e6a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="39e6a-106">Properties</span></span>

| <span data-ttu-id="39e6a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="39e6a-107">Property</span></span>    | <span data-ttu-id="39e6a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="39e6a-108">Type</span></span>                      | <span data-ttu-id="39e6a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="39e6a-109">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="39e6a-110">медиаинфо</span><span class="sxs-lookup"><span data-stu-id="39e6a-110">mediaInfo</span></span>   | [<span data-ttu-id="39e6a-111">медиаинфо</span><span class="sxs-lookup"><span data-stu-id="39e6a-111">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="39e6a-112">Сведения о мультимедиа</span><span class="sxs-lookup"><span data-stu-id="39e6a-112">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="39e6a-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="39e6a-113">JSON representation</span></span>

<span data-ttu-id="39e6a-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39e6a-114">The following is a JSON representation of the resource.</span></span>

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

