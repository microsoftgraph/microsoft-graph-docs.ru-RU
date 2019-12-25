---
title: Тип ресурса Медиаконфиг
description: Абстрактный базовый класс, который содержит конфигурацию мультимедиа, используемую для подключения к вызову.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0f47ac0986107af16640208d64190da6138805d5
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866716"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="ffcb5-103">Тип ресурса Медиаконфиг</span><span class="sxs-lookup"><span data-stu-id="ffcb5-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffcb5-104">Абстрактный базовый класс, который содержит конфигурацию мультимедиа, используемую для подключения к вызову.</span><span class="sxs-lookup"><span data-stu-id="ffcb5-104">An abstract base class that contains the media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="ffcb5-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ffcb5-105">Properties</span></span>

| <span data-ttu-id="ffcb5-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ffcb5-106">Property</span></span>       | <span data-ttu-id="ffcb5-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ffcb5-107">Type</span></span>    | <span data-ttu-id="ffcb5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ffcb5-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ffcb5-109">ремовефромдефаултаудиограуп</span><span class="sxs-lookup"><span data-stu-id="ffcb5-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="ffcb5-110">Логический</span><span class="sxs-lookup"><span data-stu-id="ffcb5-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="ffcb5-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ffcb5-111">JSON representation</span></span>

<span data-ttu-id="ffcb5-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffcb5-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
   ],
  "abstract": true,
  "@odata.type": "microsoft.graph.mediaConfig"
}-->
```json
{
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
