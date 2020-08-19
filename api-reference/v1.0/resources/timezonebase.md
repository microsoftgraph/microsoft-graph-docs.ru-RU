---
title: Тип ресурса timeZoneBase
description: Основное представление часового пояса.
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e8ec3a7d71bfc767b3ea54d9b4b8626d3ca953c4
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808853"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="e8eee-103">Тип ресурса timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="e8eee-103">timeZoneBase resource type</span></span>

<span data-ttu-id="e8eee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8eee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e8eee-105">Основное представление часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e8eee-105">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="e8eee-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e8eee-106">Properties</span></span>
| <span data-ttu-id="e8eee-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8eee-107">Property</span></span>     | <span data-ttu-id="e8eee-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e8eee-108">Type</span></span>   |<span data-ttu-id="e8eee-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e8eee-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e8eee-110">name</span><span class="sxs-lookup"><span data-stu-id="e8eee-110">name</span></span> | <span data-ttu-id="e8eee-111">string</span><span class="sxs-lookup"><span data-stu-id="e8eee-111">string</span></span> | <span data-ttu-id="e8eee-112">Имя часового пояса</span><span class="sxs-lookup"><span data-stu-id="e8eee-112">The name of a time zone.</span></span> <span data-ttu-id="e8eee-113">(стандартного, например "Гавайско-Алеутское время (зима)" или особого, например "Особый часовой пояс").</span><span class="sxs-lookup"><span data-stu-id="e8eee-113">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="e8eee-114">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e8eee-114">JSON representation</span></span>

<span data-ttu-id="e8eee-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8eee-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
