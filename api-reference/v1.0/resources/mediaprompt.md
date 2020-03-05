---
title: Тип ресурса Медиапромпт
description: Этот тип ресурса содержит сведения о звуковом файле, который необходимо воспроизвести, и другие дополнительные параметры.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4bc2f315a2f339d2ef6fe0f4b76b335970b5a642
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447446"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="ee845-103">Тип ресурса Медиапромпт</span><span class="sxs-lookup"><span data-stu-id="ee845-103">mediaPrompt resource type</span></span>

<span data-ttu-id="ee845-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ee845-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee845-105">Этот тип ресурса содержит сведения о звуковом файле, который необходимо воспроизвести, и другие дополнительные параметры.</span><span class="sxs-lookup"><span data-stu-id="ee845-105">This resource type contains information about the audio file to be played and other additional settings.</span></span>

## <a name="properties"></a><span data-ttu-id="ee845-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee845-106">Properties</span></span>

| <span data-ttu-id="ee845-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee845-107">Property</span></span>    | <span data-ttu-id="ee845-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ee845-108">Type</span></span>                      | <span data-ttu-id="ee845-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ee845-109">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="ee845-110">медиаинфо</span><span class="sxs-lookup"><span data-stu-id="ee845-110">mediaInfo</span></span>   | [<span data-ttu-id="ee845-111">медиаинфо</span><span class="sxs-lookup"><span data-stu-id="ee845-111">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="ee845-112">Сведения о мультимедиа</span><span class="sxs-lookup"><span data-stu-id="ee845-112">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="ee845-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee845-113">JSON representation</span></span>

<span data-ttu-id="ee845-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee845-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
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
