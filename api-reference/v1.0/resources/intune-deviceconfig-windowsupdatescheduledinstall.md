---
title: Тип ресурса windowsUpdateScheduledInstall
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b8f0eea6eb81f9e06243101bb2433fbcafaecae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503578"
---
# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="b8ef0-103">Тип ресурса windowsUpdateScheduledInstall</span><span class="sxs-lookup"><span data-stu-id="b8ef0-103">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="b8ef0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8ef0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8ef0-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b8ef0-105">Not yet documented</span></span>


<span data-ttu-id="b8ef0-106">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="b8ef0-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b8ef0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8ef0-107">Properties</span></span>
|<span data-ttu-id="b8ef0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8ef0-108">Property</span></span>|<span data-ttu-id="b8ef0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b8ef0-109">Type</span></span>|<span data-ttu-id="b8ef0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b8ef0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8ef0-111">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="b8ef0-111">scheduledInstallDay</span></span>|[<span data-ttu-id="b8ef0-112">Виклисчедуле</span><span class="sxs-lookup"><span data-stu-id="b8ef0-112">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="b8ef0-113">Запланированный день установки по неделям.</span><span class="sxs-lookup"><span data-stu-id="b8ef0-113">Scheduled Install Day in week.</span></span> <span data-ttu-id="b8ef0-114">Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="b8ef0-114">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="b8ef0-115">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="b8ef0-115">scheduledInstallTime</span></span>|<span data-ttu-id="b8ef0-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b8ef0-116">TimeOfDay</span></span>|<span data-ttu-id="b8ef0-117">Время дня, на которое запланирована установка</span><span class="sxs-lookup"><span data-stu-id="b8ef0-117">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8ef0-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="b8ef0-118">Relationships</span></span>
<span data-ttu-id="b8ef0-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b8ef0-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8ef0-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8ef0-120">JSON Representation</span></span>
<span data-ttu-id="b8ef0-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8ef0-121">Here is a JSON representation of the resource.</span></span>
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



