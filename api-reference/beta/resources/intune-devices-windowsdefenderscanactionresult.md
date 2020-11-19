---
title: Тип ресурса windowsDefenderScanActionResult
description: Результат последнего сканирования, выполненного Защитником Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2774052035c99dc2616532d5a3997fb5f4e05906
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49208172"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="24b41-103">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="24b41-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="24b41-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24b41-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24b41-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24b41-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24b41-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24b41-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24b41-107">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="24b41-107">Windows Defender last scan result</span></span>


<span data-ttu-id="24b41-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="24b41-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="24b41-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="24b41-109">Properties</span></span>
|<span data-ttu-id="24b41-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="24b41-110">Property</span></span>|<span data-ttu-id="24b41-111">Тип</span><span class="sxs-lookup"><span data-stu-id="24b41-111">Type</span></span>|<span data-ttu-id="24b41-112">Описание</span><span class="sxs-lookup"><span data-stu-id="24b41-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24b41-113">actionName</span><span class="sxs-lookup"><span data-stu-id="24b41-113">actionName</span></span>|<span data-ttu-id="24b41-114">String</span><span class="sxs-lookup"><span data-stu-id="24b41-114">String</span></span>|<span data-ttu-id="24b41-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="24b41-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="24b41-116">actionState</span><span class="sxs-lookup"><span data-stu-id="24b41-116">actionState</span></span>|[<span data-ttu-id="24b41-117">actionState</span><span class="sxs-lookup"><span data-stu-id="24b41-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="24b41-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="24b41-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="24b41-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="24b41-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="24b41-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="24b41-120">startDateTime</span></span>|<span data-ttu-id="24b41-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24b41-121">DateTimeOffset</span></span>|<span data-ttu-id="24b41-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="24b41-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="24b41-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="24b41-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="24b41-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24b41-124">DateTimeOffset</span></span>|<span data-ttu-id="24b41-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="24b41-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="24b41-126">scanType</span><span class="sxs-lookup"><span data-stu-id="24b41-126">scanType</span></span>|<span data-ttu-id="24b41-127">String</span><span class="sxs-lookup"><span data-stu-id="24b41-127">String</span></span>|<span data-ttu-id="24b41-128">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="24b41-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="24b41-129">Связи</span><span class="sxs-lookup"><span data-stu-id="24b41-129">Relationships</span></span>
<span data-ttu-id="24b41-130">Нет</span><span class="sxs-lookup"><span data-stu-id="24b41-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24b41-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24b41-131">JSON Representation</span></span>
<span data-ttu-id="24b41-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24b41-132">Here is a JSON representation of the resource.</span></span>
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




