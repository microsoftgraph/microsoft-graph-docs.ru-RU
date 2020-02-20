---
title: Тип ресурса Кустомупдатетимевиндов
description: Настраиваемое окно времени обновления
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d412f568a48c4da7b41d56b44180ac5200961238
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42161343"
---
# <a name="customupdatetimewindow-resource-type"></a><span data-ttu-id="af4ff-103">Тип ресурса Кустомупдатетимевиндов</span><span class="sxs-lookup"><span data-stu-id="af4ff-103">customUpdateTimeWindow resource type</span></span>

> <span data-ttu-id="af4ff-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af4ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af4ff-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af4ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af4ff-106">Настраиваемое окно времени обновления</span><span class="sxs-lookup"><span data-stu-id="af4ff-106">Custom update time window</span></span>

## <a name="properties"></a><span data-ttu-id="af4ff-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="af4ff-107">Properties</span></span>
|<span data-ttu-id="af4ff-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="af4ff-108">Property</span></span>|<span data-ttu-id="af4ff-109">Тип</span><span class="sxs-lookup"><span data-stu-id="af4ff-109">Type</span></span>|<span data-ttu-id="af4ff-110">Описание</span><span class="sxs-lookup"><span data-stu-id="af4ff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af4ff-111">стартдай</span><span class="sxs-lookup"><span data-stu-id="af4ff-111">startDay</span></span>|[<span data-ttu-id="af4ff-112">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="af4ff-112">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="af4ff-113">День начала периода времени.</span><span class="sxs-lookup"><span data-stu-id="af4ff-113">Start day of the time window.</span></span> <span data-ttu-id="af4ff-114">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="af4ff-114">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="af4ff-115">енддай</span><span class="sxs-lookup"><span data-stu-id="af4ff-115">endDay</span></span>|[<span data-ttu-id="af4ff-116">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="af4ff-116">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="af4ff-117">День окончания периода времени.</span><span class="sxs-lookup"><span data-stu-id="af4ff-117">End day of the time window.</span></span> <span data-ttu-id="af4ff-118">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="af4ff-118">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="af4ff-119">startTime</span><span class="sxs-lookup"><span data-stu-id="af4ff-119">startTime</span></span>|<span data-ttu-id="af4ff-120">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="af4ff-120">TimeOfDay</span></span>|<span data-ttu-id="af4ff-121">Время начала периода времени</span><span class="sxs-lookup"><span data-stu-id="af4ff-121">Start time of the time window</span></span>|
|<span data-ttu-id="af4ff-122">endTime</span><span class="sxs-lookup"><span data-stu-id="af4ff-122">endTime</span></span>|<span data-ttu-id="af4ff-123">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="af4ff-123">TimeOfDay</span></span>|<span data-ttu-id="af4ff-124">Время окончания периода времени</span><span class="sxs-lookup"><span data-stu-id="af4ff-124">End time of the time window</span></span>|

## <a name="relationships"></a><span data-ttu-id="af4ff-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="af4ff-125">Relationships</span></span>
<span data-ttu-id="af4ff-126">Нет</span><span class="sxs-lookup"><span data-stu-id="af4ff-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af4ff-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af4ff-127">JSON Representation</span></span>
<span data-ttu-id="af4ff-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af4ff-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customUpdateTimeWindow"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customUpdateTimeWindow",
  "startDay": "String",
  "endDay": "String",
  "startTime": "String (time of day)",
  "endTime": "String (time of day)"
}
```



