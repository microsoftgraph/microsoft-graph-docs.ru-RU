---
title: Тип ресурса mediaConfig
description: Конфигурация мультимедиа, используемый для подключения к звонку.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 74b3b5dc4c71db80e94216756a3513a03011572a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948921"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="7ca14-103">Тип ресурса mediaConfig</span><span class="sxs-lookup"><span data-stu-id="7ca14-103">mediaConfig resource type</span></span>

> <span data-ttu-id="7ca14-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7ca14-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ca14-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ca14-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7ca14-106">Конфигурация мультимедиа, используемый для подключения к звонку.</span><span class="sxs-lookup"><span data-stu-id="7ca14-106">The media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="7ca14-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ca14-107">Properties</span></span>

| <span data-ttu-id="7ca14-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ca14-108">Property</span></span>       | <span data-ttu-id="7ca14-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7ca14-109">Type</span></span>    | <span data-ttu-id="7ca14-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7ca14-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7ca14-111">removeFromDefaultAudioGroup</span><span class="sxs-lookup"><span data-stu-id="7ca14-111">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="7ca14-112">Логический</span><span class="sxs-lookup"><span data-stu-id="7ca14-112">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="7ca14-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ca14-113">JSON representation</span></span>

<span data-ttu-id="7ca14-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ca14-114">The following is a JSON representation of the resource.</span></span>

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
