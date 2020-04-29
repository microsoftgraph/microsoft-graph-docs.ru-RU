---
title: Тип ресурса windowsUpdateScheduledInstall
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d2b9173207c52029d4d65faafa2d6c8607423fe8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451364"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="6071b-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="6071b-103">windowsUpdateScheduledInstall resource type</span></span>

<span data-ttu-id="6071b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6071b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6071b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6071b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6071b-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6071b-106">Not yet documented</span></span>


<span data-ttu-id="6071b-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="6071b-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6071b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6071b-108">Properties</span></span>
|<span data-ttu-id="6071b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6071b-109">Property</span></span>|<span data-ttu-id="6071b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6071b-110">Type</span></span>|<span data-ttu-id="6071b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6071b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6071b-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="6071b-112">scheduledInstallDay</span></span>|[<span data-ttu-id="6071b-113">виклисчедуле</span><span class="sxs-lookup"><span data-stu-id="6071b-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="6071b-114">Запланированный день установки по неделям.</span><span class="sxs-lookup"><span data-stu-id="6071b-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="6071b-115">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="6071b-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="6071b-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="6071b-116">scheduledInstallTime</span></span>|<span data-ttu-id="6071b-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6071b-117">TimeOfDay</span></span>|<span data-ttu-id="6071b-118">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="6071b-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="6071b-119">Связи</span><span class="sxs-lookup"><span data-stu-id="6071b-119">Relationships</span></span>
<span data-ttu-id="6071b-120">Нет</span><span class="sxs-lookup"><span data-stu-id="6071b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6071b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6071b-121">JSON Representation</span></span>
<span data-ttu-id="6071b-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6071b-122">Here is a JSON representation of the resource.</span></span>
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







