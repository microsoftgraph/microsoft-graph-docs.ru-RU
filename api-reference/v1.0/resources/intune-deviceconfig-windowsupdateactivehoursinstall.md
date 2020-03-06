---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d66aae6ed12abe546b5a7776e864015e20896ee7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530335"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="c7582-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="c7582-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="c7582-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7582-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7582-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7582-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7582-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c7582-106">Not yet documented</span></span>


<span data-ttu-id="c7582-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="c7582-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c7582-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7582-108">Properties</span></span>
|<span data-ttu-id="c7582-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7582-109">Property</span></span>|<span data-ttu-id="c7582-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c7582-110">Type</span></span>|<span data-ttu-id="c7582-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c7582-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7582-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="c7582-112">activeHoursStart</span></span>|<span data-ttu-id="c7582-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c7582-113">TimeOfDay</span></span>|<span data-ttu-id="c7582-114">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="c7582-114">Active Hours Start</span></span>|
|<span data-ttu-id="c7582-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="c7582-115">activeHoursEnd</span></span>|<span data-ttu-id="c7582-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c7582-116">TimeOfDay</span></span>|<span data-ttu-id="c7582-117">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="c7582-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7582-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c7582-118">Relationships</span></span>
<span data-ttu-id="c7582-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c7582-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7582-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c7582-120">JSON Representation</span></span>
<span data-ttu-id="c7582-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7582-121">Here is a JSON representation of the resource.</span></span>
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




