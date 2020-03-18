---
title: Тип ресурса Кустомупдатетимевиндов
description: Настраиваемое окно времени обновления
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f56cf571b24c2bcee52e82100f5c087772c336e5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795647"
---
# <a name="customupdatetimewindow-resource-type"></a><span data-ttu-id="319db-103">Тип ресурса Кустомупдатетимевиндов</span><span class="sxs-lookup"><span data-stu-id="319db-103">customUpdateTimeWindow resource type</span></span>

> <span data-ttu-id="319db-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="319db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="319db-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="319db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="319db-106">Настраиваемое окно времени обновления</span><span class="sxs-lookup"><span data-stu-id="319db-106">Custom update time window</span></span>

## <a name="properties"></a><span data-ttu-id="319db-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="319db-107">Properties</span></span>
|<span data-ttu-id="319db-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="319db-108">Property</span></span>|<span data-ttu-id="319db-109">Тип</span><span class="sxs-lookup"><span data-stu-id="319db-109">Type</span></span>|<span data-ttu-id="319db-110">Описание</span><span class="sxs-lookup"><span data-stu-id="319db-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="319db-111">стартдай</span><span class="sxs-lookup"><span data-stu-id="319db-111">startDay</span></span>|[<span data-ttu-id="319db-112">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="319db-112">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="319db-113">День начала периода времени.</span><span class="sxs-lookup"><span data-stu-id="319db-113">Start day of the time window.</span></span> <span data-ttu-id="319db-114">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="319db-114">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="319db-115">енддай</span><span class="sxs-lookup"><span data-stu-id="319db-115">endDay</span></span>|[<span data-ttu-id="319db-116">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="319db-116">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="319db-117">День окончания периода времени.</span><span class="sxs-lookup"><span data-stu-id="319db-117">End day of the time window.</span></span> <span data-ttu-id="319db-118">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="319db-118">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="319db-119">startTime</span><span class="sxs-lookup"><span data-stu-id="319db-119">startTime</span></span>|<span data-ttu-id="319db-120">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="319db-120">TimeOfDay</span></span>|<span data-ttu-id="319db-121">Время начала периода времени</span><span class="sxs-lookup"><span data-stu-id="319db-121">Start time of the time window</span></span>|
|<span data-ttu-id="319db-122">endTime</span><span class="sxs-lookup"><span data-stu-id="319db-122">endTime</span></span>|<span data-ttu-id="319db-123">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="319db-123">TimeOfDay</span></span>|<span data-ttu-id="319db-124">Время окончания периода времени</span><span class="sxs-lookup"><span data-stu-id="319db-124">End time of the time window</span></span>|

## <a name="relationships"></a><span data-ttu-id="319db-125">Связи</span><span class="sxs-lookup"><span data-stu-id="319db-125">Relationships</span></span>
<span data-ttu-id="319db-126">Нет</span><span class="sxs-lookup"><span data-stu-id="319db-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="319db-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="319db-127">JSON Representation</span></span>
<span data-ttu-id="319db-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="319db-128">Here is a JSON representation of the resource.</span></span>
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



