---
title: Тип ресурса Сервицехостедмедиаконфиг
description: Удаленно размещенный носитель.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d006a4417401859c0c385f9537656993f985198d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023958"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="67c6e-103">Тип ресурса Сервицехостедмедиаконфиг</span><span class="sxs-lookup"><span data-stu-id="67c6e-103">serviceHostedMediaConfig resource type</span></span>

<span data-ttu-id="67c6e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67c6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67c6e-105">Удаленно размещенный носитель.</span><span class="sxs-lookup"><span data-stu-id="67c6e-105">The media that's hosted remotely.</span></span> <span data-ttu-id="67c6e-106">Это наследуется от [медиаконфиг](mediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="67c6e-106">This is inherited from [mediaConfig](mediaconfig.md).</span></span>

## <a name="properties"></a><span data-ttu-id="67c6e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="67c6e-107">Properties</span></span>

| <span data-ttu-id="67c6e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="67c6e-108">Property</span></span>                    | <span data-ttu-id="67c6e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="67c6e-109">Type</span></span>                                                        | <span data-ttu-id="67c6e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="67c6e-110">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="67c6e-111">префетчмедиа</span><span class="sxs-lookup"><span data-stu-id="67c6e-111">preFetchMedia</span></span>               | <span data-ttu-id="67c6e-112">Коллекция [медиаинфо](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="67c6e-112">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="67c6e-113">Список носителей для предварительной загрузки.</span><span class="sxs-lookup"><span data-stu-id="67c6e-113">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="67c6e-114">ремовефромдефаултаудиограуп</span><span class="sxs-lookup"><span data-stu-id="67c6e-114">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="67c6e-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="67c6e-115">Boolean</span></span>                                                     | <span data-ttu-id="67c6e-116">Удаление самостоятельного участника из группы "звук" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="67c6e-116">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="67c6e-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67c6e-117">JSON representation</span></span>

<span data-ttu-id="67c6e-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67c6e-118">The following is a JSON representation of the resource.</span></span>

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


