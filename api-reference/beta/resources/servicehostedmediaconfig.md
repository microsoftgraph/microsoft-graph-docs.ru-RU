---
title: Тип ресурса serviceHostedMediaConfig
description: Тип serviceHostedMediaConfig.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d3b1ac252f13e023f56bb419625a35769570337a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991988"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="bb696-103">Тип ресурса serviceHostedMediaConfig</span><span class="sxs-lookup"><span data-stu-id="bb696-103">serviceHostedMediaConfig resource type</span></span>

> <span data-ttu-id="bb696-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bb696-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb696-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb696-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bb696-106">Тип serviceHostedMediaConfig.</span><span class="sxs-lookup"><span data-stu-id="bb696-106">The serviceHostedMediaConfig type.</span></span>

## <a name="properties"></a><span data-ttu-id="bb696-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb696-107">Properties</span></span>

| <span data-ttu-id="bb696-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb696-108">Property</span></span>                    | <span data-ttu-id="bb696-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bb696-109">Type</span></span>                                                        | <span data-ttu-id="bb696-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bb696-110">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="bb696-111">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="bb696-111">preFetchMedia</span></span>               | <span data-ttu-id="bb696-112">[mediaInfo](mediainfo.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="bb696-112">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="bb696-113">Список мультимедиа для предварительно выборки.</span><span class="sxs-lookup"><span data-stu-id="bb696-113">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="bb696-114">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="bb696-114">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="bb696-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb696-115">Boolean</span></span>                                                     | <span data-ttu-id="bb696-116">Удалите собственный участника из группы по умолчанию звука.</span><span class="sxs-lookup"><span data-stu-id="bb696-116">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bb696-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb696-117">JSON representation</span></span>

<span data-ttu-id="bb696-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb696-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "preFetchMedia"
  ],
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [ { "@odata.type": "#microsoft.graph.mediaInfo" } ],
  "removeFromDefaultAudioGroup": true
}
```

## <a name="example"></a><span data-ttu-id="bb696-119">Пример</span><span class="sxs-lookup"><span data-stu-id="bb696-119">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [
    {
      "uri": "https://cdn.contoso.com/beep.wav",
      "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
    },
    {
      "uri": "https://cdn.contoso.com/cool.wav",
      "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088F"
    }
  ],
  "removeFromDefaultAudioGroup": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
