---
title: Тип ресурса windowsDefenderScanActionResult
description: Результат последнего сканирования, выполненного Защитником Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20d30ebda6e24f26406d189ebd980e558bf74e83
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523352"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="1dff0-103">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="1dff0-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="1dff0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1dff0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dff0-105">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="1dff0-105">Windows Defender last scan result</span></span>


<span data-ttu-id="1dff0-106">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1dff0-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1dff0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1dff0-107">Properties</span></span>
|<span data-ttu-id="1dff0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1dff0-108">Property</span></span>|<span data-ttu-id="1dff0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1dff0-109">Type</span></span>|<span data-ttu-id="1dff0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1dff0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dff0-111">actionName</span><span class="sxs-lookup"><span data-stu-id="1dff0-111">actionName</span></span>|<span data-ttu-id="1dff0-112">String</span><span class="sxs-lookup"><span data-stu-id="1dff0-112">String</span></span>|<span data-ttu-id="1dff0-113">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="1dff0-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1dff0-114">actionState</span><span class="sxs-lookup"><span data-stu-id="1dff0-114">actionState</span></span>|[<span data-ttu-id="1dff0-115">actionState</span><span class="sxs-lookup"><span data-stu-id="1dff0-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="1dff0-116">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="1dff0-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="1dff0-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="1dff0-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1dff0-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1dff0-118">startDateTime</span></span>|<span data-ttu-id="1dff0-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dff0-119">DateTimeOffset</span></span>|<span data-ttu-id="1dff0-120">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="1dff0-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1dff0-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1dff0-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="1dff0-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dff0-122">DateTimeOffset</span></span>|<span data-ttu-id="1dff0-123">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="1dff0-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1dff0-124">scanType</span><span class="sxs-lookup"><span data-stu-id="1dff0-124">scanType</span></span>|<span data-ttu-id="1dff0-125">String</span><span class="sxs-lookup"><span data-stu-id="1dff0-125">String</span></span>|<span data-ttu-id="1dff0-126">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="1dff0-126">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="1dff0-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="1dff0-127">Relationships</span></span>
<span data-ttu-id="1dff0-128">Нет</span><span class="sxs-lookup"><span data-stu-id="1dff0-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1dff0-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1dff0-129">JSON Representation</span></span>
<span data-ttu-id="1dff0-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1dff0-130">Here is a JSON representation of the resource.</span></span>
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



