---
title: Тип ресурса Девицехеалсскрипсаурлисчедуле
description: Тип почасового расписания для сценария работоспособности устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d2276d95d09a1628b07d3b9bc87381b0d85d431f
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44176254"
---
# <a name="devicehealthscripthourlyschedule-resource-type"></a><span data-ttu-id="c0e11-103">Тип ресурса Девицехеалсскрипсаурлисчедуле</span><span class="sxs-lookup"><span data-stu-id="c0e11-103">deviceHealthScriptHourlySchedule resource type</span></span>

<span data-ttu-id="c0e11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0e11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0e11-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0e11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0e11-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0e11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0e11-107">Тип почасового расписания для сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="c0e11-107">Type of Device health script hourly schedule.</span></span>


<span data-ttu-id="c0e11-108">Наследуется от [девицехеалсскриптрунсчедуле](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="c0e11-108">Inherits from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c0e11-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0e11-109">Properties</span></span>
|<span data-ttu-id="c0e11-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0e11-110">Property</span></span>|<span data-ttu-id="c0e11-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c0e11-111">Type</span></span>|<span data-ttu-id="c0e11-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c0e11-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0e11-113">interval</span><span class="sxs-lookup"><span data-stu-id="c0e11-113">interval</span></span>|<span data-ttu-id="c0e11-114">Int32</span><span class="sxs-lookup"><span data-stu-id="c0e11-114">Int32</span></span>|<span data-ttu-id="c0e11-115">Значение x каждого x часа для ежечасного расписания, каждые x дней для ежедневного расписания, каждые x недель для еженедельного расписания, каждые x месяцев для ежемесячного расписания.</span><span class="sxs-lookup"><span data-stu-id="c0e11-115">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="c0e11-116">Допустимые значения — от 1 до 23, наследуемые от [девицехеалсскриптрунсчедуле](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="c0e11-116">Valid values 1 to 23 Inherited from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0e11-117">Связи</span><span class="sxs-lookup"><span data-stu-id="c0e11-117">Relationships</span></span>
<span data-ttu-id="c0e11-118">Нет</span><span class="sxs-lookup"><span data-stu-id="c0e11-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0e11-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0e11-119">JSON Representation</span></span>
<span data-ttu-id="c0e11-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0e11-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptHourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptHourlySchedule",
  "interval": 1024
}
```



