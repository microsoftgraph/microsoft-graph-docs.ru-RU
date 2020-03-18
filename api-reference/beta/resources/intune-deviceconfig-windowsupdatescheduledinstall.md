---
title: Тип ресурса windowsUpdateScheduledInstall
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9da6df7bddf40e5d5823aee59c6b96e4cbf13df1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786167"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="79ad5-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="79ad5-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="79ad5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79ad5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79ad5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79ad5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79ad5-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="79ad5-106">Not yet documented</span></span>


<span data-ttu-id="79ad5-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="79ad5-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="79ad5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="79ad5-108">Properties</span></span>
|<span data-ttu-id="79ad5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="79ad5-109">Property</span></span>|<span data-ttu-id="79ad5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="79ad5-110">Type</span></span>|<span data-ttu-id="79ad5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="79ad5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79ad5-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="79ad5-112">scheduledInstallDay</span></span>|[<span data-ttu-id="79ad5-113">виклисчедуле</span><span class="sxs-lookup"><span data-stu-id="79ad5-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="79ad5-114">Запланированный день установки по неделям.</span><span class="sxs-lookup"><span data-stu-id="79ad5-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="79ad5-115">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="79ad5-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="79ad5-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="79ad5-116">scheduledInstallTime</span></span>|<span data-ttu-id="79ad5-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="79ad5-117">TimeOfDay</span></span>|<span data-ttu-id="79ad5-118">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="79ad5-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="79ad5-119">Связи</span><span class="sxs-lookup"><span data-stu-id="79ad5-119">Relationships</span></span>
<span data-ttu-id="79ad5-120">Нет</span><span class="sxs-lookup"><span data-stu-id="79ad5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79ad5-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="79ad5-121">JSON Representation</span></span>
<span data-ttu-id="79ad5-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79ad5-122">Here is a JSON representation of the resource.</span></span>
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



