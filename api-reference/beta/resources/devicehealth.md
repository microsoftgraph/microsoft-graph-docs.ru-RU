---
title: Тип ресурса Девицехеалс
description: Представляет работоспособность устройства, включая все ошибки.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7da256308ee63607d7d2d0e7ba62cb3030db4835
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049858"
---
# <a name="devicehealth-resource-type"></a><span data-ttu-id="8bd18-103">Тип ресурса Девицехеалс</span><span class="sxs-lookup"><span data-stu-id="8bd18-103">deviceHealth resource type</span></span>

<span data-ttu-id="8bd18-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bd18-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bd18-105">Представляет работоспособность устройства, включая все ошибки.</span><span class="sxs-lookup"><span data-stu-id="8bd18-105">Represents a device's health, including any errors.</span></span>

## <a name="properties"></a><span data-ttu-id="8bd18-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8bd18-106">Properties</span></span>
| <span data-ttu-id="8bd18-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bd18-107">Property</span></span>     | <span data-ttu-id="8bd18-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8bd18-108">Type</span></span>        | <span data-ttu-id="8bd18-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8bd18-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8bd18-110">ластконнектионтиме</span><span class="sxs-lookup"><span data-stu-id="8bd18-110">lastConnectionTime</span></span>|<span data-ttu-id="8bd18-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bd18-111">DateTimeOffset</span></span>|<span data-ttu-id="8bd18-112">Время последнего подключения устройства.</span><span class="sxs-lookup"><span data-stu-id="8bd18-112">The last time the device was connected.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8bd18-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8bd18-113">JSON representation</span></span>

<span data-ttu-id="8bd18-114">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bd18-114">The following is a JSON representation of the resource.</span></span>

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

