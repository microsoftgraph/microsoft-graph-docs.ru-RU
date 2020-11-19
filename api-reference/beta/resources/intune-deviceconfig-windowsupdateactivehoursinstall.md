---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d217a9c6b3cb73a15a863491798115fef3a4c556
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49231321"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="7c0b8-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="7c0b8-103">windowsUpdateActiveHoursInstall resource type</span></span>

<span data-ttu-id="7c0b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c0b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c0b8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c0b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c0b8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c0b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c0b8-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7c0b8-107">Not yet documented</span></span>


<span data-ttu-id="7c0b8-108">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="7c0b8-108">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7c0b8-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c0b8-109">Properties</span></span>
|<span data-ttu-id="7c0b8-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c0b8-110">Property</span></span>|<span data-ttu-id="7c0b8-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7c0b8-111">Type</span></span>|<span data-ttu-id="7c0b8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7c0b8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c0b8-113">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="7c0b8-113">activeHoursStart</span></span>|<span data-ttu-id="7c0b8-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7c0b8-114">TimeOfDay</span></span>|<span data-ttu-id="7c0b8-115">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="7c0b8-115">Active Hours Start</span></span>|
|<span data-ttu-id="7c0b8-116">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="7c0b8-116">activeHoursEnd</span></span>|<span data-ttu-id="7c0b8-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7c0b8-117">TimeOfDay</span></span>|<span data-ttu-id="7c0b8-118">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="7c0b8-118">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c0b8-119">Связи</span><span class="sxs-lookup"><span data-stu-id="7c0b8-119">Relationships</span></span>
<span data-ttu-id="7c0b8-120">Нет</span><span class="sxs-lookup"><span data-stu-id="7c0b8-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c0b8-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c0b8-121">JSON Representation</span></span>
<span data-ttu-id="7c0b8-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c0b8-122">Here is a JSON representation of the resource.</span></span>
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




