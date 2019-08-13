---
title: Тип ресурса windowsDefenderScanActionResult
description: Результат последнего сканирования, выполненного Защитником Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 24cb44c634706b51baef2e840dc17e5622972233
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366506"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="24900-103">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="24900-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="24900-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24900-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24900-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24900-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24900-106">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="24900-106">Windows Defender last scan result</span></span>


<span data-ttu-id="24900-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="24900-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="24900-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="24900-108">Properties</span></span>
|<span data-ttu-id="24900-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="24900-109">Property</span></span>|<span data-ttu-id="24900-110">Тип</span><span class="sxs-lookup"><span data-stu-id="24900-110">Type</span></span>|<span data-ttu-id="24900-111">Описание</span><span class="sxs-lookup"><span data-stu-id="24900-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24900-112">actionName</span><span class="sxs-lookup"><span data-stu-id="24900-112">actionName</span></span>|<span data-ttu-id="24900-113">String</span><span class="sxs-lookup"><span data-stu-id="24900-113">String</span></span>|<span data-ttu-id="24900-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="24900-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="24900-115">actionState</span><span class="sxs-lookup"><span data-stu-id="24900-115">actionState</span></span>|[<span data-ttu-id="24900-116">actionState</span><span class="sxs-lookup"><span data-stu-id="24900-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="24900-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="24900-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="24900-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="24900-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="24900-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="24900-119">startDateTime</span></span>|<span data-ttu-id="24900-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24900-120">DateTimeOffset</span></span>|<span data-ttu-id="24900-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="24900-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="24900-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="24900-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="24900-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24900-123">DateTimeOffset</span></span>|<span data-ttu-id="24900-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="24900-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="24900-125">scanType</span><span class="sxs-lookup"><span data-stu-id="24900-125">scanType</span></span>|<span data-ttu-id="24900-126">String</span><span class="sxs-lookup"><span data-stu-id="24900-126">String</span></span>|<span data-ttu-id="24900-127">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="24900-127">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="24900-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="24900-128">Relationships</span></span>
<span data-ttu-id="24900-129">Нет</span><span class="sxs-lookup"><span data-stu-id="24900-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24900-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24900-130">JSON Representation</span></span>
<span data-ttu-id="24900-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24900-131">Here is a JSON representation of the resource.</span></span>
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



