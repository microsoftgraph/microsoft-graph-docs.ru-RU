---
title: Тип ресурса Девицехеалсскриптрунсчедуле
description: Базовый тип расписания запуска сценария работоспособности устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a1f28c4e6cfe5c1155c7cf96446d76dff609d6d
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178530"
---
# <a name="devicehealthscriptrunschedule-resource-type"></a><span data-ttu-id="d8823-103">Тип ресурса Девицехеалсскриптрунсчедуле</span><span class="sxs-lookup"><span data-stu-id="d8823-103">deviceHealthScriptRunSchedule resource type</span></span>

<span data-ttu-id="d8823-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8823-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8823-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8823-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8823-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8823-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8823-107">Базовый тип расписания запуска сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="d8823-107">Base type of Device health script run schedule.</span></span>

## <a name="properties"></a><span data-ttu-id="d8823-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8823-108">Properties</span></span>
|<span data-ttu-id="d8823-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8823-109">Property</span></span>|<span data-ttu-id="d8823-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d8823-110">Type</span></span>|<span data-ttu-id="d8823-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d8823-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8823-112">interval</span><span class="sxs-lookup"><span data-stu-id="d8823-112">interval</span></span>|<span data-ttu-id="d8823-113">Int32</span><span class="sxs-lookup"><span data-stu-id="d8823-113">Int32</span></span>|<span data-ttu-id="d8823-114">Значение x каждого x часа для ежечасного расписания, каждые x дней для ежедневного расписания, каждые x недель для еженедельного расписания, каждые x месяцев для ежемесячного расписания.</span><span class="sxs-lookup"><span data-stu-id="d8823-114">The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule.</span></span> <span data-ttu-id="d8823-115">Допустимые значения — от 1 до 23.</span><span class="sxs-lookup"><span data-stu-id="d8823-115">Valid values 1 to 23</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8823-116">Связи</span><span class="sxs-lookup"><span data-stu-id="d8823-116">Relationships</span></span>
<span data-ttu-id="d8823-117">Нет</span><span class="sxs-lookup"><span data-stu-id="d8823-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8823-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8823-118">JSON Representation</span></span>
<span data-ttu-id="d8823-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8823-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSchedule",
  "interval": 1024
}
```



