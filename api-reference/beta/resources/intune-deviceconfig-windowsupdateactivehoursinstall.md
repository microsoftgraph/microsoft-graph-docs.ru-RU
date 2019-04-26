---
title: Тип ресурса windowsUpdateActiveHoursInstall
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f65d986fa59a3087a5fe1578eec626a27a4154b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555194"
---
# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="0ce7a-103">Тип ресурса windowsUpdateActiveHoursInstall</span><span class="sxs-lookup"><span data-stu-id="0ce7a-103">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="0ce7a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ce7a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ce7a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ce7a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ce7a-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0ce7a-106">Not yet documented</span></span>


<span data-ttu-id="0ce7a-107">Наследуется от [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span><span class="sxs-lookup"><span data-stu-id="0ce7a-107">Inherits from [windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0ce7a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ce7a-108">Properties</span></span>
|<span data-ttu-id="0ce7a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ce7a-109">Property</span></span>|<span data-ttu-id="0ce7a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0ce7a-110">Type</span></span>|<span data-ttu-id="0ce7a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0ce7a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ce7a-112">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="0ce7a-112">activeHoursStart</span></span>|<span data-ttu-id="0ce7a-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0ce7a-113">TimeOfDay</span></span>|<span data-ttu-id="0ce7a-114">Время начала периода активности</span><span class="sxs-lookup"><span data-stu-id="0ce7a-114">Active Hours Start</span></span>|
|<span data-ttu-id="0ce7a-115">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="0ce7a-115">activeHoursEnd</span></span>|<span data-ttu-id="0ce7a-116">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0ce7a-116">TimeOfDay</span></span>|<span data-ttu-id="0ce7a-117">Время окончания периода активности</span><span class="sxs-lookup"><span data-stu-id="0ce7a-117">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ce7a-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="0ce7a-118">Relationships</span></span>
<span data-ttu-id="0ce7a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0ce7a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ce7a-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0ce7a-120">JSON Representation</span></span>
<span data-ttu-id="0ce7a-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ce7a-121">Here is a JSON representation of the resource.</span></span>
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





