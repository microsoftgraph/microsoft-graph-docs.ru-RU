---
title: Тип ресурса windowsUpdateScheduledInstall
description: Н/Д
ms.openlocfilehash: 9f39a9716efed39529c54eaddc62cde075b51954
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076874"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="90ad7-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="90ad7-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="90ad7-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="90ad7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90ad7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90ad7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="90ad7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="90ad7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90ad7-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="90ad7-107">Not yet documented</span></span>

<span data-ttu-id="90ad7-108">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="90ad7-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="90ad7-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="90ad7-109">Properties</span></span>
|<span data-ttu-id="90ad7-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="90ad7-110">Property</span></span>|<span data-ttu-id="90ad7-111">Тип</span><span class="sxs-lookup"><span data-stu-id="90ad7-111">Type</span></span>|<span data-ttu-id="90ad7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="90ad7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90ad7-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="90ad7-113">scheduledInstallDay</span></span>|[<span data-ttu-id="90ad7-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="90ad7-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="90ad7-115">Запланированные Установка день недели.</span><span class="sxs-lookup"><span data-stu-id="90ad7-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="90ad7-116">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="90ad7-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="90ad7-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="90ad7-117">scheduledInstallTime</span></span>|<span data-ttu-id="90ad7-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="90ad7-118">TimeOfDay</span></span>|<span data-ttu-id="90ad7-119">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="90ad7-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="90ad7-120">Связи</span><span class="sxs-lookup"><span data-stu-id="90ad7-120">Relationships</span></span>
<span data-ttu-id="90ad7-121">Нет</span><span class="sxs-lookup"><span data-stu-id="90ad7-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="90ad7-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="90ad7-122">JSON Representation</span></span>
<span data-ttu-id="90ad7-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90ad7-123">Here is a JSON representation of the resource.</span></span>
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





