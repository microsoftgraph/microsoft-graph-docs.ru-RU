---
title: Тип ресурса Сервицехостедмедиаконфиг
description: Тип Сервицехостедмедиаконфиг.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fbd59694940d6d0b3abea1a8d56bd426a3dfbb3a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343306"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="92a5c-103">Тип ресурса Сервицехостедмедиаконфиг</span><span class="sxs-lookup"><span data-stu-id="92a5c-103">serviceHostedMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92a5c-104">Тип Сервицехостедмедиаконфиг.</span><span class="sxs-lookup"><span data-stu-id="92a5c-104">The serviceHostedMediaConfig type.</span></span>

## <a name="properties"></a><span data-ttu-id="92a5c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="92a5c-105">Properties</span></span>

| <span data-ttu-id="92a5c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="92a5c-106">Property</span></span>                    | <span data-ttu-id="92a5c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="92a5c-107">Type</span></span>                                                        | <span data-ttu-id="92a5c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="92a5c-108">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="92a5c-109">Префетчмедиа</span><span class="sxs-lookup"><span data-stu-id="92a5c-109">preFetchMedia</span></span>               | <span data-ttu-id="92a5c-110">Коллекция [медиаинфо](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="92a5c-110">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="92a5c-111">Список носителей для предварительной загрузки.</span><span class="sxs-lookup"><span data-stu-id="92a5c-111">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="92a5c-112">Ремовефромдефаултаудиограуп</span><span class="sxs-lookup"><span data-stu-id="92a5c-112">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="92a5c-113">Логический</span><span class="sxs-lookup"><span data-stu-id="92a5c-113">Boolean</span></span>                                                     | <span data-ttu-id="92a5c-114">Удаление самостоятельного участника из группы "звук" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="92a5c-114">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="92a5c-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92a5c-115">JSON representation</span></span>

<span data-ttu-id="92a5c-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92a5c-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "preFetchMedia"
  ],
  "baseType": "microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [ { "@odata.type": "microsoft.graph.mediaInfo" } ],
  "removeFromDefaultAudioGroup": true
}
```

## <a name="example"></a><span data-ttu-id="92a5c-117">Пример</span><span class="sxs-lookup"><span data-stu-id="92a5c-117">Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "serviceHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
