---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 797cfc0f9279f0ab232991a95714d31ce37211a3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818426"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="16e30-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="16e30-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="16e30-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="16e30-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16e30-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16e30-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16e30-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="16e30-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16e30-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="16e30-107">Not yet documented</span></span>

<span data-ttu-id="16e30-108">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="16e30-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="16e30-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="16e30-109">Properties</span></span>
|<span data-ttu-id="16e30-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="16e30-110">Property</span></span>|<span data-ttu-id="16e30-111">Тип</span><span class="sxs-lookup"><span data-stu-id="16e30-111">Type</span></span>|<span data-ttu-id="16e30-112">Описание</span><span class="sxs-lookup"><span data-stu-id="16e30-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16e30-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="16e30-113">activeHoursStart</span></span>|<span data-ttu-id="16e30-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="16e30-114">TimeOfDay</span></span>|<span data-ttu-id="16e30-115">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="16e30-115">Active Hours Start</span></span>|
|<span data-ttu-id="16e30-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="16e30-116">activeHoursEnd</span></span>|<span data-ttu-id="16e30-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="16e30-117">TimeOfDay</span></span>|<span data-ttu-id="16e30-118">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="16e30-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="16e30-119">Связи</span><span class="sxs-lookup"><span data-stu-id="16e30-119">Relationships</span></span>
<span data-ttu-id="16e30-120">Нет</span><span class="sxs-lookup"><span data-stu-id="16e30-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="16e30-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="16e30-121">JSON Representation</span></span>
<span data-ttu-id="16e30-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16e30-122">Here is a JSON representation of the resource.</span></span>
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





