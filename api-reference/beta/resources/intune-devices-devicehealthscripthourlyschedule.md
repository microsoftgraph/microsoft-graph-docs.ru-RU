---
title: Тип ресурса Девицехеалсскрипсаурлисчедуле
description: Тип почасового расписания для сценария работоспособности устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 883ae445447d358342b9c817d3cacd732b3a9b79
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49226519"
---
# <a name="devicehealthscripthourlyschedule-resource-type"></a><span data-ttu-id="025bf-103">Тип ресурса Девицехеалсскрипсаурлисчедуле</span><span class="sxs-lookup"><span data-stu-id="025bf-103">deviceHealthScriptHourlySchedule resource type</span></span>

<span data-ttu-id="025bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="025bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="025bf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="025bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="025bf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="025bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="025bf-107">Тип почасового расписания для сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="025bf-107">Type of Device health script hourly schedule.</span></span>


<span data-ttu-id="025bf-108">Наследуется от [девицехеалсскриптрунсчедуле](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="025bf-108">Inherits from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="025bf-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="025bf-109">Properties</span></span>
|<span data-ttu-id="025bf-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="025bf-110">Property</span></span>|<span data-ttu-id="025bf-111">Тип</span><span class="sxs-lookup"><span data-stu-id="025bf-111">Type</span></span>|<span data-ttu-id="025bf-112">Описание</span><span class="sxs-lookup"><span data-stu-id="025bf-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="025bf-113">interval</span><span class="sxs-lookup"><span data-stu-id="025bf-113">interval</span></span>|<span data-ttu-id="025bf-114">Int32</span><span class="sxs-lookup"><span data-stu-id="025bf-114">Int32</span></span>|<span data-ttu-id="025bf-115">Значение x каждого x часа для ежечасного расписания, каждые x дней для ежедневного расписания, каждые x недель для еженедельного расписания, каждые x месяцев для ежемесячного расписания.</span><span class="sxs-lookup"><span data-stu-id="025bf-115">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="025bf-116">Допустимые значения — от 1 до 23, наследуемые от [девицехеалсскриптрунсчедуле](../resources/intune-devices-devicehealthscriptrunschedule.md)</span><span class="sxs-lookup"><span data-stu-id="025bf-116">Valid values 1 to 23 Inherited from [deviceHealthScriptRunSchedule](../resources/intune-devices-devicehealthscriptrunschedule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="025bf-117">Связи</span><span class="sxs-lookup"><span data-stu-id="025bf-117">Relationships</span></span>
<span data-ttu-id="025bf-118">Нет</span><span class="sxs-lookup"><span data-stu-id="025bf-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="025bf-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="025bf-119">JSON Representation</span></span>
<span data-ttu-id="025bf-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="025bf-120">Here is a JSON representation of the resource.</span></span>
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




