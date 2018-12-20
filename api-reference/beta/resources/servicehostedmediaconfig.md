---
title: Тип ресурса serviceHostedMediaConfig
description: Тип serviceHostedMediaConfig.
author: VinodRavichandran
ms.openlocfilehash: 544c1d3bce934064092e0f9c74b888686e49d426
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380319"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="ae8ed-103">Тип ресурса serviceHostedMediaConfig</span><span class="sxs-lookup"><span data-stu-id="ae8ed-103">serviceHostedMediaConfig resource type</span></span>

> <span data-ttu-id="ae8ed-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ae8ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae8ed-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae8ed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae8ed-106">Тип serviceHostedMediaConfig.</span><span class="sxs-lookup"><span data-stu-id="ae8ed-106">The serviceHostedMediaConfig type.</span></span>

## <a name="properties"></a><span data-ttu-id="ae8ed-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae8ed-107">Properties</span></span>

| <span data-ttu-id="ae8ed-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae8ed-108">Property</span></span>                    | <span data-ttu-id="ae8ed-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ae8ed-109">Type</span></span>                                                        | <span data-ttu-id="ae8ed-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ae8ed-110">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="ae8ed-111">preFetchMedia</span><span class="sxs-lookup"><span data-stu-id="ae8ed-111">preFetchMedia</span></span>               | <span data-ttu-id="ae8ed-112">[mediaInfo](mediainfo.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ae8ed-112">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="ae8ed-113">Список мультимедиа для предварительно выборки.</span><span class="sxs-lookup"><span data-stu-id="ae8ed-113">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="ae8ed-114">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="ae8ed-114">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="ae8ed-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae8ed-115">Boolean</span></span>                                                     | <span data-ttu-id="ae8ed-116">Удалите собственный участника из группы по умолчанию звука.</span><span class="sxs-lookup"><span data-stu-id="ae8ed-116">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ae8ed-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae8ed-117">JSON representation</span></span>

<span data-ttu-id="ae8ed-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae8ed-118">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="ae8ed-119">Пример</span><span class="sxs-lookup"><span data-stu-id="ae8ed-119">Example</span></span>

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
