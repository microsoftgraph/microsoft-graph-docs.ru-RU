---
title: Тип ресурса Девицехеалсскриптрунонцесчедуле
description: Сценарий работоспособности устройства запускается один раз по расписанию.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 230d9592b66f85457b20343a48d8024a9b4afe87
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299424"
---
# <a name="devicehealthscriptrunonceschedule-resource-type"></a><span data-ttu-id="f1593-103">Тип ресурса Девицехеалсскриптрунонцесчедуле</span><span class="sxs-lookup"><span data-stu-id="f1593-103">deviceHealthScriptRunOnceSchedule resource type</span></span>

<span data-ttu-id="f1593-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1593-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1593-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1593-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1593-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1593-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1593-107">Сценарий работоспособности устройства запускается один раз по расписанию.</span><span class="sxs-lookup"><span data-stu-id="f1593-107">Device health script run once schedule.</span></span>


<span data-ttu-id="f1593-108">Наследуется от [девицехеалсскрипттимесчедуле](../resources/intune-devices-devicehealthscripttimeschedule.md)</span><span class="sxs-lookup"><span data-stu-id="f1593-108">Inherits from [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f1593-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1593-109">Properties</span></span>
|<span data-ttu-id="f1593-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1593-110">Property</span></span>|<span data-ttu-id="f1593-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f1593-111">Type</span></span>|<span data-ttu-id="f1593-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f1593-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1593-113">interval</span><span class="sxs-lookup"><span data-stu-id="f1593-113">interval</span></span>|<span data-ttu-id="f1593-114">Int32</span><span class="sxs-lookup"><span data-stu-id="f1593-114">Int32</span></span>|<span data-ttu-id="f1593-115">Значение x каждого x часа для ежечасного расписания, каждые x дней для ежедневного расписания, каждые x недель для еженедельного расписания, каждые x месяцев для ежемесячного расписания.</span><span class="sxs-lookup"><span data-stu-id="f1593-115">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="f1593-116">Допустимые значения — от 1 до 23, наследуемые от [девицехеалсскриптрунсчедуле](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="f1593-116">Valid values 1 to 23 Inherited from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>|
|<span data-ttu-id="f1593-117">усеутк</span><span class="sxs-lookup"><span data-stu-id="f1593-117">useUtc</span></span>|<span data-ttu-id="f1593-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1593-118">Boolean</span></span>|<span data-ttu-id="f1593-119">Укажите время в формате UTC или местное время клиента.</span><span class="sxs-lookup"><span data-stu-id="f1593-119">Indicate if the time is Utc or client local time.</span></span> <span data-ttu-id="f1593-120">Наследуется от [девицехеалсскрипттимесчедуле](../resources/intune-devices-devicehealthscripttimeschedule.md)</span><span class="sxs-lookup"><span data-stu-id="f1593-120">Inherited from [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span></span>|
|<span data-ttu-id="f1593-121">time</span><span class="sxs-lookup"><span data-stu-id="f1593-121">time</span></span>|<span data-ttu-id="f1593-122">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f1593-122">TimeOfDay</span></span>|<span data-ttu-id="f1593-123">При планировании запуска сценария.</span><span class="sxs-lookup"><span data-stu-id="f1593-123">At what time the script is scheduled to run.</span></span> <span data-ttu-id="f1593-124">Эта коллекция может содержать не более 20 элементов.</span><span class="sxs-lookup"><span data-stu-id="f1593-124">This collection can contain a maximum of 20 elements.</span></span> <span data-ttu-id="f1593-125">Наследуется от [девицехеалсскрипттимесчедуле](../resources/intune-devices-devicehealthscripttimeschedule.md)</span><span class="sxs-lookup"><span data-stu-id="f1593-125">Inherited from [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span></span>|
|<span data-ttu-id="f1593-126">date</span><span class="sxs-lookup"><span data-stu-id="f1593-126">date</span></span>|<span data-ttu-id="f1593-127">Date</span><span class="sxs-lookup"><span data-stu-id="f1593-127">Date</span></span>|<span data-ttu-id="f1593-128">Дата запланированного запуска сценария.</span><span class="sxs-lookup"><span data-stu-id="f1593-128">The date the script is scheduled to run.</span></span> <span data-ttu-id="f1593-129">Эта коллекция может содержать не более 20 элементов.</span><span class="sxs-lookup"><span data-stu-id="f1593-129">This collection can contain a maximum of 20 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1593-130">Связи</span><span class="sxs-lookup"><span data-stu-id="f1593-130">Relationships</span></span>
<span data-ttu-id="f1593-131">Нет</span><span class="sxs-lookup"><span data-stu-id="f1593-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1593-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1593-132">JSON Representation</span></span>
<span data-ttu-id="f1593-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1593-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunOnceSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunOnceSchedule",
  "interval": 1024,
  "useUtc": true,
  "time": "String (time of day)",
  "date": "String (Date)"
}
```




