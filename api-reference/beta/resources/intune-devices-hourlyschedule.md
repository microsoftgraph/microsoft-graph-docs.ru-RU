---
title: Тип ресурса hourlySchedule
description: Каждый час запустите расписание для повторяющихся сценарий управления устройства.
ms.openlocfilehash: 1161f7dfc3d74224c22075db8eff83b7f412b9b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079635"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="c1cdd-103">Тип ресурса hourlySchedule</span><span class="sxs-lookup"><span data-stu-id="c1cdd-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="c1cdd-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c1cdd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1cdd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1cdd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1cdd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c1cdd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1cdd-107">Каждый час запустите расписание для повторяющихся сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="c1cdd-107">Hourly run schedule of a recurring device management script.</span></span>

<span data-ttu-id="c1cdd-108">Наследуется от [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="c1cdd-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c1cdd-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1cdd-109">Properties</span></span>
|<span data-ttu-id="c1cdd-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1cdd-110">Property</span></span>|<span data-ttu-id="c1cdd-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c1cdd-111">Type</span></span>|<span data-ttu-id="c1cdd-112">Description</span><span class="sxs-lookup"><span data-stu-id="c1cdd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1cdd-113">interval</span><span class="sxs-lookup"><span data-stu-id="c1cdd-113">interval</span></span>|<span data-ttu-id="c1cdd-114">Int32</span><span class="sxs-lookup"><span data-stu-id="c1cdd-114">Int32</span></span>|<span data-ttu-id="c1cdd-115">Интервал в часах</span><span class="sxs-lookup"><span data-stu-id="c1cdd-115">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1cdd-116">Связи</span><span class="sxs-lookup"><span data-stu-id="c1cdd-116">Relationships</span></span>
<span data-ttu-id="c1cdd-117">Нет</span><span class="sxs-lookup"><span data-stu-id="c1cdd-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c1cdd-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1cdd-118">JSON Representation</span></span>
<span data-ttu-id="c1cdd-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1cdd-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hourlySchedule",
  "interval": 1024
}
```





