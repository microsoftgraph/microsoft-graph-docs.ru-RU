---
title: Тип ресурса windowsDefenderScanActionResult
description: Результат последнего сканирования, выполненного Защитником Windows
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 14ed1b41445625b6c460a1438df2b48e17c5e48a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43401828"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="5c822-103">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="5c822-103">windowsDefenderScanActionResult resource type</span></span>

<span data-ttu-id="5c822-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c822-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c822-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c822-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c822-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c822-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c822-107">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="5c822-107">Windows Defender last scan result</span></span>


<span data-ttu-id="5c822-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5c822-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5c822-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c822-109">Properties</span></span>
|<span data-ttu-id="5c822-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c822-110">Property</span></span>|<span data-ttu-id="5c822-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5c822-111">Type</span></span>|<span data-ttu-id="5c822-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5c822-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c822-113">actionName</span><span class="sxs-lookup"><span data-stu-id="5c822-113">actionName</span></span>|<span data-ttu-id="5c822-114">String</span><span class="sxs-lookup"><span data-stu-id="5c822-114">String</span></span>|<span data-ttu-id="5c822-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="5c822-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5c822-116">actionState</span><span class="sxs-lookup"><span data-stu-id="5c822-116">actionState</span></span>|[<span data-ttu-id="5c822-117">actionState</span><span class="sxs-lookup"><span data-stu-id="5c822-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="5c822-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="5c822-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="5c822-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="5c822-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="5c822-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5c822-120">startDateTime</span></span>|<span data-ttu-id="5c822-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c822-121">DateTimeOffset</span></span>|<span data-ttu-id="5c822-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="5c822-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5c822-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c822-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="5c822-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c822-124">DateTimeOffset</span></span>|<span data-ttu-id="5c822-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="5c822-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5c822-126">scanType</span><span class="sxs-lookup"><span data-stu-id="5c822-126">scanType</span></span>|<span data-ttu-id="5c822-127">String</span><span class="sxs-lookup"><span data-stu-id="5c822-127">String</span></span>|<span data-ttu-id="5c822-128">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="5c822-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c822-129">Связи</span><span class="sxs-lookup"><span data-stu-id="5c822-129">Relationships</span></span>
<span data-ttu-id="5c822-130">Нет</span><span class="sxs-lookup"><span data-stu-id="5c822-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c822-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5c822-131">JSON Representation</span></span>
<span data-ttu-id="5c822-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c822-132">Here is a JSON representation of the resource.</span></span>
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



