---
title: Тип ресурса windowsUpdateScheduledInstall
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 21fde76a0114cb8ebd9a5e586e43b2e1cd968170
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039623"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="885d1-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="885d1-103">windowsUpdateScheduledInstall resource type</span></span>

<span data-ttu-id="885d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="885d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="885d1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="885d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="885d1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="885d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="885d1-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="885d1-107">Not yet documented</span></span>


<span data-ttu-id="885d1-108">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="885d1-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="885d1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="885d1-109">Properties</span></span>
|<span data-ttu-id="885d1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="885d1-110">Property</span></span>|<span data-ttu-id="885d1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="885d1-111">Type</span></span>|<span data-ttu-id="885d1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="885d1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="885d1-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="885d1-113">scheduledInstallDay</span></span>|[<span data-ttu-id="885d1-114">виклисчедуле</span><span class="sxs-lookup"><span data-stu-id="885d1-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="885d1-115">Запланированный день установки по неделям.</span><span class="sxs-lookup"><span data-stu-id="885d1-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="885d1-116">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="885d1-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="885d1-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="885d1-117">scheduledInstallTime</span></span>|<span data-ttu-id="885d1-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="885d1-118">TimeOfDay</span></span>|<span data-ttu-id="885d1-119">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="885d1-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="885d1-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="885d1-120">Relationships</span></span>
<span data-ttu-id="885d1-121">Нет</span><span class="sxs-lookup"><span data-stu-id="885d1-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="885d1-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="885d1-122">JSON Representation</span></span>
<span data-ttu-id="885d1-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="885d1-123">Here is a JSON representation of the resource.</span></span>
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






