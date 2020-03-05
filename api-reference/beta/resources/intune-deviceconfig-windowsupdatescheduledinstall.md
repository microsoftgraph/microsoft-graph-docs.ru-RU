---
title: Тип ресурса windowsUpdateScheduledInstall
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 13c6df3f312872b1fab64c320c17ae3c3115c99e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528937"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="5275c-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="5275c-103">windowsUpdateScheduledInstall resource type</span></span>

<span data-ttu-id="5275c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5275c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5275c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5275c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5275c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5275c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5275c-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5275c-107">Not yet documented</span></span>


<span data-ttu-id="5275c-108">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="5275c-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5275c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5275c-109">Properties</span></span>
|<span data-ttu-id="5275c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5275c-110">Property</span></span>|<span data-ttu-id="5275c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5275c-111">Type</span></span>|<span data-ttu-id="5275c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5275c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5275c-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="5275c-113">scheduledInstallDay</span></span>|[<span data-ttu-id="5275c-114">виклисчедуле</span><span class="sxs-lookup"><span data-stu-id="5275c-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="5275c-115">Запланированный день установки по неделям.</span><span class="sxs-lookup"><span data-stu-id="5275c-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="5275c-116">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="5275c-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="5275c-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="5275c-117">scheduledInstallTime</span></span>|<span data-ttu-id="5275c-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="5275c-118">TimeOfDay</span></span>|<span data-ttu-id="5275c-119">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="5275c-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="5275c-120">Связи</span><span class="sxs-lookup"><span data-stu-id="5275c-120">Relationships</span></span>
<span data-ttu-id="5275c-121">Нет</span><span class="sxs-lookup"><span data-stu-id="5275c-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5275c-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5275c-122">JSON Representation</span></span>
<span data-ttu-id="5275c-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5275c-123">Here is a JSON representation of the resource.</span></span>
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



