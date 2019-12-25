---
title: Тип ресурса Медиапромпт
description: Этот тип ресурса содержит сведения о звуковом файле, который необходимо воспроизвести, и другие дополнительные параметры.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f981559ce5bac9bb597e49ff1b9d31e48413454b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871394"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="859f2-103">Тип ресурса Медиапромпт</span><span class="sxs-lookup"><span data-stu-id="859f2-103">mediaPrompt resource type</span></span>

<span data-ttu-id="859f2-104">Этот тип ресурса содержит сведения о звуковом файле, который необходимо воспроизвести, и другие дополнительные параметры.</span><span class="sxs-lookup"><span data-stu-id="859f2-104">This resource type contains information about the audio file to be played and other additional settings.</span></span>

## <a name="properties"></a><span data-ttu-id="859f2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="859f2-105">Properties</span></span>

| <span data-ttu-id="859f2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="859f2-106">Property</span></span>    | <span data-ttu-id="859f2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="859f2-107">Type</span></span>                      | <span data-ttu-id="859f2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="859f2-108">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="859f2-109">медиаинфо</span><span class="sxs-lookup"><span data-stu-id="859f2-109">mediaInfo</span></span>   | [<span data-ttu-id="859f2-110">медиаинфо</span><span class="sxs-lookup"><span data-stu-id="859f2-110">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="859f2-111">Сведения о мультимедиа</span><span class="sxs-lookup"><span data-stu-id="859f2-111">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="859f2-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="859f2-112">JSON representation</span></span>

<span data-ttu-id="859f2-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="859f2-113">The following is a JSON representation of the resource.</span></span>

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
