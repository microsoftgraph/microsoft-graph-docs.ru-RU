---
title: Тип ресурса windowsDefenderScanActionResult
description: Результат последнего сканирования, выполненного Защитником Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1ce77c0e034cacf301dfdfa5df96070bd1944160
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356886"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="55756-103">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="55756-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="55756-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55756-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55756-105">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="55756-105">Windows Defender last scan result</span></span>


<span data-ttu-id="55756-106">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="55756-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="55756-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="55756-107">Properties</span></span>
|<span data-ttu-id="55756-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="55756-108">Property</span></span>|<span data-ttu-id="55756-109">Тип</span><span class="sxs-lookup"><span data-stu-id="55756-109">Type</span></span>|<span data-ttu-id="55756-110">Описание</span><span class="sxs-lookup"><span data-stu-id="55756-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55756-111">actionName</span><span class="sxs-lookup"><span data-stu-id="55756-111">actionName</span></span>|<span data-ttu-id="55756-112">String</span><span class="sxs-lookup"><span data-stu-id="55756-112">String</span></span>|<span data-ttu-id="55756-113">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="55756-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="55756-114">actionState</span><span class="sxs-lookup"><span data-stu-id="55756-114">actionState</span></span>|[<span data-ttu-id="55756-115">actionState</span><span class="sxs-lookup"><span data-stu-id="55756-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="55756-116">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="55756-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="55756-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="55756-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="55756-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="55756-118">startDateTime</span></span>|<span data-ttu-id="55756-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55756-119">DateTimeOffset</span></span>|<span data-ttu-id="55756-120">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="55756-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="55756-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="55756-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="55756-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55756-122">DateTimeOffset</span></span>|<span data-ttu-id="55756-123">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="55756-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="55756-124">scanType</span><span class="sxs-lookup"><span data-stu-id="55756-124">scanType</span></span>|<span data-ttu-id="55756-125">String</span><span class="sxs-lookup"><span data-stu-id="55756-125">String</span></span>|<span data-ttu-id="55756-126">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="55756-126">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="55756-127">Связи</span><span class="sxs-lookup"><span data-stu-id="55756-127">Relationships</span></span>
<span data-ttu-id="55756-128">Нет</span><span class="sxs-lookup"><span data-stu-id="55756-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55756-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55756-129">JSON Representation</span></span>
<span data-ttu-id="55756-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55756-130">Here is a JSON representation of the resource.</span></span>
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




