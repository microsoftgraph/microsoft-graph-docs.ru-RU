---
title: Тип ресурса windowsUpdateScheduledInstall
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd3a1aafe751bd5db334387cc3872c68e6de6637
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523638"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="d627b-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="d627b-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="d627b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d627b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d627b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d627b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d627b-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d627b-106">Not yet documented</span></span>


<span data-ttu-id="d627b-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="d627b-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d627b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d627b-108">Properties</span></span>
|<span data-ttu-id="d627b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d627b-109">Property</span></span>|<span data-ttu-id="d627b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d627b-110">Type</span></span>|<span data-ttu-id="d627b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d627b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d627b-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="d627b-112">scheduledInstallDay</span></span>|[<span data-ttu-id="d627b-113">Виклисчедуле</span><span class="sxs-lookup"><span data-stu-id="d627b-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="d627b-114">Запланированный день установки по неделям.</span><span class="sxs-lookup"><span data-stu-id="d627b-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="d627b-115">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="d627b-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="d627b-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="d627b-116">scheduledInstallTime</span></span>|<span data-ttu-id="d627b-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d627b-117">TimeOfDay</span></span>|<span data-ttu-id="d627b-118">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="d627b-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="d627b-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="d627b-119">Relationships</span></span>
<span data-ttu-id="d627b-120">Нет</span><span class="sxs-lookup"><span data-stu-id="d627b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d627b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d627b-121">JSON Representation</span></span>
<span data-ttu-id="d627b-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d627b-122">Here is a JSON representation of the resource.</span></span>
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





