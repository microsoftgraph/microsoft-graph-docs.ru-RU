---
title: Тип ресурса Кустомупдатетимевиндов
description: Настраиваемое окно времени обновления
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7392ba0eeb3af516682ff63f9f65fce94d08f0e9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729793"
---
# <a name="customupdatetimewindow-resource-type"></a><span data-ttu-id="f91fb-103">Тип ресурса Кустомупдатетимевиндов</span><span class="sxs-lookup"><span data-stu-id="f91fb-103">customUpdateTimeWindow resource type</span></span>

<span data-ttu-id="f91fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f91fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f91fb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f91fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f91fb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f91fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f91fb-107">Настраиваемое окно времени обновления</span><span class="sxs-lookup"><span data-stu-id="f91fb-107">Custom update time window</span></span>

## <a name="properties"></a><span data-ttu-id="f91fb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f91fb-108">Properties</span></span>
|<span data-ttu-id="f91fb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f91fb-109">Property</span></span>|<span data-ttu-id="f91fb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f91fb-110">Type</span></span>|<span data-ttu-id="f91fb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f91fb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f91fb-112">стартдай</span><span class="sxs-lookup"><span data-stu-id="f91fb-112">startDay</span></span>|[<span data-ttu-id="f91fb-113">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="f91fb-113">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="f91fb-114">День начала периода времени.</span><span class="sxs-lookup"><span data-stu-id="f91fb-114">Start day of the time window.</span></span> <span data-ttu-id="f91fb-115">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="f91fb-115">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="f91fb-116">енддай</span><span class="sxs-lookup"><span data-stu-id="f91fb-116">endDay</span></span>|[<span data-ttu-id="f91fb-117">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="f91fb-117">dayOfWeek</span></span>](../resources/intune-deviceconfig-dayofweek.md)|<span data-ttu-id="f91fb-118">День окончания периода времени.</span><span class="sxs-lookup"><span data-stu-id="f91fb-118">End day of the time window.</span></span> <span data-ttu-id="f91fb-119">Возможные значения: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span><span class="sxs-lookup"><span data-stu-id="f91fb-119">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="f91fb-120">startTime</span><span class="sxs-lookup"><span data-stu-id="f91fb-120">startTime</span></span>|<span data-ttu-id="f91fb-121">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f91fb-121">TimeOfDay</span></span>|<span data-ttu-id="f91fb-122">Время начала периода времени</span><span class="sxs-lookup"><span data-stu-id="f91fb-122">Start time of the time window</span></span>|
|<span data-ttu-id="f91fb-123">endTime</span><span class="sxs-lookup"><span data-stu-id="f91fb-123">endTime</span></span>|<span data-ttu-id="f91fb-124">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f91fb-124">TimeOfDay</span></span>|<span data-ttu-id="f91fb-125">Время окончания периода времени</span><span class="sxs-lookup"><span data-stu-id="f91fb-125">End time of the time window</span></span>|

## <a name="relationships"></a><span data-ttu-id="f91fb-126">Связи</span><span class="sxs-lookup"><span data-stu-id="f91fb-126">Relationships</span></span>
<span data-ttu-id="f91fb-127">Нет</span><span class="sxs-lookup"><span data-stu-id="f91fb-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f91fb-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f91fb-128">JSON Representation</span></span>
<span data-ttu-id="f91fb-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f91fb-129">Here is a JSON representation of the resource.</span></span>
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





