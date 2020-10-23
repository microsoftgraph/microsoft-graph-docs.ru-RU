---
title: Тип ресурса windowsDefenderScanActionResult
description: Результат последнего сканирования, выполненного Защитником Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 221fee2c96170534a6c20c151b813497598f774f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727374"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="90177-103">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="90177-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="90177-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90177-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90177-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90177-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90177-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90177-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90177-107">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="90177-107">Windows Defender last scan result</span></span>


<span data-ttu-id="90177-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="90177-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="90177-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="90177-109">Properties</span></span>
|<span data-ttu-id="90177-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="90177-110">Property</span></span>|<span data-ttu-id="90177-111">Тип</span><span class="sxs-lookup"><span data-stu-id="90177-111">Type</span></span>|<span data-ttu-id="90177-112">Описание</span><span class="sxs-lookup"><span data-stu-id="90177-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90177-113">actionName</span><span class="sxs-lookup"><span data-stu-id="90177-113">actionName</span></span>|<span data-ttu-id="90177-114">String</span><span class="sxs-lookup"><span data-stu-id="90177-114">String</span></span>|<span data-ttu-id="90177-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="90177-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="90177-116">actionState</span><span class="sxs-lookup"><span data-stu-id="90177-116">actionState</span></span>|[<span data-ttu-id="90177-117">actionState</span><span class="sxs-lookup"><span data-stu-id="90177-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="90177-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="90177-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="90177-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="90177-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="90177-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="90177-120">startDateTime</span></span>|<span data-ttu-id="90177-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90177-121">DateTimeOffset</span></span>|<span data-ttu-id="90177-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="90177-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="90177-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="90177-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="90177-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90177-124">DateTimeOffset</span></span>|<span data-ttu-id="90177-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="90177-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="90177-126">scanType</span><span class="sxs-lookup"><span data-stu-id="90177-126">scanType</span></span>|<span data-ttu-id="90177-127">String</span><span class="sxs-lookup"><span data-stu-id="90177-127">String</span></span>|<span data-ttu-id="90177-128">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="90177-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="90177-129">Связи</span><span class="sxs-lookup"><span data-stu-id="90177-129">Relationships</span></span>
<span data-ttu-id="90177-130">Нет</span><span class="sxs-lookup"><span data-stu-id="90177-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90177-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="90177-131">JSON Representation</span></span>
<span data-ttu-id="90177-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90177-132">Here is a JSON representation of the resource.</span></span>
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





