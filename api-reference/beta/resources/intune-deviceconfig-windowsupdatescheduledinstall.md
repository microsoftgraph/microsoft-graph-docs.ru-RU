---
title: Тип ресурса windowsUpdateScheduledInstall
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1ca4c658c9fa9837deb56868a84ff0bddefeb6d3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272418"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="3749f-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="3749f-103">windowsUpdateScheduledInstall resource type</span></span>

<span data-ttu-id="3749f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3749f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3749f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3749f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3749f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3749f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3749f-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3749f-107">Not yet documented</span></span>


<span data-ttu-id="3749f-108">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="3749f-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3749f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="3749f-109">Properties</span></span>
|<span data-ttu-id="3749f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="3749f-110">Property</span></span>|<span data-ttu-id="3749f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="3749f-111">Type</span></span>|<span data-ttu-id="3749f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3749f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3749f-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="3749f-113">scheduledInstallDay</span></span>|[<span data-ttu-id="3749f-114">виклисчедуле</span><span class="sxs-lookup"><span data-stu-id="3749f-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="3749f-115">Запланированный день установки по неделям.</span><span class="sxs-lookup"><span data-stu-id="3749f-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="3749f-116">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="3749f-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="3749f-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="3749f-117">scheduledInstallTime</span></span>|<span data-ttu-id="3749f-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="3749f-118">TimeOfDay</span></span>|<span data-ttu-id="3749f-119">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="3749f-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="3749f-120">Связи</span><span class="sxs-lookup"><span data-stu-id="3749f-120">Relationships</span></span>
<span data-ttu-id="3749f-121">Нет</span><span class="sxs-lookup"><span data-stu-id="3749f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3749f-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3749f-122">JSON Representation</span></span>
<span data-ttu-id="3749f-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3749f-123">Here is a JSON representation of the resource.</span></span>
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




