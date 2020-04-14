---
title: Тип ресурса Кустомупдатетимевиндов
description: Настраиваемое окно времени обновления
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b7a83637e3462d33745a14dead15eb86cbb86337
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402170"
---
# <a name="customupdatetimewindow-resource-type"></a><span data-ttu-id="971fe-103">Тип ресурса Кустомупдатетимевиндов</span><span class="sxs-lookup"><span data-stu-id="971fe-103">customUpdateTimeWindow resource type</span></span>

<span data-ttu-id="971fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="971fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="971fe-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="971fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="971fe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="971fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="971fe-107">Настраиваемое окно времени обновления</span><span class="sxs-lookup"><span data-stu-id="971fe-107">Custom update time window</span></span>

## <a name="properties"></a><span data-ttu-id="971fe-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="971fe-108">Properties</span></span>
|<span data-ttu-id="971fe-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="971fe-109">Property</span></span>|<span data-ttu-id="971fe-110">Тип</span><span class="sxs-lookup"><span data-stu-id="971fe-110">Type</span></span>|<span data-ttu-id="971fe-111">Описание</span><span class="sxs-lookup"><span data-stu-id="971fe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="971fe-112">стартдай</span><span class="sxs-lookup"><span data-stu-id="971fe-112">startDay</span></span>|[<span data-ttu-id="971fe-113">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="971fe-113">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="971fe-114">День начала периода времени.</span><span class="sxs-lookup"><span data-stu-id="971fe-114">Start day of the time window.</span></span> <span data-ttu-id="971fe-115">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="971fe-115">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="971fe-116">енддай</span><span class="sxs-lookup"><span data-stu-id="971fe-116">endDay</span></span>|[<span data-ttu-id="971fe-117">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="971fe-117">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="971fe-118">День окончания периода времени.</span><span class="sxs-lookup"><span data-stu-id="971fe-118">End day of the time window.</span></span> <span data-ttu-id="971fe-119">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="971fe-119">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="971fe-120">startTime</span><span class="sxs-lookup"><span data-stu-id="971fe-120">startTime</span></span>|<span data-ttu-id="971fe-121">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="971fe-121">TimeOfDay</span></span>|<span data-ttu-id="971fe-122">Время начала периода времени</span><span class="sxs-lookup"><span data-stu-id="971fe-122">Start time of the time window</span></span>|
|<span data-ttu-id="971fe-123">endTime</span><span class="sxs-lookup"><span data-stu-id="971fe-123">endTime</span></span>|<span data-ttu-id="971fe-124">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="971fe-124">TimeOfDay</span></span>|<span data-ttu-id="971fe-125">Время окончания периода времени</span><span class="sxs-lookup"><span data-stu-id="971fe-125">End time of the time window</span></span>|

## <a name="relationships"></a><span data-ttu-id="971fe-126">Связи</span><span class="sxs-lookup"><span data-stu-id="971fe-126">Relationships</span></span>
<span data-ttu-id="971fe-127">Нет</span><span class="sxs-lookup"><span data-stu-id="971fe-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="971fe-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="971fe-128">JSON Representation</span></span>
<span data-ttu-id="971fe-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="971fe-129">Here is a JSON representation of the resource.</span></span>
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



