---
title: Тип ресурса windowsUpdateScheduledInstall
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 47518277f54526e84cc3152a96ba3b49ec8a199e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836003"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="d2a07-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="d2a07-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="d2a07-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d2a07-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2a07-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2a07-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2a07-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d2a07-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2a07-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d2a07-107">Not yet documented</span></span>

<span data-ttu-id="d2a07-108">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="d2a07-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d2a07-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2a07-109">Properties</span></span>
|<span data-ttu-id="d2a07-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2a07-110">Property</span></span>|<span data-ttu-id="d2a07-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d2a07-111">Type</span></span>|<span data-ttu-id="d2a07-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d2a07-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2a07-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="d2a07-113">scheduledInstallDay</span></span>|[<span data-ttu-id="d2a07-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="d2a07-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="d2a07-115">Запланированные Установка день недели.</span><span class="sxs-lookup"><span data-stu-id="d2a07-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="d2a07-116">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="d2a07-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="d2a07-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="d2a07-117">scheduledInstallTime</span></span>|<span data-ttu-id="d2a07-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d2a07-118">TimeOfDay</span></span>|<span data-ttu-id="d2a07-119">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="d2a07-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2a07-120">Связи</span><span class="sxs-lookup"><span data-stu-id="d2a07-120">Relationships</span></span>
<span data-ttu-id="d2a07-121">Нет</span><span class="sxs-lookup"><span data-stu-id="d2a07-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d2a07-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2a07-122">JSON Representation</span></span>
<span data-ttu-id="d2a07-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2a07-123">Here is a JSON representation of the resource.</span></span>
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





