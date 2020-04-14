---
title: Тип ресурса windowsUpdateScheduledInstall
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ceb6330bddf03b230dca644217c70bf1e3bba5d4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441102"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="60ef8-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="60ef8-103">windowsUpdateScheduledInstall resource type</span></span>

<span data-ttu-id="60ef8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60ef8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60ef8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60ef8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60ef8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="60ef8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60ef8-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="60ef8-107">Not yet documented</span></span>


<span data-ttu-id="60ef8-108">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="60ef8-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="60ef8-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="60ef8-109">Properties</span></span>
|<span data-ttu-id="60ef8-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="60ef8-110">Property</span></span>|<span data-ttu-id="60ef8-111">Тип</span><span class="sxs-lookup"><span data-stu-id="60ef8-111">Type</span></span>|<span data-ttu-id="60ef8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="60ef8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60ef8-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="60ef8-113">scheduledInstallDay</span></span>|[<span data-ttu-id="60ef8-114">виклисчедуле</span><span class="sxs-lookup"><span data-stu-id="60ef8-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="60ef8-115">Запланированный день установки по неделям.</span><span class="sxs-lookup"><span data-stu-id="60ef8-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="60ef8-116">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="60ef8-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="60ef8-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="60ef8-117">scheduledInstallTime</span></span>|<span data-ttu-id="60ef8-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="60ef8-118">TimeOfDay</span></span>|<span data-ttu-id="60ef8-119">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="60ef8-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="60ef8-120">Связи</span><span class="sxs-lookup"><span data-stu-id="60ef8-120">Relationships</span></span>
<span data-ttu-id="60ef8-121">Нет</span><span class="sxs-lookup"><span data-stu-id="60ef8-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60ef8-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60ef8-122">JSON Representation</span></span>
<span data-ttu-id="60ef8-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60ef8-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```



