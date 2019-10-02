---
title: Тип ресурса windowsUpdateScheduledInstall
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2fd5958e5b8e853f07c715cd1ecf8c03a9a49a15
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357138"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="42484-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="42484-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="42484-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42484-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42484-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="42484-105">Not yet documented</span></span>


<span data-ttu-id="42484-106">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="42484-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="42484-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="42484-107">Properties</span></span>
|<span data-ttu-id="42484-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="42484-108">Property</span></span>|<span data-ttu-id="42484-109">Тип</span><span class="sxs-lookup"><span data-stu-id="42484-109">Type</span></span>|<span data-ttu-id="42484-110">Описание</span><span class="sxs-lookup"><span data-stu-id="42484-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42484-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="42484-111">scheduledInstallDay</span></span>|[<span data-ttu-id="42484-112">виклисчедуле</span><span class="sxs-lookup"><span data-stu-id="42484-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="42484-113">Запланированный день установки по неделям.</span><span class="sxs-lookup"><span data-stu-id="42484-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="42484-114">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="42484-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="42484-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="42484-115">scheduledInstallTime</span></span>|<span data-ttu-id="42484-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="42484-116">TimeOfDay</span></span>|<span data-ttu-id="42484-117">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="42484-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="42484-118">Связи</span><span class="sxs-lookup"><span data-stu-id="42484-118">Relationships</span></span>
<span data-ttu-id="42484-119">Нет</span><span class="sxs-lookup"><span data-stu-id="42484-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42484-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42484-120">JSON Representation</span></span>
<span data-ttu-id="42484-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42484-121">Here is a JSON representation of the resource.</span></span>
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




