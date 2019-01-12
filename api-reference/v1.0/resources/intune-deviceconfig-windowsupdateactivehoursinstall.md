---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ed4f909db5dd31195ace7d98151b226b03849c81
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967184"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="849dd-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="849dd-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="849dd-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="849dd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="849dd-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="849dd-105">Not yet documented</span></span>

<span data-ttu-id="849dd-106">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="849dd-106">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="849dd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="849dd-107">Properties</span></span>
|<span data-ttu-id="849dd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="849dd-108">Property</span></span>|<span data-ttu-id="849dd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="849dd-109">Type</span></span>|<span data-ttu-id="849dd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="849dd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="849dd-111">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="849dd-111">activeHoursStart</span></span>|<span data-ttu-id="849dd-112">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="849dd-112">TimeOfDay</span></span>|<span data-ttu-id="849dd-113">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="849dd-113">Active Hours Start</span></span>|
|<span data-ttu-id="849dd-114">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="849dd-114">activeHoursEnd</span></span>|<span data-ttu-id="849dd-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="849dd-115">TimeOfDay</span></span>|<span data-ttu-id="849dd-116">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="849dd-116">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="849dd-117">Связи</span><span class="sxs-lookup"><span data-stu-id="849dd-117">Relationships</span></span>
<span data-ttu-id="849dd-118">Нет</span><span class="sxs-lookup"><span data-stu-id="849dd-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="849dd-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="849dd-119">JSON Representation</span></span>
<span data-ttu-id="849dd-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="849dd-120">Here is a JSON representation of the resource.</span></span>
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



