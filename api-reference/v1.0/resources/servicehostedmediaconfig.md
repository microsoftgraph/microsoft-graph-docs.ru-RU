---
title: Тип ресурса Сервицехостедмедиаконфиг
description: Тип Сервицехостедмедиаконфиг.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d4bdea6009dae0bd06ec9ffc00d00e417e7c22d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991847"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="bd709-103">Тип ресурса Сервицехостедмедиаконфиг</span><span class="sxs-lookup"><span data-stu-id="bd709-103">serviceHostedMediaConfig resource type</span></span>

<span data-ttu-id="bd709-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd709-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bd709-105">Удаленно размещенный носитель.</span><span class="sxs-lookup"><span data-stu-id="bd709-105">The media that's hosted remotely.</span></span> <span data-ttu-id="bd709-106">Это наследуется от [медиаконфиг](mediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="bd709-106">This is inherited from [mediaConfig](mediaconfig.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bd709-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd709-107">Properties</span></span>

| <span data-ttu-id="bd709-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd709-108">Property</span></span>                    | <span data-ttu-id="bd709-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bd709-109">Type</span></span>                                                        | <span data-ttu-id="bd709-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bd709-110">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="bd709-111">префетчмедиа</span><span class="sxs-lookup"><span data-stu-id="bd709-111">preFetchMedia</span></span>               | <span data-ttu-id="bd709-112">Коллекция [медиаинфо](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="bd709-112">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="bd709-113">Список носителей для предварительной загрузки.</span><span class="sxs-lookup"><span data-stu-id="bd709-113">The list of media to pre-fetch.</span></span>                   |


## <a name="json-representation"></a><span data-ttu-id="bd709-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd709-114">JSON representation</span></span>

<span data-ttu-id="bd709-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd709-115">The following is a JSON representation of the resource.</span></span>

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

