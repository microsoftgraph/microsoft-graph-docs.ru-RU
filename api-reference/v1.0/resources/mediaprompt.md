---
title: Тип ресурса Медиапромпт
description: Этот тип ресурса содержит сведения о звуковом файле, который необходимо воспроизвести, и другие дополнительные параметры.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0ef83d9645ac4277893ff8c769ecb6e092e3e84d
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913200"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="25a53-103">Тип ресурса Медиапромпт</span><span class="sxs-lookup"><span data-stu-id="25a53-103">mediaPrompt resource type</span></span>

<span data-ttu-id="25a53-104">Этот тип ресурса содержит сведения о звуковом файле, который необходимо воспроизвести, и другие дополнительные параметры.</span><span class="sxs-lookup"><span data-stu-id="25a53-104">This resource type contains information about the audio file to be played and other additional settings.</span></span>

## <a name="properties"></a><span data-ttu-id="25a53-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="25a53-105">Properties</span></span>

| <span data-ttu-id="25a53-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="25a53-106">Property</span></span>    | <span data-ttu-id="25a53-107">Тип</span><span class="sxs-lookup"><span data-stu-id="25a53-107">Type</span></span>                      | <span data-ttu-id="25a53-108">Описание</span><span class="sxs-lookup"><span data-stu-id="25a53-108">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="25a53-109">медиаинфо</span><span class="sxs-lookup"><span data-stu-id="25a53-109">mediaInfo</span></span>   | [<span data-ttu-id="25a53-110">медиаинфо</span><span class="sxs-lookup"><span data-stu-id="25a53-110">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="25a53-111">Сведения о мультимедиа</span><span class="sxs-lookup"><span data-stu-id="25a53-111">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="25a53-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="25a53-112">JSON representation</span></span>

<span data-ttu-id="25a53-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25a53-113">The following is a JSON representation of the resource.</span></span>

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
