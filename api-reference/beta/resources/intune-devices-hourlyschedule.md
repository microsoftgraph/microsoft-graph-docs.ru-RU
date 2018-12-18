---
title: Тип ресурса hourlySchedule
description: Каждый час запустите расписание для повторяющихся сценарий управления устройства.
author: tfitzmac
ms.openlocfilehash: e73ff542b7de780d16d9f2bd76c11c2d0f92e8ae
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317579"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="f2d18-103">Тип ресурса hourlySchedule</span><span class="sxs-lookup"><span data-stu-id="f2d18-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="f2d18-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f2d18-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2d18-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2d18-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2d18-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f2d18-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2d18-107">Каждый час запустите расписание для повторяющихся сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="f2d18-107">Hourly run schedule of a recurring device management script.</span></span>

<span data-ttu-id="f2d18-108">Наследуется от [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="f2d18-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f2d18-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2d18-109">Properties</span></span>
|<span data-ttu-id="f2d18-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2d18-110">Property</span></span>|<span data-ttu-id="f2d18-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f2d18-111">Type</span></span>|<span data-ttu-id="f2d18-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f2d18-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2d18-113">interval</span><span class="sxs-lookup"><span data-stu-id="f2d18-113">interval</span></span>|<span data-ttu-id="f2d18-114">Int32</span><span class="sxs-lookup"><span data-stu-id="f2d18-114">Int32</span></span>|<span data-ttu-id="f2d18-115">Интервал в часах</span><span class="sxs-lookup"><span data-stu-id="f2d18-115">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2d18-116">Связи</span><span class="sxs-lookup"><span data-stu-id="f2d18-116">Relationships</span></span>
<span data-ttu-id="f2d18-117">Нет</span><span class="sxs-lookup"><span data-stu-id="f2d18-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f2d18-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2d18-118">JSON Representation</span></span>
<span data-ttu-id="f2d18-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2d18-119">Here is a JSON representation of the resource.</span></span>
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





