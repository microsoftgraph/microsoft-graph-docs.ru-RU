---
title: Тип ресурса windowsUpdateScheduledInstall
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ee91ed2541c02adbb7a130f0a9de869d86044632
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395631"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="4f082-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="4f082-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="4f082-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4f082-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4f082-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f082-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4f082-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f082-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f082-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="4f082-107">Not yet documented</span></span>


<span data-ttu-id="4f082-108">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="4f082-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4f082-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f082-109">Properties</span></span>
|<span data-ttu-id="4f082-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f082-110">Property</span></span>|<span data-ttu-id="4f082-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4f082-111">Type</span></span>|<span data-ttu-id="4f082-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4f082-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f082-113">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="4f082-113">scheduledInstallDay</span></span>|[<span data-ttu-id="4f082-114">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="4f082-114">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="4f082-115">Запланированные Установка день недели.</span><span class="sxs-lookup"><span data-stu-id="4f082-115">Scheduled Install Day in week.</span></span> <span data-ttu-id="4f082-116">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="4f082-116">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="4f082-117">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="4f082-117">scheduledInstallTime</span></span>|<span data-ttu-id="4f082-118">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4f082-118">TimeOfDay</span></span>|<span data-ttu-id="4f082-119">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="4f082-119">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f082-120">Связи</span><span class="sxs-lookup"><span data-stu-id="4f082-120">Relationships</span></span>
<span data-ttu-id="4f082-121">Нет</span><span class="sxs-lookup"><span data-stu-id="4f082-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f082-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f082-122">JSON Representation</span></span>
<span data-ttu-id="4f082-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f082-123">Here is a JSON representation of the resource.</span></span>
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




