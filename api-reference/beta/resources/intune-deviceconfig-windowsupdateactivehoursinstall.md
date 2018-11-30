---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Н/Д
ms.openlocfilehash: 7a40a791a9a00d7cfd60287bade1759592e1bcf2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081352"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="f49cd-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="f49cd-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="f49cd-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f49cd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f49cd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f49cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f49cd-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f49cd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f49cd-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f49cd-107">Not yet documented</span></span>

<span data-ttu-id="f49cd-108">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="f49cd-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f49cd-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f49cd-109">Properties</span></span>
|<span data-ttu-id="f49cd-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f49cd-110">Property</span></span>|<span data-ttu-id="f49cd-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f49cd-111">Type</span></span>|<span data-ttu-id="f49cd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f49cd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f49cd-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="f49cd-113">activeHoursStart</span></span>|<span data-ttu-id="f49cd-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f49cd-114">TimeOfDay</span></span>|<span data-ttu-id="f49cd-115">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="f49cd-115">Active Hours Start</span></span>|
|<span data-ttu-id="f49cd-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="f49cd-116">activeHoursEnd</span></span>|<span data-ttu-id="f49cd-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f49cd-117">TimeOfDay</span></span>|<span data-ttu-id="f49cd-118">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="f49cd-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="f49cd-119">Связи</span><span class="sxs-lookup"><span data-stu-id="f49cd-119">Relationships</span></span>
<span data-ttu-id="f49cd-120">Нет</span><span class="sxs-lookup"><span data-stu-id="f49cd-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f49cd-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f49cd-121">JSON Representation</span></span>
<span data-ttu-id="f49cd-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f49cd-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateActiveHoursInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateActiveHoursInstall",
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)"
}
```





