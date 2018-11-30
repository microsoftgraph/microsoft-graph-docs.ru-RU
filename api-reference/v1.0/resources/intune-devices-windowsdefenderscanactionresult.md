---
title: Тип ресурса windowsDefenderScanActionResult
description: Результат последнего сканирования, выполненного Защитником Windows
ms.openlocfilehash: 6221e0d746e677f09b2be00ec66a898e6dfc288c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024785"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="3b272-103">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="3b272-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="3b272-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3b272-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b272-105">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="3b272-105">Windows Defender last scan result</span></span>

<span data-ttu-id="3b272-106">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3b272-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3b272-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b272-107">Properties</span></span>
|<span data-ttu-id="3b272-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b272-108">Property</span></span>|<span data-ttu-id="3b272-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3b272-109">Type</span></span>|<span data-ttu-id="3b272-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3b272-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b272-111">actionName</span><span class="sxs-lookup"><span data-stu-id="3b272-111">actionName</span></span>|<span data-ttu-id="3b272-112">String</span><span class="sxs-lookup"><span data-stu-id="3b272-112">String</span></span>|<span data-ttu-id="3b272-113">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3b272-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3b272-114">actionState</span><span class="sxs-lookup"><span data-stu-id="3b272-114">actionState</span></span>|[<span data-ttu-id="3b272-115">actionState</span><span class="sxs-lookup"><span data-stu-id="3b272-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="3b272-116">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="3b272-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="3b272-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="3b272-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="3b272-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3b272-118">startDateTime</span></span>|<span data-ttu-id="3b272-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b272-119">DateTimeOffset</span></span>|<span data-ttu-id="3b272-120">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3b272-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3b272-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b272-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="3b272-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b272-122">DateTimeOffset</span></span>|<span data-ttu-id="3b272-123">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="3b272-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="3b272-124">scanType</span><span class="sxs-lookup"><span data-stu-id="3b272-124">scanType</span></span>|<span data-ttu-id="3b272-125">String</span><span class="sxs-lookup"><span data-stu-id="3b272-125">String</span></span>|<span data-ttu-id="3b272-126">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="3b272-126">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b272-127">Связи</span><span class="sxs-lookup"><span data-stu-id="3b272-127">Relationships</span></span>
<span data-ttu-id="3b272-128">Нет</span><span class="sxs-lookup"><span data-stu-id="3b272-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3b272-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b272-129">JSON Representation</span></span>
<span data-ttu-id="3b272-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b272-130">Here is a JSON representation of the resource.</span></span>
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



