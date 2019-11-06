---
title: Тип ресурса Сервицехостедмедиаконфиг
description: Тип Сервицехостедмедиаконфиг.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: edefba3e415a50322022e4549fbecbd37da6d1da
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006545"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="29e84-103">Тип ресурса Сервицехостедмедиаконфиг</span><span class="sxs-lookup"><span data-stu-id="29e84-103">serviceHostedMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29e84-104">Тип Сервицехостедмедиаконфиг.</span><span class="sxs-lookup"><span data-stu-id="29e84-104">The serviceHostedMediaConfig type.</span></span>

## <a name="properties"></a><span data-ttu-id="29e84-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="29e84-105">Properties</span></span>

| <span data-ttu-id="29e84-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="29e84-106">Property</span></span>                    | <span data-ttu-id="29e84-107">Тип</span><span class="sxs-lookup"><span data-stu-id="29e84-107">Type</span></span>                                                        | <span data-ttu-id="29e84-108">Описание</span><span class="sxs-lookup"><span data-stu-id="29e84-108">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="29e84-109">префетчмедиа</span><span class="sxs-lookup"><span data-stu-id="29e84-109">preFetchMedia</span></span>               | <span data-ttu-id="29e84-110">Коллекция [медиаинфо](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="29e84-110">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="29e84-111">Список носителей для предварительной загрузки.</span><span class="sxs-lookup"><span data-stu-id="29e84-111">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="29e84-112">ремовефромдефаултаудиограуп</span><span class="sxs-lookup"><span data-stu-id="29e84-112">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="29e84-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="29e84-113">Boolean</span></span>                                                     | <span data-ttu-id="29e84-114">Удаление самостоятельного участника из группы "звук" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="29e84-114">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="29e84-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="29e84-115">JSON representation</span></span>

<span data-ttu-id="29e84-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29e84-116">The following is a JSON representation of the resource.</span></span>

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
