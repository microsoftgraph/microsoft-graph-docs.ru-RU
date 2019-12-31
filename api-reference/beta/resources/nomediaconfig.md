---
title: Тип ресурса Номедиаконфиг
description: Конфигурация мультимедиа, указывающая на отсутствие носителя.
author: ananmishr
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e916c0498a3a8fffd09dd4b86d7b7ec3ab4b9a08
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913676"
---
# <a name="nomediaconfig-resource-type"></a><span data-ttu-id="8fccb-103">Тип ресурса Номедиаконфиг</span><span class="sxs-lookup"><span data-stu-id="8fccb-103">noMediaConfig resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fccb-104">Конфигурация мультимедиа, указывающая на отсутствие носителя.</span><span class="sxs-lookup"><span data-stu-id="8fccb-104">Media configuration for indicating no media.</span></span>

## <a name="properties"></a><span data-ttu-id="8fccb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8fccb-105">Properties</span></span>

| <span data-ttu-id="8fccb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8fccb-106">Property</span></span>       | <span data-ttu-id="8fccb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8fccb-107">Type</span></span>    | <span data-ttu-id="8fccb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8fccb-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8fccb-109">ремовефромдефаултаудиограуп</span><span class="sxs-lookup"><span data-stu-id="8fccb-109">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="8fccb-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fccb-110">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="8fccb-111">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8fccb-111">JSON representation</span></span>

<span data-ttu-id="8fccb-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8fccb-112">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.noMediaConfig"
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
  "description": "noMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
