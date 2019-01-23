---
title: Тип ресурса hourlySchedule
description: Каждый час запустите расписание для повторяющихся сценарий управления устройства.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf62c11da0932f5f10b6cc7a76ccecfd1e74ee92
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396828"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="21470-103">Тип ресурса hourlySchedule</span><span class="sxs-lookup"><span data-stu-id="21470-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="21470-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="21470-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="21470-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21470-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21470-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21470-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21470-107">Каждый час запустите расписание для повторяющихся сценарий управления устройства.</span><span class="sxs-lookup"><span data-stu-id="21470-107">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="21470-108">Наследуется от [runSchedule](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="21470-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="21470-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="21470-109">Properties</span></span>
|<span data-ttu-id="21470-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="21470-110">Property</span></span>|<span data-ttu-id="21470-111">Тип</span><span class="sxs-lookup"><span data-stu-id="21470-111">Type</span></span>|<span data-ttu-id="21470-112">Описание</span><span class="sxs-lookup"><span data-stu-id="21470-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21470-113">interval</span><span class="sxs-lookup"><span data-stu-id="21470-113">interval</span></span>|<span data-ttu-id="21470-114">Int32</span><span class="sxs-lookup"><span data-stu-id="21470-114">Int32</span></span>|<span data-ttu-id="21470-115">Интервал в часах</span><span class="sxs-lookup"><span data-stu-id="21470-115">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="21470-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="21470-116">Relationships</span></span>
<span data-ttu-id="21470-117">Нет</span><span class="sxs-lookup"><span data-stu-id="21470-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21470-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21470-118">JSON Representation</span></span>
<span data-ttu-id="21470-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21470-119">Here is a JSON representation of the resource.</span></span>
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




