---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 81ccc29bfe0eb9c3d0d943975807cbf5776051a9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758766"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="cb0d9-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="cb0d9-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="cb0d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb0d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb0d9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb0d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb0d9-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cb0d9-106">Not yet documented</span></span>


<span data-ttu-id="cb0d9-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="cb0d9-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cb0d9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb0d9-108">Properties</span></span>
|<span data-ttu-id="cb0d9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb0d9-109">Property</span></span>|<span data-ttu-id="cb0d9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cb0d9-110">Type</span></span>|<span data-ttu-id="cb0d9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cb0d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb0d9-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="cb0d9-112">activeHoursStart</span></span>|<span data-ttu-id="cb0d9-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="cb0d9-113">TimeOfDay</span></span>|<span data-ttu-id="cb0d9-114">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="cb0d9-114">Active Hours Start</span></span>|
|<span data-ttu-id="cb0d9-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="cb0d9-115">activeHoursEnd</span></span>|<span data-ttu-id="cb0d9-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="cb0d9-116">TimeOfDay</span></span>|<span data-ttu-id="cb0d9-117">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="cb0d9-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb0d9-118">Связи</span><span class="sxs-lookup"><span data-stu-id="cb0d9-118">Relationships</span></span>
<span data-ttu-id="cb0d9-119">Нет</span><span class="sxs-lookup"><span data-stu-id="cb0d9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb0d9-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb0d9-120">JSON Representation</span></span>
<span data-ttu-id="cb0d9-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb0d9-121">Here is a JSON representation of the resource.</span></span>
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




