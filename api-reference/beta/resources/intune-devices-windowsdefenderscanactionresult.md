---
title: Тип ресурса windowsDefenderScanActionResult
description: Результат последнего сканирования, выполненного Защитником Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1e26904504d882af0ed253b547709a29e075954c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528437"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="c19f5-103">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="c19f5-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="c19f5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c19f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c19f5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c19f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c19f5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c19f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c19f5-107">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="c19f5-107">Windows Defender last scan result</span></span>


<span data-ttu-id="c19f5-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c19f5-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c19f5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c19f5-109">Properties</span></span>
|<span data-ttu-id="c19f5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c19f5-110">Property</span></span>|<span data-ttu-id="c19f5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c19f5-111">Type</span></span>|<span data-ttu-id="c19f5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c19f5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c19f5-113">actionName</span><span class="sxs-lookup"><span data-stu-id="c19f5-113">actionName</span></span>|<span data-ttu-id="c19f5-114">String</span><span class="sxs-lookup"><span data-stu-id="c19f5-114">String</span></span>|<span data-ttu-id="c19f5-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c19f5-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c19f5-116">actionState</span><span class="sxs-lookup"><span data-stu-id="c19f5-116">actionState</span></span>|[<span data-ttu-id="c19f5-117">actionState</span><span class="sxs-lookup"><span data-stu-id="c19f5-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="c19f5-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c19f5-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="c19f5-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="c19f5-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c19f5-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c19f5-120">startDateTime</span></span>|<span data-ttu-id="c19f5-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c19f5-121">DateTimeOffset</span></span>|<span data-ttu-id="c19f5-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c19f5-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c19f5-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c19f5-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="c19f5-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c19f5-124">DateTimeOffset</span></span>|<span data-ttu-id="c19f5-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c19f5-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c19f5-126">scanType</span><span class="sxs-lookup"><span data-stu-id="c19f5-126">scanType</span></span>|<span data-ttu-id="c19f5-127">String</span><span class="sxs-lookup"><span data-stu-id="c19f5-127">String</span></span>|<span data-ttu-id="c19f5-128">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="c19f5-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="c19f5-129">Связи</span><span class="sxs-lookup"><span data-stu-id="c19f5-129">Relationships</span></span>
<span data-ttu-id="c19f5-130">Нет</span><span class="sxs-lookup"><span data-stu-id="c19f5-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c19f5-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c19f5-131">JSON Representation</span></span>
<span data-ttu-id="c19f5-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c19f5-132">Here is a JSON representation of the resource.</span></span>
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



