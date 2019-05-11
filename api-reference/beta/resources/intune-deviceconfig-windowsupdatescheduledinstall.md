---
title: Тип ресурса windowsUpdateScheduledInstall
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 270df73ef5db5cde3784adb797475b9232591de6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943622"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="f0a09-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="f0a09-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="f0a09-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0a09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0a09-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0a09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0a09-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f0a09-106">Not yet documented</span></span>


<span data-ttu-id="f0a09-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="f0a09-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f0a09-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0a09-108">Properties</span></span>
|<span data-ttu-id="f0a09-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0a09-109">Property</span></span>|<span data-ttu-id="f0a09-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f0a09-110">Type</span></span>|<span data-ttu-id="f0a09-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f0a09-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0a09-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="f0a09-112">scheduledInstallDay</span></span>|[<span data-ttu-id="f0a09-113">Виклисчедуле</span><span class="sxs-lookup"><span data-stu-id="f0a09-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="f0a09-114">Запланированный день установки по неделям.</span><span class="sxs-lookup"><span data-stu-id="f0a09-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="f0a09-115">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="f0a09-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="f0a09-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="f0a09-116">scheduledInstallTime</span></span>|<span data-ttu-id="f0a09-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f0a09-117">TimeOfDay</span></span>|<span data-ttu-id="f0a09-118">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="f0a09-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0a09-119">Связи</span><span class="sxs-lookup"><span data-stu-id="f0a09-119">Relationships</span></span>
<span data-ttu-id="f0a09-120">Нет</span><span class="sxs-lookup"><span data-stu-id="f0a09-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0a09-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0a09-121">JSON Representation</span></span>
<span data-ttu-id="f0a09-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0a09-122">Here is a JSON representation of the resource.</span></span>
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




