---
title: Тип ресурса windowsUpdateScheduledInstall
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 22c1c6e2ba205c705baabc6bc7643848f7f12686
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759954"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="4aa59-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="4aa59-103">windowsUpdateScheduledInstall resource type</span></span>

<span data-ttu-id="4aa59-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4aa59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4aa59-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4aa59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4aa59-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4aa59-106">Not yet documented</span></span>


<span data-ttu-id="4aa59-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="4aa59-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4aa59-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4aa59-108">Properties</span></span>
|<span data-ttu-id="4aa59-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4aa59-109">Property</span></span>|<span data-ttu-id="4aa59-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4aa59-110">Type</span></span>|<span data-ttu-id="4aa59-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4aa59-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4aa59-112">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="4aa59-112">scheduledInstallDay</span></span>|[<span data-ttu-id="4aa59-113">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="4aa59-113">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="4aa59-114">Запланированный день установки в неделю.</span><span class="sxs-lookup"><span data-stu-id="4aa59-114">Scheduled Install Day in week.</span></span> <span data-ttu-id="4aa59-115">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="4aa59-115">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="4aa59-116">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="4aa59-116">scheduledInstallTime</span></span>|<span data-ttu-id="4aa59-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4aa59-117">TimeOfDay</span></span>|<span data-ttu-id="4aa59-118">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="4aa59-118">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="4aa59-119">Связи</span><span class="sxs-lookup"><span data-stu-id="4aa59-119">Relationships</span></span>
<span data-ttu-id="4aa59-120">Нет</span><span class="sxs-lookup"><span data-stu-id="4aa59-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4aa59-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4aa59-121">JSON Representation</span></span>
<span data-ttu-id="4aa59-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4aa59-122">Here is a JSON representation of the resource.</span></span>
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




