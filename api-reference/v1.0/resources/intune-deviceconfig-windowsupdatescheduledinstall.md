---
title: Тип ресурса windowsUpdateScheduledInstall
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f291fbb34f5fa412fb6da172dd196c766a7327a6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091399"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="7dda0-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="7dda0-103">windowsUpdateScheduledInstall resource type</span></span>

<span data-ttu-id="7dda0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dda0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7dda0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7dda0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dda0-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7dda0-106">Not yet documented</span></span>


<span data-ttu-id="7dda0-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="7dda0-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7dda0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7dda0-108">Properties</span></span>
|<span data-ttu-id="7dda0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7dda0-109">Property</span></span>|<span data-ttu-id="7dda0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7dda0-110">Type</span></span>|<span data-ttu-id="7dda0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7dda0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dda0-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="7dda0-112">scheduledInstallDay</span></span>|[<span data-ttu-id="7dda0-113">виклисчедуле</span><span class="sxs-lookup"><span data-stu-id="7dda0-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="7dda0-114">Запланированный день установки по неделям.</span><span class="sxs-lookup"><span data-stu-id="7dda0-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="7dda0-115">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="7dda0-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="7dda0-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="7dda0-116">scheduledInstallTime</span></span>|<span data-ttu-id="7dda0-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7dda0-117">TimeOfDay</span></span>|<span data-ttu-id="7dda0-118">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="7dda0-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="7dda0-119">Связи</span><span class="sxs-lookup"><span data-stu-id="7dda0-119">Relationships</span></span>
<span data-ttu-id="7dda0-120">Нет</span><span class="sxs-lookup"><span data-stu-id="7dda0-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7dda0-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7dda0-121">JSON Representation</span></span>
<span data-ttu-id="7dda0-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7dda0-122">Here is a JSON representation of the resource.</span></span>
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









