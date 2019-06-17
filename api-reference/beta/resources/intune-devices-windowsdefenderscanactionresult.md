---
title: Тип ресурса windowsDefenderScanActionResult
description: Результат последнего сканирования, выполненного Защитником Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f28e33c5edae2efe22368cd827d7e41fa2c51a51
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994288"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="bfaa9-103">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="bfaa9-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="bfaa9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfaa9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bfaa9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bfaa9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfaa9-106">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="bfaa9-106">Windows Defender last scan result</span></span>


<span data-ttu-id="bfaa9-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="bfaa9-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bfaa9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bfaa9-108">Properties</span></span>
|<span data-ttu-id="bfaa9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfaa9-109">Property</span></span>|<span data-ttu-id="bfaa9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bfaa9-110">Type</span></span>|<span data-ttu-id="bfaa9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bfaa9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfaa9-112">actionName</span><span class="sxs-lookup"><span data-stu-id="bfaa9-112">actionName</span></span>|<span data-ttu-id="bfaa9-113">String</span><span class="sxs-lookup"><span data-stu-id="bfaa9-113">String</span></span>|<span data-ttu-id="bfaa9-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="bfaa9-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bfaa9-115">actionState</span><span class="sxs-lookup"><span data-stu-id="bfaa9-115">actionState</span></span>|[<span data-ttu-id="bfaa9-116">actionState</span><span class="sxs-lookup"><span data-stu-id="bfaa9-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="bfaa9-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="bfaa9-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="bfaa9-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="bfaa9-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="bfaa9-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bfaa9-119">startDateTime</span></span>|<span data-ttu-id="bfaa9-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfaa9-120">DateTimeOffset</span></span>|<span data-ttu-id="bfaa9-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="bfaa9-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bfaa9-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="bfaa9-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="bfaa9-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfaa9-123">DateTimeOffset</span></span>|<span data-ttu-id="bfaa9-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="bfaa9-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="bfaa9-125">scanType</span><span class="sxs-lookup"><span data-stu-id="bfaa9-125">scanType</span></span>|<span data-ttu-id="bfaa9-126">String</span><span class="sxs-lookup"><span data-stu-id="bfaa9-126">String</span></span>|<span data-ttu-id="bfaa9-127">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="bfaa9-127">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfaa9-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="bfaa9-128">Relationships</span></span>
<span data-ttu-id="bfaa9-129">Нет</span><span class="sxs-lookup"><span data-stu-id="bfaa9-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bfaa9-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bfaa9-130">JSON Representation</span></span>
<span data-ttu-id="bfaa9-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bfaa9-131">Here is a JSON representation of the resource.</span></span>
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





