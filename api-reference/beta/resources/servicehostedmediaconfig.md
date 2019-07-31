---
title: Тип ресурса Сервицехостедмедиаконфиг
description: Тип Сервицехостедмедиаконфиг.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f56928a7294fba1cb31f5061a2c7b8f7bb70f02a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965203"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="b0a6d-103">Тип ресурса Сервицехостедмедиаконфиг</span><span class="sxs-lookup"><span data-stu-id="b0a6d-103">serviceHostedMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0a6d-104">Тип Сервицехостедмедиаконфиг.</span><span class="sxs-lookup"><span data-stu-id="b0a6d-104">The serviceHostedMediaConfig type.</span></span>

## <a name="properties"></a><span data-ttu-id="b0a6d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0a6d-105">Properties</span></span>

| <span data-ttu-id="b0a6d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0a6d-106">Property</span></span>                    | <span data-ttu-id="b0a6d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b0a6d-107">Type</span></span>                                                        | <span data-ttu-id="b0a6d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b0a6d-108">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="b0a6d-109">Префетчмедиа</span><span class="sxs-lookup"><span data-stu-id="b0a6d-109">preFetchMedia</span></span>               | <span data-ttu-id="b0a6d-110">Коллекция [медиаинфо](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="b0a6d-110">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="b0a6d-111">Список носителей для предварительной загрузки.</span><span class="sxs-lookup"><span data-stu-id="b0a6d-111">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="b0a6d-112">Ремовефромдефаултаудиограуп</span><span class="sxs-lookup"><span data-stu-id="b0a6d-112">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="b0a6d-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a6d-113">Boolean</span></span>                                                     | <span data-ttu-id="b0a6d-114">Удаление самостоятельного участника из группы "звук" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b0a6d-114">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b0a6d-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0a6d-115">JSON representation</span></span>

<span data-ttu-id="b0a6d-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0a6d-116">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="b0a6d-117">Пример</span><span class="sxs-lookup"><span data-stu-id="b0a6d-117">Example</span></span>

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
