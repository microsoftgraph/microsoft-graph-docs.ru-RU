---
title: Тип ресурса Девицехеалсскриптдаилисчедуле
description: Ежедневное расписание сценариев работоспособности устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 456c52392e57e6381f512a7d5403009ea83c6659
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293005"
---
# <a name="devicehealthscriptdailyschedule-resource-type"></a><span data-ttu-id="9fbf5-103">Тип ресурса Девицехеалсскриптдаилисчедуле</span><span class="sxs-lookup"><span data-stu-id="9fbf5-103">deviceHealthScriptDailySchedule resource type</span></span>

<span data-ttu-id="9fbf5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fbf5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fbf5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fbf5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fbf5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9fbf5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fbf5-107">Ежедневное расписание сценариев работоспособности устройств.</span><span class="sxs-lookup"><span data-stu-id="9fbf5-107">Device health script daily schedule.</span></span>


<span data-ttu-id="9fbf5-108">Наследуется от [девицехеалсскрипттимесчедуле](../resources/intune-devices-devicehealthscripttimeschedule.md)</span><span class="sxs-lookup"><span data-stu-id="9fbf5-108">Inherits from [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9fbf5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fbf5-109">Properties</span></span>
|<span data-ttu-id="9fbf5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fbf5-110">Property</span></span>|<span data-ttu-id="9fbf5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9fbf5-111">Type</span></span>|<span data-ttu-id="9fbf5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9fbf5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fbf5-113">interval</span><span class="sxs-lookup"><span data-stu-id="9fbf5-113">interval</span></span>|<span data-ttu-id="9fbf5-114">Int32</span><span class="sxs-lookup"><span data-stu-id="9fbf5-114">Int32</span></span>|<span data-ttu-id="9fbf5-115">Значение x каждого x часа для ежечасного расписания, каждые x дней для ежедневного расписания, каждые x недель для еженедельного расписания, каждые x месяцев для ежемесячного расписания.</span><span class="sxs-lookup"><span data-stu-id="9fbf5-115">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="9fbf5-116">Допустимые значения — от 1 до 23, наследуемые от [девицехеалсскриптрунсчедуле](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="9fbf5-116">Valid values 1 to 23 Inherited from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>|
|<span data-ttu-id="9fbf5-117">усеутк</span><span class="sxs-lookup"><span data-stu-id="9fbf5-117">useUtc</span></span>|<span data-ttu-id="9fbf5-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fbf5-118">Boolean</span></span>|<span data-ttu-id="9fbf5-119">Укажите время в формате UTC или местное время клиента.</span><span class="sxs-lookup"><span data-stu-id="9fbf5-119">Indicate if the time is Utc or client local time.</span></span> <span data-ttu-id="9fbf5-120">Наследуется от [девицехеалсскрипттимесчедуле](../resources/intune-devices-devicehealthscripttimeschedule.md)</span><span class="sxs-lookup"><span data-stu-id="9fbf5-120">Inherited from [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span></span>|
|<span data-ttu-id="9fbf5-121">time</span><span class="sxs-lookup"><span data-stu-id="9fbf5-121">time</span></span>|<span data-ttu-id="9fbf5-122">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9fbf5-122">TimeOfDay</span></span>|<span data-ttu-id="9fbf5-123">При планировании запуска сценария.</span><span class="sxs-lookup"><span data-stu-id="9fbf5-123">At what time the script is scheduled to run.</span></span> <span data-ttu-id="9fbf5-124">Эта коллекция может содержать не более 20 элементов.</span><span class="sxs-lookup"><span data-stu-id="9fbf5-124">This collection can contain a maximum of 20 elements.</span></span> <span data-ttu-id="9fbf5-125">Наследуется от [девицехеалсскрипттимесчедуле](../resources/intune-devices-devicehealthscripttimeschedule.md)</span><span class="sxs-lookup"><span data-stu-id="9fbf5-125">Inherited from [deviceHealthScriptTimeSchedule](../resources/intune-devices-devicehealthscripttimeschedule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fbf5-126">Связи</span><span class="sxs-lookup"><span data-stu-id="9fbf5-126">Relationships</span></span>
<span data-ttu-id="9fbf5-127">Нет</span><span class="sxs-lookup"><span data-stu-id="9fbf5-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fbf5-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fbf5-128">JSON Representation</span></span>
<span data-ttu-id="9fbf5-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fbf5-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptDailySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDailySchedule",
  "interval": 1024,
  "useUtc": true,
  "time": "String (time of day)"
}
```




