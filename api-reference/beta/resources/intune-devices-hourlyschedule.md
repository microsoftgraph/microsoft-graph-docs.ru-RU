---
title: Тип ресурса Хаурлисчедуле
description: Почасовое расписание выполнения сценария управления повторяющимся устройством.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 78afa43149f35645f2167a8f593124f01ea11c12
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369901"
---
# <a name="hourlyschedule-resource-type"></a><span data-ttu-id="de8a1-103">Тип ресурса Хаурлисчедуле</span><span class="sxs-lookup"><span data-stu-id="de8a1-103">hourlySchedule resource type</span></span>

> <span data-ttu-id="de8a1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de8a1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de8a1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de8a1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de8a1-106">Почасовое расписание выполнения сценария управления повторяющимся устройством.</span><span class="sxs-lookup"><span data-stu-id="de8a1-106">Hourly run schedule of a recurring device management script.</span></span>


<span data-ttu-id="de8a1-107">Наследуется от [рунсчедуле](../resources/intune-devices-runschedule.md)</span><span class="sxs-lookup"><span data-stu-id="de8a1-107">Inherits from [runSchedule](../resources/intune-devices-runschedule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="de8a1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="de8a1-108">Properties</span></span>
|<span data-ttu-id="de8a1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="de8a1-109">Property</span></span>|<span data-ttu-id="de8a1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="de8a1-110">Type</span></span>|<span data-ttu-id="de8a1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="de8a1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de8a1-112">interval</span><span class="sxs-lookup"><span data-stu-id="de8a1-112">interval</span></span>|<span data-ttu-id="de8a1-113">Int32</span><span class="sxs-lookup"><span data-stu-id="de8a1-113">Int32</span></span>|<span data-ttu-id="de8a1-114">Интервал (в часах)</span><span class="sxs-lookup"><span data-stu-id="de8a1-114">Interval in number of hours</span></span>|

## <a name="relationships"></a><span data-ttu-id="de8a1-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="de8a1-115">Relationships</span></span>
<span data-ttu-id="de8a1-116">Нет</span><span class="sxs-lookup"><span data-stu-id="de8a1-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de8a1-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de8a1-117">JSON Representation</span></span>
<span data-ttu-id="de8a1-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de8a1-118">Here is a JSON representation of the resource.</span></span>
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



