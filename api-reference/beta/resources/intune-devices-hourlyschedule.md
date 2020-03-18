---
title: Тип ресурса Хаурлисчедуле
description: Почасовое расписание выполнения сценария управления повторяющимся устройством.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e798eed75cdb5499bb2ea0c3ca40ac4d7c0b9c54
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784021"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="f8719-103">Тип ресурса Хаурлисчедуле</span><span class="sxs-lookup"><span data-stu-id="f8719-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="f8719-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8719-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8719-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f8719-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8719-106">Почасовое расписание выполнения сценария управления повторяющимся устройством.</span><span class="sxs-lookup"><span data-stu-id="f8719-106">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="f8719-107">Наследуется от [рунсчедуле](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="f8719-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f8719-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f8719-108">Properties</span></span>
|<span data-ttu-id="f8719-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8719-109">Property</span></span>|<span data-ttu-id="f8719-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f8719-110">Type</span></span>|<span data-ttu-id="f8719-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f8719-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8719-112">interval</span><span class="sxs-lookup"><span data-stu-id="f8719-112">interval</span></span>|<span data-ttu-id="f8719-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f8719-113">Int32</span></span>|<span data-ttu-id="f8719-114">Интервал (в часах)</span><span class="sxs-lookup"><span data-stu-id="f8719-114">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8719-115">Связи</span><span class="sxs-lookup"><span data-stu-id="f8719-115">Relationships</span></span>
<span data-ttu-id="f8719-116">Нет</span><span class="sxs-lookup"><span data-stu-id="f8719-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8719-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f8719-117">JSON Representation</span></span>
<span data-ttu-id="f8719-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8719-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hourlySchedule",
  "interval": 1024
}
```



