---
title: тип ресурса timeClockSettings
description: Представляет параметры времени для расписания.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 96ffddc0730ffaff73d21a8ab051acf9ea140ccc
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786391"
---
# <a name="timeclocksettings-resource-type"></a><span data-ttu-id="432b5-103">тип ресурса timeClockSettings</span><span class="sxs-lookup"><span data-stu-id="432b5-103">timeClockSettings resource type</span></span>

<span data-ttu-id="432b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="432b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="432b5-105">Представляет параметры времени для [расписания.](schedule.md)</span><span class="sxs-lookup"><span data-stu-id="432b5-105">Represents timeclock settings for a [schedule](schedule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="432b5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="432b5-106">Properties</span></span>
|<span data-ttu-id="432b5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="432b5-107">Property</span></span>               |<span data-ttu-id="432b5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="432b5-108">Type</span></span>           |<span data-ttu-id="432b5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="432b5-109">Description</span></span>                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| <span data-ttu-id="432b5-110">approvedLocation</span><span class="sxs-lookup"><span data-stu-id="432b5-110">approvedLocation</span></span> | [<span data-ttu-id="432b5-111">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="432b5-111">geoCoordinates</span></span>](geocoordinates.md)  |<span data-ttu-id="432b5-112">Aprroved location of the **timeClock**.</span><span class="sxs-lookup"><span data-stu-id="432b5-112">The aprroved location of the **timeClock**.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="432b5-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="432b5-113">JSON representation</span></span>

<span data-ttu-id="432b5-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="432b5-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeClockSettings"
}-->
```json
{ 
   "approvedLocation": {

           "altitude": {"@odata.type": "microsoft.graph.GeoCoordinates"},

           "latitude": {"@odata.type": "microsoft.graph.GeoCoordinates"},

           "longitude": {"@odata.type": "microsoft.graph.GeoCoordinates"}

        }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeClockSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
