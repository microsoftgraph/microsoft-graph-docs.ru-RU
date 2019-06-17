---
title: Тип ресурса Хаурлисчедуле
description: Почасовое расписание выполнения сценария управления повторяющимся устройством.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aadd9f6e53288087cea5ee75a5f7cab2b2decbde
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995170"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="e13fc-103">Тип ресурса Хаурлисчедуле</span><span class="sxs-lookup"><span data-stu-id="e13fc-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="e13fc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e13fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e13fc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e13fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e13fc-106">Почасовое расписание выполнения сценария управления повторяющимся устройством.</span><span class="sxs-lookup"><span data-stu-id="e13fc-106">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="e13fc-107">Наследуется от [рунсчедуле](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="e13fc-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e13fc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e13fc-108">Properties</span></span>
|<span data-ttu-id="e13fc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e13fc-109">Property</span></span>|<span data-ttu-id="e13fc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e13fc-110">Type</span></span>|<span data-ttu-id="e13fc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e13fc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e13fc-112">interval</span><span class="sxs-lookup"><span data-stu-id="e13fc-112">interval</span></span>|<span data-ttu-id="e13fc-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e13fc-113">Int32</span></span>|<span data-ttu-id="e13fc-114">Интервал (в часах)</span><span class="sxs-lookup"><span data-stu-id="e13fc-114">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="e13fc-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="e13fc-115">Relationships</span></span>
<span data-ttu-id="e13fc-116">Нет</span><span class="sxs-lookup"><span data-stu-id="e13fc-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e13fc-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e13fc-117">JSON Representation</span></span>
<span data-ttu-id="e13fc-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e13fc-118">Here is a JSON representation of the resource.</span></span>
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





