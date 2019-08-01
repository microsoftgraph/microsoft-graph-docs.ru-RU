---
title: Тип ресурса windowsDefenderScanActionResult
description: Результат последнего сканирования, выполненного Защитником Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0e9bcf4d45a184ea54a15bedc85efc6fc9bb4073
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027407"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="7a00b-103">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="7a00b-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="7a00b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a00b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a00b-105">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="7a00b-105">Windows Defender last scan result</span></span>


<span data-ttu-id="7a00b-106">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7a00b-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7a00b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a00b-107">Properties</span></span>
|<span data-ttu-id="7a00b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a00b-108">Property</span></span>|<span data-ttu-id="7a00b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7a00b-109">Type</span></span>|<span data-ttu-id="7a00b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7a00b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a00b-111">actionName</span><span class="sxs-lookup"><span data-stu-id="7a00b-111">actionName</span></span>|<span data-ttu-id="7a00b-112">String</span><span class="sxs-lookup"><span data-stu-id="7a00b-112">String</span></span>|<span data-ttu-id="7a00b-113">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="7a00b-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7a00b-114">actionState</span><span class="sxs-lookup"><span data-stu-id="7a00b-114">actionState</span></span>|[<span data-ttu-id="7a00b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="7a00b-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="7a00b-116">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="7a00b-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="7a00b-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="7a00b-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="7a00b-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7a00b-118">startDateTime</span></span>|<span data-ttu-id="7a00b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a00b-119">DateTimeOffset</span></span>|<span data-ttu-id="7a00b-120">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="7a00b-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7a00b-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a00b-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="7a00b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a00b-122">DateTimeOffset</span></span>|<span data-ttu-id="7a00b-123">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="7a00b-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7a00b-124">scanType</span><span class="sxs-lookup"><span data-stu-id="7a00b-124">scanType</span></span>|<span data-ttu-id="7a00b-125">String</span><span class="sxs-lookup"><span data-stu-id="7a00b-125">String</span></span>|<span data-ttu-id="7a00b-126">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="7a00b-126">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a00b-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="7a00b-127">Relationships</span></span>
<span data-ttu-id="7a00b-128">Нет</span><span class="sxs-lookup"><span data-stu-id="7a00b-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a00b-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a00b-129">JSON Representation</span></span>
<span data-ttu-id="7a00b-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a00b-130">Here is a JSON representation of the resource.</span></span>
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



