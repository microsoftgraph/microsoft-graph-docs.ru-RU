---
title: Тип ресурса Даилисчедуле
description: Расписание ежедневного запуска сценария управления для повторяющегося устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b921b13fd87d3a500ca543ca6601a9ad368456ea
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465002"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="2bb6a-103">Тип ресурса Даилисчедуле</span><span class="sxs-lookup"><span data-stu-id="2bb6a-103">dailySchedule resource type</span></span>

<span data-ttu-id="2bb6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bb6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2bb6a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bb6a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bb6a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2bb6a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bb6a-107">Расписание ежедневного запуска сценария управления для повторяющегося устройства.</span><span class="sxs-lookup"><span data-stu-id="2bb6a-107">Daily run schedule of a recurring device management script.</span></span>


<span data-ttu-id="2bb6a-108">Наследуется от [рунсчедуле](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="2bb6a-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2bb6a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2bb6a-109">Properties</span></span>
|<span data-ttu-id="2bb6a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2bb6a-110">Property</span></span>|<span data-ttu-id="2bb6a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2bb6a-111">Type</span></span>|<span data-ttu-id="2bb6a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2bb6a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bb6a-113">interval</span><span class="sxs-lookup"><span data-stu-id="2bb6a-113">interval</span></span>|<span data-ttu-id="2bb6a-114">Int32</span><span class="sxs-lookup"><span data-stu-id="2bb6a-114">Int32</span></span>|<span data-ttu-id="2bb6a-115">Интервал (количество дней)</span><span class="sxs-lookup"><span data-stu-id="2bb6a-115">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="2bb6a-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="2bb6a-116">Relationships</span></span>
<span data-ttu-id="2bb6a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="2bb6a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2bb6a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2bb6a-118">JSON Representation</span></span>
<span data-ttu-id="2bb6a-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2bb6a-119">Here is a JSON representation of the resource.</span></span>
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



