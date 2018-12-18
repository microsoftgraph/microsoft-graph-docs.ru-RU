---
title: Тип ресурса dailySchedule
description: График ежедневного выполнения повторяющихся сценарий управления устройства.
author: tfitzmac
ms.openlocfilehash: 86a3dda75c0aecef6ba0672bc114092bd301a582
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351130"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="4dcff-103">Тип ресурса dailySchedule</span><span class="sxs-lookup"><span data-stu-id="4dcff-103">dailySchedule resource type</span></span>

> <span data-ttu-id="4dcff-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4dcff-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4dcff-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dcff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4dcff-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4dcff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4dcff-107">График ежедневного выполнения повторяющихся сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="4dcff-107">Daily run schedule of a recurring device management script.</span></span>

<span data-ttu-id="4dcff-108">Наследуется от [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="4dcff-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4dcff-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4dcff-109">Properties</span></span>
|<span data-ttu-id="4dcff-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4dcff-110">Property</span></span>|<span data-ttu-id="4dcff-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4dcff-111">Type</span></span>|<span data-ttu-id="4dcff-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4dcff-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dcff-113">interval</span><span class="sxs-lookup"><span data-stu-id="4dcff-113">interval</span></span>|<span data-ttu-id="4dcff-114">Int32</span><span class="sxs-lookup"><span data-stu-id="4dcff-114">Int32</span></span>|<span data-ttu-id="4dcff-115">Интервал в днях</span><span class="sxs-lookup"><span data-stu-id="4dcff-115">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="4dcff-116">Связи</span><span class="sxs-lookup"><span data-stu-id="4dcff-116">Relationships</span></span>
<span data-ttu-id="4dcff-117">Нет</span><span class="sxs-lookup"><span data-stu-id="4dcff-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4dcff-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4dcff-118">JSON Representation</span></span>
<span data-ttu-id="4dcff-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4dcff-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.dailySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dailySchedule",
  "interval": 1024
}
```





