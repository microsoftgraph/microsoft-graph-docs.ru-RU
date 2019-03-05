---
title: Тип ресурса windowsUpdateScheduledInstall
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de36e3777518cf7c79a7590c19147d014e2aee7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172508"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="b383f-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="b383f-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="b383f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b383f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b383f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b383f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b383f-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b383f-106">Not yet documented</span></span>


<span data-ttu-id="b383f-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="b383f-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b383f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b383f-108">Properties</span></span>
|<span data-ttu-id="b383f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b383f-109">Property</span></span>|<span data-ttu-id="b383f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b383f-110">Type</span></span>|<span data-ttu-id="b383f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b383f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b383f-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="b383f-112">scheduledInstallDay</span></span>|[<span data-ttu-id="b383f-113">Виклисчедуле</span><span class="sxs-lookup"><span data-stu-id="b383f-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="b383f-114">Запланированный день установки по неделям.</span><span class="sxs-lookup"><span data-stu-id="b383f-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="b383f-115">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="b383f-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="b383f-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="b383f-116">scheduledInstallTime</span></span>|<span data-ttu-id="b383f-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b383f-117">TimeOfDay</span></span>|<span data-ttu-id="b383f-118">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="b383f-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="b383f-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b383f-119">Relationships</span></span>
<span data-ttu-id="b383f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b383f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b383f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b383f-121">JSON Representation</span></span>
<span data-ttu-id="b383f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b383f-122">Here is a JSON representation of the resource.</span></span>
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




