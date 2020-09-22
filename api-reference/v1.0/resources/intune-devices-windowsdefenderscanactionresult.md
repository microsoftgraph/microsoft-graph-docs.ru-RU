---
title: Тип ресурса windowsDefenderScanActionResult
description: Результат последнего сканирования, выполненного Защитником Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7f6de49d6a87a2f385b4d6c29f3442286c63beb7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091014"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="f361f-103">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="f361f-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="f361f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f361f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f361f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f361f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f361f-106">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="f361f-106">Windows Defender last scan result</span></span>


<span data-ttu-id="f361f-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f361f-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f361f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f361f-108">Properties</span></span>
|<span data-ttu-id="f361f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f361f-109">Property</span></span>|<span data-ttu-id="f361f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f361f-110">Type</span></span>|<span data-ttu-id="f361f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f361f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f361f-112">actionName</span><span class="sxs-lookup"><span data-stu-id="f361f-112">actionName</span></span>|<span data-ttu-id="f361f-113">String</span><span class="sxs-lookup"><span data-stu-id="f361f-113">String</span></span>|<span data-ttu-id="f361f-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="f361f-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f361f-115">actionState</span><span class="sxs-lookup"><span data-stu-id="f361f-115">actionState</span></span>|[<span data-ttu-id="f361f-116">actionState</span><span class="sxs-lookup"><span data-stu-id="f361f-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="f361f-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="f361f-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="f361f-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="f361f-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="f361f-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f361f-119">startDateTime</span></span>|<span data-ttu-id="f361f-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f361f-120">DateTimeOffset</span></span>|<span data-ttu-id="f361f-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="f361f-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f361f-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f361f-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="f361f-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f361f-123">DateTimeOffset</span></span>|<span data-ttu-id="f361f-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="f361f-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f361f-125">scanType</span><span class="sxs-lookup"><span data-stu-id="f361f-125">scanType</span></span>|<span data-ttu-id="f361f-126">String</span><span class="sxs-lookup"><span data-stu-id="f361f-126">String</span></span>|<span data-ttu-id="f361f-127">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="f361f-127">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="f361f-128">Связи</span><span class="sxs-lookup"><span data-stu-id="f361f-128">Relationships</span></span>
<span data-ttu-id="f361f-129">Нет</span><span class="sxs-lookup"><span data-stu-id="f361f-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f361f-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f361f-130">JSON Representation</span></span>
<span data-ttu-id="f361f-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f361f-131">Here is a JSON representation of the resource.</span></span>
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









