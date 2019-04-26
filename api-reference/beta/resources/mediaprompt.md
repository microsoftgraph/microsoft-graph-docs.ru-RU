---
title: Тип ресурса Медиапромпт
description: Тип Медиапромпт.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: aa08436d46777b4e82712e3288ec17047c33a1ff
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342634"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="bde63-103">Тип ресурса Медиапромпт</span><span class="sxs-lookup"><span data-stu-id="bde63-103">mediaPrompt resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bde63-104">Тип Медиапромпт.</span><span class="sxs-lookup"><span data-stu-id="bde63-104">The mediaPrompt type.</span></span>

## <a name="properties"></a><span data-ttu-id="bde63-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="bde63-105">Properties</span></span>

| <span data-ttu-id="bde63-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="bde63-106">Property</span></span>    | <span data-ttu-id="bde63-107">Тип</span><span class="sxs-lookup"><span data-stu-id="bde63-107">Type</span></span>                      | <span data-ttu-id="bde63-108">Описание</span><span class="sxs-lookup"><span data-stu-id="bde63-108">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="bde63-109">CNAME</span><span class="sxs-lookup"><span data-stu-id="bde63-109">loop</span></span>        | <span data-ttu-id="bde63-110">Int32</span><span class="sxs-lookup"><span data-stu-id="bde63-110">Int32</span></span>                     | <span data-ttu-id="bde63-111">Число циклов.</span><span class="sxs-lookup"><span data-stu-id="bde63-111">The loop count.</span></span> <span data-ttu-id="bde63-112">значение 0 указывает, что цикл должен быть бесконечным.</span><span class="sxs-lookup"><span data-stu-id="bde63-112">0 value indicates to loop infinitely.</span></span> <span data-ttu-id="bde63-113">Значение по умолчанию — `1`.</span><span class="sxs-lookup"><span data-stu-id="bde63-113">The default value is `1`.</span></span> |
| <span data-ttu-id="bde63-114">Медиаинфо</span><span class="sxs-lookup"><span data-stu-id="bde63-114">mediaInfo</span></span>   | [<span data-ttu-id="bde63-115">Медиаинфо</span><span class="sxs-lookup"><span data-stu-id="bde63-115">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="bde63-116">Сведения о мультимедиа</span><span class="sxs-lookup"><span data-stu-id="bde63-116">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="bde63-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bde63-117">JSON representation</span></span>

<span data-ttu-id="bde63-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bde63-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "loop": 1024,
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

## <a name="example"></a><span data-ttu-id="bde63-119">Пример</span><span class="sxs-lookup"><span data-stu-id="bde63-119">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->
```json
{
  "mediaInfo": {
    "uri": "https://cdn.contoso.com/beep.wav",
    "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
  },
  "loop": 5
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
