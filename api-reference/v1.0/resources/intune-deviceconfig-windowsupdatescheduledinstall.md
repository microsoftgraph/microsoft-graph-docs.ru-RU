---
title: Тип ресурса windowsUpdateScheduledInstall
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2ab68aa48d83e47e6cdbd3afc45ade10545b0590
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530318"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="9d30d-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="9d30d-103">windowsUpdateScheduledInstall resource type</span></span>

<span data-ttu-id="9d30d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d30d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d30d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9d30d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d30d-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9d30d-106">Not yet documented</span></span>


<span data-ttu-id="9d30d-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="9d30d-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9d30d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d30d-108">Properties</span></span>
|<span data-ttu-id="9d30d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d30d-109">Property</span></span>|<span data-ttu-id="9d30d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9d30d-110">Type</span></span>|<span data-ttu-id="9d30d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9d30d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d30d-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="9d30d-112">scheduledInstallDay</span></span>|[<span data-ttu-id="9d30d-113">виклисчедуле</span><span class="sxs-lookup"><span data-stu-id="9d30d-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="9d30d-114">Запланированный день установки по неделям.</span><span class="sxs-lookup"><span data-stu-id="9d30d-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="9d30d-115">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="9d30d-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="9d30d-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="9d30d-116">scheduledInstallTime</span></span>|<span data-ttu-id="9d30d-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9d30d-117">TimeOfDay</span></span>|<span data-ttu-id="9d30d-118">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="9d30d-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d30d-119">Связи</span><span class="sxs-lookup"><span data-stu-id="9d30d-119">Relationships</span></span>
<span data-ttu-id="9d30d-120">Нет</span><span class="sxs-lookup"><span data-stu-id="9d30d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d30d-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d30d-121">JSON Representation</span></span>
<span data-ttu-id="9d30d-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d30d-122">Here is a JSON representation of the resource.</span></span>
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




