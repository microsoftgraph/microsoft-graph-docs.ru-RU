---
title: Тип ресурса Даилисчедуле
description: Расписание ежедневного запуска сценария управления для повторяющегося устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 01a7b999d06bdf0a5c367cad5960563c70c932e9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528666"
---
# <a name="dailyschedule-resource-type"></a><span data-ttu-id="14f29-103">Тип ресурса Даилисчедуле</span><span class="sxs-lookup"><span data-stu-id="14f29-103">dailySchedule resource type</span></span>

<span data-ttu-id="14f29-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="14f29-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14f29-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14f29-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14f29-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14f29-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14f29-107">Расписание ежедневного запуска сценария управления для повторяющегося устройства.</span><span class="sxs-lookup"><span data-stu-id="14f29-107">Daily run schedule of a recurring device management script.</span></span>


<span data-ttu-id="14f29-108">Наследуется от [рунсчедуле](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="14f29-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="14f29-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="14f29-109">Properties</span></span>
|<span data-ttu-id="14f29-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="14f29-110">Property</span></span>|<span data-ttu-id="14f29-111">Тип</span><span class="sxs-lookup"><span data-stu-id="14f29-111">Type</span></span>|<span data-ttu-id="14f29-112">Описание</span><span class="sxs-lookup"><span data-stu-id="14f29-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14f29-113">interval</span><span class="sxs-lookup"><span data-stu-id="14f29-113">interval</span></span>|<span data-ttu-id="14f29-114">Int32</span><span class="sxs-lookup"><span data-stu-id="14f29-114">Int32</span></span>|<span data-ttu-id="14f29-115">Интервал (количество дней)</span><span class="sxs-lookup"><span data-stu-id="14f29-115">Interval in number of days</span></span>|

## <a name="relationships"></a><span data-ttu-id="14f29-116">Связи</span><span class="sxs-lookup"><span data-stu-id="14f29-116">Relationships</span></span>
<span data-ttu-id="14f29-117">Нет</span><span class="sxs-lookup"><span data-stu-id="14f29-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14f29-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="14f29-118">JSON Representation</span></span>
<span data-ttu-id="14f29-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14f29-119">Here is a JSON representation of the resource.</span></span>
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



