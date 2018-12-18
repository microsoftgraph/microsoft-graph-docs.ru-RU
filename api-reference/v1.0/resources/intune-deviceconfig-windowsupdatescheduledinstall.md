---
title: Тип ресурса windowsUpdateScheduledInstall
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 4a8943fa0275d8b9e5a668be207c90304f22a327
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340917"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="14706-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="14706-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="14706-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="14706-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14706-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="14706-105">Not yet documented</span></span>

<span data-ttu-id="14706-106">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="14706-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="14706-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="14706-107">Properties</span></span>
|<span data-ttu-id="14706-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="14706-108">Property</span></span>|<span data-ttu-id="14706-109">Тип</span><span class="sxs-lookup"><span data-stu-id="14706-109">Type</span></span>|<span data-ttu-id="14706-110">Описание</span><span class="sxs-lookup"><span data-stu-id="14706-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14706-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="14706-111">scheduledInstallDay</span></span>|[<span data-ttu-id="14706-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="14706-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="14706-113">Запланированные Установка день недели.</span><span class="sxs-lookup"><span data-stu-id="14706-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="14706-114">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="14706-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="14706-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="14706-115">scheduledInstallTime</span></span>|<span data-ttu-id="14706-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="14706-116">TimeOfDay</span></span>|<span data-ttu-id="14706-117">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="14706-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="14706-118">Связи</span><span class="sxs-lookup"><span data-stu-id="14706-118">Relationships</span></span>
<span data-ttu-id="14706-119">Нет</span><span class="sxs-lookup"><span data-stu-id="14706-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="14706-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="14706-120">JSON Representation</span></span>
<span data-ttu-id="14706-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14706-121">Here is a JSON representation of the resource.</span></span>
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



