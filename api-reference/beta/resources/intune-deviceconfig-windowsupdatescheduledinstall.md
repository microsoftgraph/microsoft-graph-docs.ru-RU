---
title: Тип ресурса windowsUpdateScheduledInstall
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd3a1aafe751bd5db334387cc3872c68e6de6637
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797923"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="23fdf-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="23fdf-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="23fdf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23fdf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23fdf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23fdf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23fdf-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="23fdf-106">Not yet documented</span></span>


<span data-ttu-id="23fdf-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="23fdf-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="23fdf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="23fdf-108">Properties</span></span>
|<span data-ttu-id="23fdf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="23fdf-109">Property</span></span>|<span data-ttu-id="23fdf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="23fdf-110">Type</span></span>|<span data-ttu-id="23fdf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="23fdf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23fdf-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="23fdf-112">scheduledInstallDay</span></span>|[<span data-ttu-id="23fdf-113">Виклисчедуле</span><span class="sxs-lookup"><span data-stu-id="23fdf-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="23fdf-114">Запланированный день установки по неделям.</span><span class="sxs-lookup"><span data-stu-id="23fdf-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="23fdf-115">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="23fdf-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="23fdf-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="23fdf-116">scheduledInstallTime</span></span>|<span data-ttu-id="23fdf-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="23fdf-117">TimeOfDay</span></span>|<span data-ttu-id="23fdf-118">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="23fdf-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="23fdf-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="23fdf-119">Relationships</span></span>
<span data-ttu-id="23fdf-120">Нет</span><span class="sxs-lookup"><span data-stu-id="23fdf-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23fdf-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23fdf-121">JSON Representation</span></span>
<span data-ttu-id="23fdf-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23fdf-122">Here is a JSON representation of the resource.</span></span>
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





