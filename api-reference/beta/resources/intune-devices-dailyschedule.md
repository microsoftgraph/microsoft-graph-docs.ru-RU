---
title: Тип ресурса Даилисчедуле
description: Расписание ежедневного запуска сценария управления для повторяющегося устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dd2b226255f433b4f82d042b6389830143515033
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31788074"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="3a05d-103">Тип ресурса Даилисчедуле</span><span class="sxs-lookup"><span data-stu-id="3a05d-103">dailySchedule resource type</span></span>

> <span data-ttu-id="3a05d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a05d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a05d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a05d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a05d-106">Расписание ежедневного запуска сценария управления для повторяющегося устройства.</span><span class="sxs-lookup"><span data-stu-id="3a05d-106">Daily run schedule of a recurring device management script.</span></span>


<span data-ttu-id="3a05d-107">НаСледуется от [рунсчедуле](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="3a05d-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3a05d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3a05d-108">Properties</span></span>
|<span data-ttu-id="3a05d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a05d-109">Property</span></span>|<span data-ttu-id="3a05d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3a05d-110">Type</span></span>|<span data-ttu-id="3a05d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3a05d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a05d-112">interval</span><span class="sxs-lookup"><span data-stu-id="3a05d-112">interval</span></span>|<span data-ttu-id="3a05d-113">Int32</span><span class="sxs-lookup"><span data-stu-id="3a05d-113">Int32</span></span>|<span data-ttu-id="3a05d-114">Интервал (количество дней)</span><span class="sxs-lookup"><span data-stu-id="3a05d-114">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a05d-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="3a05d-115">Relationships</span></span>
<span data-ttu-id="3a05d-116">Нет</span><span class="sxs-lookup"><span data-stu-id="3a05d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a05d-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3a05d-117">JSON Representation</span></span>
<span data-ttu-id="3a05d-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a05d-118">Here is a JSON representation of the resource.</span></span>
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





