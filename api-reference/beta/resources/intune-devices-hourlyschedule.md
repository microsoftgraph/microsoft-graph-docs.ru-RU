---
title: Тип ресурса Хаурлисчедуле
description: ПоЧасовое расписание выполнения сценария управления повторяющимся устройством.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f86591326f2b4df8e887c657c05ad3d5021946e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522183"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="97728-103">Тип ресурса Хаурлисчедуле</span><span class="sxs-lookup"><span data-stu-id="97728-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="97728-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97728-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97728-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97728-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97728-106">ПоЧасовое расписание выполнения сценария управления повторяющимся устройством.</span><span class="sxs-lookup"><span data-stu-id="97728-106">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="97728-107">НаСледуется от [рунсчедуле](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="97728-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="97728-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="97728-108">Properties</span></span>
|<span data-ttu-id="97728-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="97728-109">Property</span></span>|<span data-ttu-id="97728-110">Тип</span><span class="sxs-lookup"><span data-stu-id="97728-110">Type</span></span>|<span data-ttu-id="97728-111">Описание</span><span class="sxs-lookup"><span data-stu-id="97728-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97728-112">interval</span><span class="sxs-lookup"><span data-stu-id="97728-112">interval</span></span>|<span data-ttu-id="97728-113">Int32</span><span class="sxs-lookup"><span data-stu-id="97728-113">Int32</span></span>|<span data-ttu-id="97728-114">Интервал (в часах)</span><span class="sxs-lookup"><span data-stu-id="97728-114">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="97728-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="97728-115">Relationships</span></span>
<span data-ttu-id="97728-116">Нет</span><span class="sxs-lookup"><span data-stu-id="97728-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97728-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="97728-117">JSON Representation</span></span>
<span data-ttu-id="97728-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97728-118">Here is a JSON representation of the resource.</span></span>
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





