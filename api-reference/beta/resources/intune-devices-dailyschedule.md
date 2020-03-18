---
title: Тип ресурса Даилисчедуле
description: Расписание ежедневного запуска сценария управления для повторяющегося устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6b95238a35db1e439768784a58007f6b604031e2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785044"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="fc2d0-103">Тип ресурса Даилисчедуле</span><span class="sxs-lookup"><span data-stu-id="fc2d0-103">dailySchedule resource type</span></span>

> <span data-ttu-id="fc2d0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc2d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc2d0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc2d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc2d0-106">Расписание ежедневного запуска сценария управления для повторяющегося устройства.</span><span class="sxs-lookup"><span data-stu-id="fc2d0-106">Daily run schedule of a recurring device management script.</span></span>


<span data-ttu-id="fc2d0-107">Наследуется от [рунсчедуле](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="fc2d0-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fc2d0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc2d0-108">Properties</span></span>
|<span data-ttu-id="fc2d0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc2d0-109">Property</span></span>|<span data-ttu-id="fc2d0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fc2d0-110">Type</span></span>|<span data-ttu-id="fc2d0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fc2d0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc2d0-112">interval</span><span class="sxs-lookup"><span data-stu-id="fc2d0-112">interval</span></span>|<span data-ttu-id="fc2d0-113">Int32</span><span class="sxs-lookup"><span data-stu-id="fc2d0-113">Int32</span></span>|<span data-ttu-id="fc2d0-114">Интервал (количество дней)</span><span class="sxs-lookup"><span data-stu-id="fc2d0-114">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc2d0-115">Связи</span><span class="sxs-lookup"><span data-stu-id="fc2d0-115">Relationships</span></span>
<span data-ttu-id="fc2d0-116">Нет</span><span class="sxs-lookup"><span data-stu-id="fc2d0-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc2d0-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc2d0-117">JSON Representation</span></span>
<span data-ttu-id="fc2d0-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc2d0-118">Here is a JSON representation of the resource.</span></span>
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



