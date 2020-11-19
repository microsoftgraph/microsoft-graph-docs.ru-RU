---
title: Тип ресурса Девицехеалсскрипттимесчедуле
description: Базовый тип расписания работоспособности устройства для сценария работоспособности.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 362bc9d449c3854fa98272758546a871333162a8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299340"
---
# <a name="devicehealthscripttimeschedule-resource-type"></a><span data-ttu-id="1bd5c-103">Тип ресурса Девицехеалсскрипттимесчедуле</span><span class="sxs-lookup"><span data-stu-id="1bd5c-103">deviceHealthScriptTimeSchedule resource type</span></span>

<span data-ttu-id="1bd5c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bd5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bd5c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bd5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bd5c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1bd5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bd5c-107">Базовый тип расписания работоспособности устройства для сценария работоспособности.</span><span class="sxs-lookup"><span data-stu-id="1bd5c-107">Base type of Device health script time schedule.</span></span>


<span data-ttu-id="1bd5c-108">Наследуется от [девицехеалсскриптрунсчедуле](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="1bd5c-108">Inherits from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1bd5c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1bd5c-109">Properties</span></span>
|<span data-ttu-id="1bd5c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1bd5c-110">Property</span></span>|<span data-ttu-id="1bd5c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1bd5c-111">Type</span></span>|<span data-ttu-id="1bd5c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1bd5c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bd5c-113">interval</span><span class="sxs-lookup"><span data-stu-id="1bd5c-113">interval</span></span>|<span data-ttu-id="1bd5c-114">Int32</span><span class="sxs-lookup"><span data-stu-id="1bd5c-114">Int32</span></span>|<span data-ttu-id="1bd5c-115">Значение x каждого x часа для ежечасного расписания, каждые x дней для ежедневного расписания, каждые x недель для еженедельного расписания, каждые x месяцев для ежемесячного расписания.</span><span class="sxs-lookup"><span data-stu-id="1bd5c-115">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="1bd5c-116">Допустимые значения — от 1 до 23, наследуемые от [девицехеалсскриптрунсчедуле](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="1bd5c-116">Valid values 1 to 23 Inherited from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>|
|<span data-ttu-id="1bd5c-117">усеутк</span><span class="sxs-lookup"><span data-stu-id="1bd5c-117">useUtc</span></span>|<span data-ttu-id="1bd5c-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="1bd5c-118">Boolean</span></span>|<span data-ttu-id="1bd5c-119">Укажите время в формате UTC или местное время клиента.</span><span class="sxs-lookup"><span data-stu-id="1bd5c-119">Indicate if the time is Utc or client local time.</span></span>|
|<span data-ttu-id="1bd5c-120">time</span><span class="sxs-lookup"><span data-stu-id="1bd5c-120">time</span></span>|<span data-ttu-id="1bd5c-121">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1bd5c-121">TimeOfDay</span></span>|<span data-ttu-id="1bd5c-122">При планировании запуска сценария.</span><span class="sxs-lookup"><span data-stu-id="1bd5c-122">At what time the script is scheduled to run.</span></span> <span data-ttu-id="1bd5c-123">Эта коллекция может содержать не более 20 элементов.</span><span class="sxs-lookup"><span data-stu-id="1bd5c-123">This collection can contain a maximum of 20 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1bd5c-124">Связи</span><span class="sxs-lookup"><span data-stu-id="1bd5c-124">Relationships</span></span>
<span data-ttu-id="1bd5c-125">Нет</span><span class="sxs-lookup"><span data-stu-id="1bd5c-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1bd5c-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1bd5c-126">JSON Representation</span></span>
<span data-ttu-id="1bd5c-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1bd5c-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptTimeSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptTimeSchedule",
  "interval": 1024,
  "useUtc": true,
  "time": "String (time of day)"
}
```




