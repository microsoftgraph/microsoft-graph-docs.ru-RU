---
title: Тип ресурса Сервицехостедмедиаконфиг
description: Удаленно размещенный носитель.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 405f6b40260908d7492a3b02c8535588c8475ca8
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870091"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="6f057-103">Тип ресурса Сервицехостедмедиаконфиг</span><span class="sxs-lookup"><span data-stu-id="6f057-103">serviceHostedMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f057-104">Удаленно размещенный носитель.</span><span class="sxs-lookup"><span data-stu-id="6f057-104">The media that's hosted remotely.</span></span> <span data-ttu-id="6f057-105">Это наследуется от [медиаконфиг](mediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="6f057-105">This is inherited from [mediaConfig](mediaconfig.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6f057-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f057-106">Properties</span></span>

| <span data-ttu-id="6f057-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f057-107">Property</span></span>                    | <span data-ttu-id="6f057-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6f057-108">Type</span></span>                                                        | <span data-ttu-id="6f057-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6f057-109">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="6f057-110">префетчмедиа</span><span class="sxs-lookup"><span data-stu-id="6f057-110">preFetchMedia</span></span>               | <span data-ttu-id="6f057-111">Коллекция [медиаинфо](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="6f057-111">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="6f057-112">Список носителей для предварительной загрузки.</span><span class="sxs-lookup"><span data-stu-id="6f057-112">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="6f057-113">ремовефромдефаултаудиограуп</span><span class="sxs-lookup"><span data-stu-id="6f057-113">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="6f057-114">Логический</span><span class="sxs-lookup"><span data-stu-id="6f057-114">Boolean</span></span>                                                     | <span data-ttu-id="6f057-115">Удаление самостоятельного участника из группы "звук" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6f057-115">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6f057-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f057-116">JSON representation</span></span>

<span data-ttu-id="6f057-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f057-117">The following is a JSON representation of the resource.</span></span>

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
