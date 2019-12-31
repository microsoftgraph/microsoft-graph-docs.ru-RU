---
title: Тип ресурса Медиаконфиг
description: Абстрактный базовый класс, который содержит конфигурацию мультимедиа, используемую для подключения к вызову.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 61fe1dfcc4c2c9b686a61d22e55ddae3c80661be
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913305"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="4295a-103">Тип ресурса Медиаконфиг</span><span class="sxs-lookup"><span data-stu-id="4295a-103">mediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4295a-104">Абстрактный базовый класс, который содержит конфигурацию мультимедиа, используемую для подключения к вызову.</span><span class="sxs-lookup"><span data-stu-id="4295a-104">An abstract base class that contains the media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="4295a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4295a-105">Properties</span></span>

| <span data-ttu-id="4295a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4295a-106">Property</span></span>       | <span data-ttu-id="4295a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4295a-107">Type</span></span>    | <span data-ttu-id="4295a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4295a-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4295a-109">ремовефромдефаултаудиограуп</span><span class="sxs-lookup"><span data-stu-id="4295a-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="4295a-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="4295a-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="4295a-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4295a-111">JSON representation</span></span>

<span data-ttu-id="4295a-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4295a-112">The following is a JSON representation of the resource.</span></span>

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
