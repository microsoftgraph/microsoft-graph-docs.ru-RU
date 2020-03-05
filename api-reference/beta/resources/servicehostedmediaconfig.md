---
title: Тип ресурса Сервицехостедмедиаконфиг
description: Удаленно размещенный носитель.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 16db7e17e48ce8f257d9b6a1bfd296ca06bd0634
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520796"
---
# <a name="servicehostedmediaconfig-resource-type"></a><span data-ttu-id="f70bc-103">Тип ресурса Сервицехостедмедиаконфиг</span><span class="sxs-lookup"><span data-stu-id="f70bc-103">serviceHostedMediaConfig resource type</span></span>

<span data-ttu-id="f70bc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f70bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f70bc-105">Удаленно размещенный носитель.</span><span class="sxs-lookup"><span data-stu-id="f70bc-105">The media that's hosted remotely.</span></span> <span data-ttu-id="f70bc-106">Это наследуется от [медиаконфиг](mediaconfig.md).</span><span class="sxs-lookup"><span data-stu-id="f70bc-106">This is inherited from [mediaConfig](mediaconfig.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f70bc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f70bc-107">Properties</span></span>

| <span data-ttu-id="f70bc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f70bc-108">Property</span></span>                    | <span data-ttu-id="f70bc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f70bc-109">Type</span></span>                                                        | <span data-ttu-id="f70bc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f70bc-110">Description</span></span>                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| <span data-ttu-id="f70bc-111">префетчмедиа</span><span class="sxs-lookup"><span data-stu-id="f70bc-111">preFetchMedia</span></span>               | <span data-ttu-id="f70bc-112">Коллекция [медиаинфо](mediainfo.md)</span><span class="sxs-lookup"><span data-stu-id="f70bc-112">[mediaInfo](mediainfo.md) collection</span></span>                        | <span data-ttu-id="f70bc-113">Список носителей для предварительной загрузки.</span><span class="sxs-lookup"><span data-stu-id="f70bc-113">The list of media to pre-fetch.</span></span>                   |
| <span data-ttu-id="f70bc-114">ремовефромдефаултаудиограуп</span><span class="sxs-lookup"><span data-stu-id="f70bc-114">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="f70bc-115">Логический</span><span class="sxs-lookup"><span data-stu-id="f70bc-115">Boolean</span></span>                                                     | <span data-ttu-id="f70bc-116">Удаление самостоятельного участника из группы "звук" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f70bc-116">Remove self participant from default audio group.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f70bc-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f70bc-117">JSON representation</span></span>

<span data-ttu-id="f70bc-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f70bc-118">The following is a JSON representation of the resource.</span></span>

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
