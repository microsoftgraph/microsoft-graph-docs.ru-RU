---
title: Тип ресурса Даилисчедуле
description: Расписание ежедневного запуска сценария управления для повторяющегося устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf0f5b59992a862b88ae663b45b6ae910ac4ba82
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942964"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="e62c1-103">Тип ресурса Даилисчедуле</span><span class="sxs-lookup"><span data-stu-id="e62c1-103">dailySchedule resource type</span></span>

> <span data-ttu-id="e62c1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e62c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e62c1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e62c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e62c1-106">Расписание ежедневного запуска сценария управления для повторяющегося устройства.</span><span class="sxs-lookup"><span data-stu-id="e62c1-106">Daily run schedule of a recurring device management script.</span></span>


<span data-ttu-id="e62c1-107">Наследуется от [рунсчедуле](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="e62c1-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e62c1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e62c1-108">Properties</span></span>
|<span data-ttu-id="e62c1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e62c1-109">Property</span></span>|<span data-ttu-id="e62c1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e62c1-110">Type</span></span>|<span data-ttu-id="e62c1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e62c1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e62c1-112">interval</span><span class="sxs-lookup"><span data-stu-id="e62c1-112">interval</span></span>|<span data-ttu-id="e62c1-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e62c1-113">Int32</span></span>|<span data-ttu-id="e62c1-114">Интервал (количество дней)</span><span class="sxs-lookup"><span data-stu-id="e62c1-114">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="e62c1-115">Связи</span><span class="sxs-lookup"><span data-stu-id="e62c1-115">Relationships</span></span>
<span data-ttu-id="e62c1-116">Нет</span><span class="sxs-lookup"><span data-stu-id="e62c1-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e62c1-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e62c1-117">JSON Representation</span></span>
<span data-ttu-id="e62c1-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e62c1-118">Here is a JSON representation of the resource.</span></span>
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




