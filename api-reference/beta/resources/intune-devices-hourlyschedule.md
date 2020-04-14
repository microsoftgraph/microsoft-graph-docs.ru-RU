---
title: Тип ресурса Хаурлисчедуле
description: Почасовое расписание выполнения сценария управления повторяющимся устройством.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2eae0d244eb78e006f74c127a81df1786bc9bd8f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470615"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="d86c6-103">Тип ресурса Хаурлисчедуле</span><span class="sxs-lookup"><span data-stu-id="d86c6-103">hourlySchedule resource type</span></span>

<span data-ttu-id="d86c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d86c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d86c6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d86c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d86c6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d86c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d86c6-107">Почасовое расписание выполнения сценария управления повторяющимся устройством.</span><span class="sxs-lookup"><span data-stu-id="d86c6-107">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="d86c6-108">Наследуется от [рунсчедуле](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="d86c6-108">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d86c6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d86c6-109">Properties</span></span>
|<span data-ttu-id="d86c6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d86c6-110">Property</span></span>|<span data-ttu-id="d86c6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d86c6-111">Type</span></span>|<span data-ttu-id="d86c6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d86c6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d86c6-113">interval</span><span class="sxs-lookup"><span data-stu-id="d86c6-113">interval</span></span>|<span data-ttu-id="d86c6-114">Int32</span><span class="sxs-lookup"><span data-stu-id="d86c6-114">Int32</span></span>|<span data-ttu-id="d86c6-115">Интервал (в часах)</span><span class="sxs-lookup"><span data-stu-id="d86c6-115">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="d86c6-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="d86c6-116">Relationships</span></span>
<span data-ttu-id="d86c6-117">Нет</span><span class="sxs-lookup"><span data-stu-id="d86c6-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d86c6-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d86c6-118">JSON Representation</span></span>
<span data-ttu-id="d86c6-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d86c6-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hourlySchedule",
  "interval": 1024
}
```



