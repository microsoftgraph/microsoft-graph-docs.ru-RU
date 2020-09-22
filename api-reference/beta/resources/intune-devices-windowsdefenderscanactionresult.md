---
title: Тип ресурса windowsDefenderScanActionResult
description: Результат последнего сканирования, выполненного Защитником Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e9fcddceae21218978b121ae8b5749c739f3d105
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080749"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="b3ef6-103">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="b3ef6-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="b3ef6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3ef6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3ef6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3ef6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3ef6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3ef6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3ef6-107">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="b3ef6-107">Windows Defender last scan result</span></span>


<span data-ttu-id="b3ef6-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b3ef6-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b3ef6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3ef6-109">Properties</span></span>
|<span data-ttu-id="b3ef6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3ef6-110">Property</span></span>|<span data-ttu-id="b3ef6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b3ef6-111">Type</span></span>|<span data-ttu-id="b3ef6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b3ef6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3ef6-113">actionName</span><span class="sxs-lookup"><span data-stu-id="b3ef6-113">actionName</span></span>|<span data-ttu-id="b3ef6-114">String</span><span class="sxs-lookup"><span data-stu-id="b3ef6-114">String</span></span>|<span data-ttu-id="b3ef6-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b3ef6-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b3ef6-116">actionState</span><span class="sxs-lookup"><span data-stu-id="b3ef6-116">actionState</span></span>|[<span data-ttu-id="b3ef6-117">actionState</span><span class="sxs-lookup"><span data-stu-id="b3ef6-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="b3ef6-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b3ef6-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b3ef6-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b3ef6-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b3ef6-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b3ef6-120">startDateTime</span></span>|<span data-ttu-id="b3ef6-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3ef6-121">DateTimeOffset</span></span>|<span data-ttu-id="b3ef6-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b3ef6-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b3ef6-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3ef6-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="b3ef6-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3ef6-124">DateTimeOffset</span></span>|<span data-ttu-id="b3ef6-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b3ef6-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b3ef6-126">scanType</span><span class="sxs-lookup"><span data-stu-id="b3ef6-126">scanType</span></span>|<span data-ttu-id="b3ef6-127">String</span><span class="sxs-lookup"><span data-stu-id="b3ef6-127">String</span></span>|<span data-ttu-id="b3ef6-128">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="b3ef6-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3ef6-129">Связи</span><span class="sxs-lookup"><span data-stu-id="b3ef6-129">Relationships</span></span>
<span data-ttu-id="b3ef6-130">Нет</span><span class="sxs-lookup"><span data-stu-id="b3ef6-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3ef6-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b3ef6-131">JSON Representation</span></span>
<span data-ttu-id="b3ef6-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3ef6-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderScanActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "scanType": "String"
}
```






