---
title: Тип ресурса Девицехеалсскрипттимесчедуле
description: Базовый тип расписания работоспособности устройства для сценария работоспособности.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6152b9b2c0c6e5d7a3cb6928f4047f9f68c912b9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060197"
---
# <a name="devicehealthscripttimeschedule-resource-type"></a><span data-ttu-id="a88be-103">Тип ресурса Девицехеалсскрипттимесчедуле</span><span class="sxs-lookup"><span data-stu-id="a88be-103">deviceHealthScriptTimeSchedule resource type</span></span>

<span data-ttu-id="a88be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a88be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a88be-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a88be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a88be-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a88be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a88be-107">Базовый тип расписания работоспособности устройства для сценария работоспособности.</span><span class="sxs-lookup"><span data-stu-id="a88be-107">Base type of Device health script time schedule.</span></span>


<span data-ttu-id="a88be-108">Наследуется от [девицехеалсскриптрунсчедуле](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="a88be-108">Inherits from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a88be-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a88be-109">Properties</span></span>
|<span data-ttu-id="a88be-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a88be-110">Property</span></span>|<span data-ttu-id="a88be-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a88be-111">Type</span></span>|<span data-ttu-id="a88be-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a88be-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a88be-113">interval</span><span class="sxs-lookup"><span data-stu-id="a88be-113">interval</span></span>|<span data-ttu-id="a88be-114">Int32</span><span class="sxs-lookup"><span data-stu-id="a88be-114">Int32</span></span>|<span data-ttu-id="a88be-115">Значение x каждого x часа для ежечасного расписания, каждые x дней для ежедневного расписания, каждые x недель для еженедельного расписания, каждые x месяцев для ежемесячного расписания.</span><span class="sxs-lookup"><span data-stu-id="a88be-115">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="a88be-116">Допустимые значения — от 1 до 23, наследуемые от [девицехеалсскриптрунсчедуле](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="a88be-116">Valid values 1 to 23 Inherited from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>|
|<span data-ttu-id="a88be-117">усеутк</span><span class="sxs-lookup"><span data-stu-id="a88be-117">useUtc</span></span>|<span data-ttu-id="a88be-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="a88be-118">Boolean</span></span>|<span data-ttu-id="a88be-119">Укажите время в формате UTC или местное время клиента.</span><span class="sxs-lookup"><span data-stu-id="a88be-119">Indicate if the time is Utc or client local time.</span></span>|
|<span data-ttu-id="a88be-120">time</span><span class="sxs-lookup"><span data-stu-id="a88be-120">time</span></span>|<span data-ttu-id="a88be-121">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a88be-121">TimeOfDay</span></span>|<span data-ttu-id="a88be-122">При планировании запуска сценария.</span><span class="sxs-lookup"><span data-stu-id="a88be-122">At what time the script is scheduled to run.</span></span> <span data-ttu-id="a88be-123">Эта коллекция может содержать не более 20 элементов.</span><span class="sxs-lookup"><span data-stu-id="a88be-123">This collection can contain a maximum of 20 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a88be-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="a88be-124">Relationships</span></span>
<span data-ttu-id="a88be-125">Нет</span><span class="sxs-lookup"><span data-stu-id="a88be-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a88be-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a88be-126">JSON Representation</span></span>
<span data-ttu-id="a88be-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a88be-127">Here is a JSON representation of the resource.</span></span>
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






