---
title: Тип ресурса windowsUpdateScheduledInstall
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b3c6d5fa7e517713d1904d33c94bcd8dccec5d6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030900"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="d24ca-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="d24ca-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="d24ca-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d24ca-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d24ca-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d24ca-105">Not yet documented</span></span>


<span data-ttu-id="d24ca-106">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="d24ca-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d24ca-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d24ca-107">Properties</span></span>
|<span data-ttu-id="d24ca-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d24ca-108">Property</span></span>|<span data-ttu-id="d24ca-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d24ca-109">Type</span></span>|<span data-ttu-id="d24ca-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d24ca-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d24ca-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="d24ca-111">scheduledInstallDay</span></span>|[<span data-ttu-id="d24ca-112">Виклисчедуле</span><span class="sxs-lookup"><span data-stu-id="d24ca-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="d24ca-113">Запланированный день установки по неделям.</span><span class="sxs-lookup"><span data-stu-id="d24ca-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="d24ca-114">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="d24ca-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="d24ca-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="d24ca-115">scheduledInstallTime</span></span>|<span data-ttu-id="d24ca-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d24ca-116">TimeOfDay</span></span>|<span data-ttu-id="d24ca-117">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="d24ca-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="d24ca-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="d24ca-118">Relationships</span></span>
<span data-ttu-id="d24ca-119">Нет</span><span class="sxs-lookup"><span data-stu-id="d24ca-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d24ca-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d24ca-120">JSON Representation</span></span>
<span data-ttu-id="d24ca-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d24ca-121">Here is a JSON representation of the resource.</span></span>
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



