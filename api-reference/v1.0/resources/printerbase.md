---
title: тип ресурса printerBase
description: Представляет базовый тип для обмена принтерами и принтерами
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 515c14bb4de7352a8c17cffdacbd7a4c9091fc70
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517332"
---
# <a name="printerbase-resource-type"></a><span data-ttu-id="e44ab-103">тип ресурса printerBase</span><span class="sxs-lookup"><span data-stu-id="e44ab-103">printerBase resource type</span></span>

<span data-ttu-id="e44ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e44ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="e44ab-105">Представляет базовый тип для [типов сущности](printer.md) [принтера и принтераShare.](printerShare.md)</span><span class="sxs-lookup"><span data-stu-id="e44ab-105">Represents a base type for [printer](printer.md) and [printerShare](printerShare.md) entity types.</span></span>

## <a name="properties"></a><span data-ttu-id="e44ab-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e44ab-106">Properties</span></span>
|<span data-ttu-id="e44ab-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e44ab-107">Property</span></span>|<span data-ttu-id="e44ab-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e44ab-108">Type</span></span>|<span data-ttu-id="e44ab-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e44ab-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e44ab-110">capabilities</span><span class="sxs-lookup"><span data-stu-id="e44ab-110">capabilities</span></span>|[<span data-ttu-id="e44ab-111">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="e44ab-111">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="e44ab-112">Возможности принтера и принтераShare.</span><span class="sxs-lookup"><span data-stu-id="e44ab-112">The capabilities of the printer/printerShare.</span></span>|
|<span data-ttu-id="e44ab-113">defaults</span><span class="sxs-lookup"><span data-stu-id="e44ab-113">defaults</span></span>|[<span data-ttu-id="e44ab-114">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="e44ab-114">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="e44ab-115">Параметры печати принтера и принтера По умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e44ab-115">The default print settings of printer/printerShare.</span></span>|
|<span data-ttu-id="e44ab-116">displayName</span><span class="sxs-lookup"><span data-stu-id="e44ab-116">displayName</span></span>|<span data-ttu-id="e44ab-117">Строка</span><span class="sxs-lookup"><span data-stu-id="e44ab-117">String</span></span>|<span data-ttu-id="e44ab-118">Имя принтера/принтераShare.</span><span class="sxs-lookup"><span data-stu-id="e44ab-118">The name of the printer/printerShare.</span></span>|
|<span data-ttu-id="e44ab-119">id</span><span class="sxs-lookup"><span data-stu-id="e44ab-119">id</span></span>|<span data-ttu-id="e44ab-120">Строка</span><span class="sxs-lookup"><span data-stu-id="e44ab-120">String</span></span>|<span data-ttu-id="e44ab-121">Идентификатор.</span><span class="sxs-lookup"><span data-stu-id="e44ab-121">The identifier.</span></span>|
|<span data-ttu-id="e44ab-122">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="e44ab-122">isAcceptingJobs</span></span>|<span data-ttu-id="e44ab-123">Логический</span><span class="sxs-lookup"><span data-stu-id="e44ab-123">Boolean</span></span>|<span data-ttu-id="e44ab-124">Принимает ли принтер или принтер в настоящее время новые задания печати.</span><span class="sxs-lookup"><span data-stu-id="e44ab-124">Whether the printer/printerShare is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="e44ab-125">location</span><span class="sxs-lookup"><span data-stu-id="e44ab-125">location</span></span>|[<span data-ttu-id="e44ab-126">printerLocation</span><span class="sxs-lookup"><span data-stu-id="e44ab-126">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="e44ab-127">Физическое и/или организационное расположение принтера/принтераShare.</span><span class="sxs-lookup"><span data-stu-id="e44ab-127">The physical and/or organizational location of the printer/printerShare.</span></span>|
|<span data-ttu-id="e44ab-128">manufacturer</span><span class="sxs-lookup"><span data-stu-id="e44ab-128">manufacturer</span></span>|<span data-ttu-id="e44ab-129">String</span><span class="sxs-lookup"><span data-stu-id="e44ab-129">String</span></span>|<span data-ttu-id="e44ab-130">Производитель принтера и принтераShare.</span><span class="sxs-lookup"><span data-stu-id="e44ab-130">The manufacturer of the printer/printerShare.</span></span>|
|<span data-ttu-id="e44ab-131">model</span><span class="sxs-lookup"><span data-stu-id="e44ab-131">model</span></span>|<span data-ttu-id="e44ab-132">String</span><span class="sxs-lookup"><span data-stu-id="e44ab-132">String</span></span>|<span data-ttu-id="e44ab-133">Имя модели принтера/принтераShare.</span><span class="sxs-lookup"><span data-stu-id="e44ab-133">The model name of the printer/printerShare.</span></span>|
|<span data-ttu-id="e44ab-134">status</span><span class="sxs-lookup"><span data-stu-id="e44ab-134">status</span></span>|[<span data-ttu-id="e44ab-135">printerStatus</span><span class="sxs-lookup"><span data-stu-id="e44ab-135">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="e44ab-136">Состояние обработки принтера и принтераShare, включая ошибки.</span><span class="sxs-lookup"><span data-stu-id="e44ab-136">The processing status of the printer/printerShare, including any errors.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e44ab-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="e44ab-137">Relationships</span></span>
|<span data-ttu-id="e44ab-138">Связь</span><span class="sxs-lookup"><span data-stu-id="e44ab-138">Relationship</span></span>|<span data-ttu-id="e44ab-139">Тип</span><span class="sxs-lookup"><span data-stu-id="e44ab-139">Type</span></span>|<span data-ttu-id="e44ab-140">Описание</span><span class="sxs-lookup"><span data-stu-id="e44ab-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e44ab-141">jobs</span><span class="sxs-lookup"><span data-stu-id="e44ab-141">jobs</span></span>|<span data-ttu-id="e44ab-142">[коллекция printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="e44ab-142">[printJob](printjob.md) collection</span></span>|<span data-ttu-id="e44ab-143">Список заданий, которые стоят в очереди для печати принтером или принтеромShare.</span><span class="sxs-lookup"><span data-stu-id="e44ab-143">The list of jobs that are queued for printing by the printer/printerShare.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e44ab-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e44ab-144">JSON representation</span></span>
<span data-ttu-id="e44ab-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e44ab-145">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printerBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerBase",
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "isAcceptingJobs": "Boolean",
  "defaults": {
    "@odata.type": "microsoft.graph.printerDefaults"
  },
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "capabilities": {
    "@odata.type": "microsoft.graph.printerCapabilities"
  },
  "status": {
    "@odata.type": "microsoft.graph.printerStatus"
  }
}
```

