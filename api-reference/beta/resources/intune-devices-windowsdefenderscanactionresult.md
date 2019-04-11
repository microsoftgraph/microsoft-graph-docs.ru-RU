---
title: Тип ресурса windowsDefenderScanActionResult
description: Результат последнего сканирования, выполненного Защитником Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b54feb06e18e0ea772ab69e2ed3bd138564cfc08
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789012"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="760a5-103">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="760a5-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="760a5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="760a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="760a5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="760a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="760a5-106">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="760a5-106">Windows Defender last scan result</span></span>


<span data-ttu-id="760a5-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="760a5-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="760a5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="760a5-108">Properties</span></span>
|<span data-ttu-id="760a5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="760a5-109">Property</span></span>|<span data-ttu-id="760a5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="760a5-110">Type</span></span>|<span data-ttu-id="760a5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="760a5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="760a5-112">actionName</span><span class="sxs-lookup"><span data-stu-id="760a5-112">actionName</span></span>|<span data-ttu-id="760a5-113">String</span><span class="sxs-lookup"><span data-stu-id="760a5-113">String</span></span>|<span data-ttu-id="760a5-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="760a5-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="760a5-115">actionState</span><span class="sxs-lookup"><span data-stu-id="760a5-115">actionState</span></span>|[<span data-ttu-id="760a5-116">actionState</span><span class="sxs-lookup"><span data-stu-id="760a5-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="760a5-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="760a5-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="760a5-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="760a5-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="760a5-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="760a5-119">startDateTime</span></span>|<span data-ttu-id="760a5-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="760a5-120">DateTimeOffset</span></span>|<span data-ttu-id="760a5-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="760a5-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="760a5-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="760a5-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="760a5-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="760a5-123">DateTimeOffset</span></span>|<span data-ttu-id="760a5-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="760a5-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="760a5-125">scanType</span><span class="sxs-lookup"><span data-stu-id="760a5-125">scanType</span></span>|<span data-ttu-id="760a5-126">String</span><span class="sxs-lookup"><span data-stu-id="760a5-126">String</span></span>|<span data-ttu-id="760a5-127">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="760a5-127">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="760a5-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="760a5-128">Relationships</span></span>
<span data-ttu-id="760a5-129">Нет</span><span class="sxs-lookup"><span data-stu-id="760a5-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="760a5-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="760a5-130">JSON Representation</span></span>
<span data-ttu-id="760a5-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="760a5-131">Here is a JSON representation of the resource.</span></span>
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





