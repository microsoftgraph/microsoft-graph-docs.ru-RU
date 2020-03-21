---
title: Тип ресурса Девицехеалс
description: Представляет работоспособность устройства, включая все ошибки.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: efd8b1e7722eabcacd05512b0101735d677d9b89
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896119"
---
# <a name="devicehealth-resource-type"></a><span data-ttu-id="94901-103">Тип ресурса Девицехеалс</span><span class="sxs-lookup"><span data-stu-id="94901-103">deviceHealth resource type</span></span>

<span data-ttu-id="94901-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94901-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94901-105">Представляет работоспособность устройства, включая все ошибки.</span><span class="sxs-lookup"><span data-stu-id="94901-105">Represents a device's health, including any errors.</span></span>

## <a name="properties"></a><span data-ttu-id="94901-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="94901-106">Properties</span></span>
| <span data-ttu-id="94901-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="94901-107">Property</span></span>     | <span data-ttu-id="94901-108">Тип</span><span class="sxs-lookup"><span data-stu-id="94901-108">Type</span></span>        | <span data-ttu-id="94901-109">Описание</span><span class="sxs-lookup"><span data-stu-id="94901-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="94901-110">ластконнектионтиме</span><span class="sxs-lookup"><span data-stu-id="94901-110">lastConnectionTime</span></span>|<span data-ttu-id="94901-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94901-111">DateTimeOffset</span></span>|<span data-ttu-id="94901-112">Время последнего подключения устройства.</span><span class="sxs-lookup"><span data-stu-id="94901-112">The last time the device was connected.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94901-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="94901-113">JSON representation</span></span>

<span data-ttu-id="94901-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94901-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceHealth"
}-->

```json
{
    "lastConnectionTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceHealth resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->