---
title: Тип ресурса windowsDefenderScanActionResult
description: Результат последнего сканирования, выполненного Защитником Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3fce56be7dcc0d1262bb65420d6ce3986cce1fe3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530270"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="2e3c6-103">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="2e3c6-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="2e3c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e3c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e3c6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e3c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e3c6-106">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="2e3c6-106">Windows Defender last scan result</span></span>


<span data-ttu-id="2e3c6-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2e3c6-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2e3c6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e3c6-108">Properties</span></span>
|<span data-ttu-id="2e3c6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e3c6-109">Property</span></span>|<span data-ttu-id="2e3c6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2e3c6-110">Type</span></span>|<span data-ttu-id="2e3c6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2e3c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e3c6-112">actionName</span><span class="sxs-lookup"><span data-stu-id="2e3c6-112">actionName</span></span>|<span data-ttu-id="2e3c6-113">Строка</span><span class="sxs-lookup"><span data-stu-id="2e3c6-113">String</span></span>|<span data-ttu-id="2e3c6-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="2e3c6-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2e3c6-115">actionState</span><span class="sxs-lookup"><span data-stu-id="2e3c6-115">actionState</span></span>|[<span data-ttu-id="2e3c6-116">actionState</span><span class="sxs-lookup"><span data-stu-id="2e3c6-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="2e3c6-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="2e3c6-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="2e3c6-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="2e3c6-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="2e3c6-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2e3c6-119">startDateTime</span></span>|<span data-ttu-id="2e3c6-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e3c6-120">DateTimeOffset</span></span>|<span data-ttu-id="2e3c6-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="2e3c6-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2e3c6-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e3c6-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="2e3c6-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e3c6-123">DateTimeOffset</span></span>|<span data-ttu-id="2e3c6-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="2e3c6-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2e3c6-125">scanType</span><span class="sxs-lookup"><span data-stu-id="2e3c6-125">scanType</span></span>|<span data-ttu-id="2e3c6-126">String</span><span class="sxs-lookup"><span data-stu-id="2e3c6-126">String</span></span>|<span data-ttu-id="2e3c6-127">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="2e3c6-127">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e3c6-128">Связи</span><span class="sxs-lookup"><span data-stu-id="2e3c6-128">Relationships</span></span>
<span data-ttu-id="2e3c6-129">Нет</span><span class="sxs-lookup"><span data-stu-id="2e3c6-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e3c6-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e3c6-130">JSON Representation</span></span>
<span data-ttu-id="2e3c6-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e3c6-131">Here is a JSON representation of the resource.</span></span>
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




