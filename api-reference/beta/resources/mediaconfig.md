---
title: Тип ресурса mediaConfig
description: Конфигурация мультимедиа, используемый для подключения к звонку.
author: VinodRavichandran
ms.openlocfilehash: 1b68d9236ba78ae1a83228b3382c96fc81516d1f
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380263"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="460e9-103">Тип ресурса mediaConfig</span><span class="sxs-lookup"><span data-stu-id="460e9-103">mediaConfig resource type</span></span>

> <span data-ttu-id="460e9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="460e9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="460e9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="460e9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="460e9-106">Конфигурация мультимедиа, используемый для подключения к звонку.</span><span class="sxs-lookup"><span data-stu-id="460e9-106">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="460e9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="460e9-107">Properties</span></span>

| <span data-ttu-id="460e9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="460e9-108">Property</span></span>       | <span data-ttu-id="460e9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="460e9-109">Type</span></span>    | <span data-ttu-id="460e9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="460e9-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="460e9-111">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="460e9-111">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="460e9-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="460e9-112">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="460e9-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="460e9-113">JSON representation</span></span>

<span data-ttu-id="460e9-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="460e9-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "removeFromDefaultAudioGroup"
  ],
  "@odata.type": "microsoft.graph.mediaConfig"
}-->
```json
{
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->