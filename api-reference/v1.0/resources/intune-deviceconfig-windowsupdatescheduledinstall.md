---
title: Тип ресурса windowsUpdateScheduledInstall
description: Н/Д
ms.openlocfilehash: 06e26bfb43691c8774e166a65b36d6ab872d44e1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025886"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="c4ca4-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="c4ca4-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="c4ca4-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c4ca4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4ca4-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c4ca4-105">Not yet documented</span></span>

<span data-ttu-id="c4ca4-106">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="c4ca4-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c4ca4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4ca4-107">Properties</span></span>
|<span data-ttu-id="c4ca4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4ca4-108">Property</span></span>|<span data-ttu-id="c4ca4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c4ca4-109">Type</span></span>|<span data-ttu-id="c4ca4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c4ca4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4ca4-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="c4ca4-111">scheduledInstallDay</span></span>|[<span data-ttu-id="c4ca4-112">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="c4ca4-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="c4ca4-113">Запланированные Установка день недели.</span><span class="sxs-lookup"><span data-stu-id="c4ca4-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="c4ca4-114">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="c4ca4-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="c4ca4-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="c4ca4-115">scheduledInstallTime</span></span>|<span data-ttu-id="c4ca4-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c4ca4-116">TimeOfDay</span></span>|<span data-ttu-id="c4ca4-117">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="c4ca4-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4ca4-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c4ca4-118">Relationships</span></span>
<span data-ttu-id="c4ca4-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c4ca4-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c4ca4-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4ca4-120">JSON Representation</span></span>
<span data-ttu-id="c4ca4-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4ca4-121">Here is a JSON representation of the resource.</span></span>
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



