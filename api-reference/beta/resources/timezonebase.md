---
title: Тип ресурса timeZoneBase
description: Основное представление часового пояса.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 95347a76ff5622f1e93d6e4c61a6ab050c302db9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519689"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="004b4-103">Тип ресурса timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="004b4-103">timeZoneBase resource type</span></span>

<span data-ttu-id="004b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="004b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="004b4-105">Основное представление часового пояса.</span><span class="sxs-lookup"><span data-stu-id="004b4-105">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="004b4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="004b4-106">Properties</span></span>
| <span data-ttu-id="004b4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="004b4-107">Property</span></span>     | <span data-ttu-id="004b4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="004b4-108">Type</span></span>   |<span data-ttu-id="004b4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="004b4-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="004b4-110">name</span><span class="sxs-lookup"><span data-stu-id="004b4-110">name</span></span> | <span data-ttu-id="004b4-111">string</span><span class="sxs-lookup"><span data-stu-id="004b4-111">string</span></span> | <span data-ttu-id="004b4-112">Имя часового пояса</span><span class="sxs-lookup"><span data-stu-id="004b4-112">The name of a time zone.</span></span> <span data-ttu-id="004b4-113">(стандартного, например "Гавайско-Алеутское время (зима)" или особого, например "Особый часовой пояс").</span><span class="sxs-lookup"><span data-stu-id="004b4-113">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="004b4-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="004b4-114">JSON representation</span></span>

<span data-ttu-id="004b4-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="004b4-115">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
