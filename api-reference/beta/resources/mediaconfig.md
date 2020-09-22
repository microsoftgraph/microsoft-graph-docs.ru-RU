---
title: Тип ресурса Медиаконфиг
description: Абстрактный базовый класс, который содержит конфигурацию мультимедиа, используемую для подключения к вызову.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 05f93ff0776795d988b66ad84c98af1d5f5bede2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971757"
---
# <a name="mediaconfig-resource-type"></a><span data-ttu-id="26ce6-103">Тип ресурса Медиаконфиг</span><span class="sxs-lookup"><span data-stu-id="26ce6-103">mediaConfig resource type</span></span>

<span data-ttu-id="26ce6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26ce6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26ce6-105">Абстрактный базовый класс, который содержит конфигурацию мультимедиа, используемую для подключения к вызову.</span><span class="sxs-lookup"><span data-stu-id="26ce6-105">An abstract base class that contains the media configuration used to connect to a call.</span></span>

## <a name="properties"></a><span data-ttu-id="26ce6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="26ce6-106">Properties</span></span>

| <span data-ttu-id="26ce6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="26ce6-107">Property</span></span>       | <span data-ttu-id="26ce6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="26ce6-108">Type</span></span>    | <span data-ttu-id="26ce6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="26ce6-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="26ce6-110">ремовефромдефаултаудиограуп</span><span class="sxs-lookup"><span data-stu-id="26ce6-110">removeFromDefaultAudioGroup</span></span> | <span data-ttu-id="26ce6-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="26ce6-111">Boolean</span></span> |  |

## <a name="json-representation"></a><span data-ttu-id="26ce6-112">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="26ce6-112">JSON representation</span></span>

<span data-ttu-id="26ce6-113">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26ce6-113">The following is a JSON representation of the resource.</span></span>

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


