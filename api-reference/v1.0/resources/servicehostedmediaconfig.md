---
title: Тип ресурса Сервицехостедмедиаконфиг
description: Тип Сервицехостедмедиаконфиг.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 590eef4c572695188e609133f5bc852fd90c51f7
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866253"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="f4452-103">Тип ресурса Сервицехостедмедиаконфиг</span><span class="sxs-lookup"><span data-stu-id="f4452-103">serviceHostedMediaConfig resource type</span></span>

<span data-ttu-id="f4452-104">Удаленно размещенный носитель.</span><span class="sxs-lookup"><span data-stu-id="f4452-104">The media that's hosted remotely.</span></span> <span data-ttu-id="f4452-105">Это наследуется от [медиаконфиг](mediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="f4452-105">This is inherited from [mediaConfig](mediaconfig.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f4452-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4452-106">Properties</span></span>

| <span data-ttu-id="f4452-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4452-107">Property</span></span>                    | <span data-ttu-id="f4452-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f4452-108">Type</span></span>                                                        | <span data-ttu-id="f4452-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f4452-109">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="f4452-110">префетчмедиа</span><span class="sxs-lookup"><span data-stu-id="f4452-110">preFetchMedia</span></span>               | <span data-ttu-id="f4452-111">Коллекция [медиаинфо](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="f4452-111">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="f4452-112">Список носителей для предварительной загрузки.</span><span class="sxs-lookup"><span data-stu-id="f4452-112">The list of media to pre-fetch.</span></span>                   |


## <a name="json-representation"></a><span data-ttu-id="f4452-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4452-113">JSON representation</span></span>

<span data-ttu-id="f4452-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4452-114">The following is a JSON representation of the resource.</span></span>

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
  "preFetchMedia": [ { "@odata.type": "microsoft.graph.mediaInfo" } ]
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
