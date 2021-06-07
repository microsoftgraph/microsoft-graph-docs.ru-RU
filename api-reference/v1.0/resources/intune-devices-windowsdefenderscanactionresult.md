---
title: Тип ресурса windowsDefenderScanActionResult
description: Результат последнего сканирования, выполненного Защитником Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 857494e6c4e08fe2f659bf26ae63a0be19c17c3e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755009"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="33e8c-103">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="33e8c-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="33e8c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33e8c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33e8c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33e8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33e8c-106">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="33e8c-106">Windows Defender last scan result</span></span>


<span data-ttu-id="33e8c-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="33e8c-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="33e8c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="33e8c-108">Properties</span></span>
|<span data-ttu-id="33e8c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="33e8c-109">Property</span></span>|<span data-ttu-id="33e8c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="33e8c-110">Type</span></span>|<span data-ttu-id="33e8c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="33e8c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33e8c-112">actionName</span><span class="sxs-lookup"><span data-stu-id="33e8c-112">actionName</span></span>|<span data-ttu-id="33e8c-113">String</span><span class="sxs-lookup"><span data-stu-id="33e8c-113">String</span></span>|<span data-ttu-id="33e8c-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="33e8c-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="33e8c-115">actionState</span><span class="sxs-lookup"><span data-stu-id="33e8c-115">actionState</span></span>|[<span data-ttu-id="33e8c-116">actionState</span><span class="sxs-lookup"><span data-stu-id="33e8c-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="33e8c-117">Состояние действия, унаследованной от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="33e8c-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="33e8c-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="33e8c-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="33e8c-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="33e8c-119">startDateTime</span></span>|<span data-ttu-id="33e8c-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33e8c-120">DateTimeOffset</span></span>|<span data-ttu-id="33e8c-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="33e8c-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="33e8c-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="33e8c-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="33e8c-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33e8c-123">DateTimeOffset</span></span>|<span data-ttu-id="33e8c-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="33e8c-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="33e8c-125">scanType</span><span class="sxs-lookup"><span data-stu-id="33e8c-125">scanType</span></span>|<span data-ttu-id="33e8c-126">String</span><span class="sxs-lookup"><span data-stu-id="33e8c-126">String</span></span>|<span data-ttu-id="33e8c-127">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="33e8c-127">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="33e8c-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="33e8c-128">Relationships</span></span>
<span data-ttu-id="33e8c-129">Нет</span><span class="sxs-lookup"><span data-stu-id="33e8c-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="33e8c-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="33e8c-130">JSON Representation</span></span>
<span data-ttu-id="33e8c-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33e8c-131">Here is a JSON representation of the resource.</span></span>
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




