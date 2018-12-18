---
title: Тип ресурса windowsDefenderScanActionResult
description: Результат последнего сканирования, выполненного Защитником Windows
author: tfitzmac
ms.openlocfilehash: fa988a971925cf61db0ab9f7e962162565e8a4b3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323039"
---
# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="6a6de-103">Тип ресурса windowsDefenderScanActionResult</span><span class="sxs-lookup"><span data-stu-id="6a6de-103">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="6a6de-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6a6de-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a6de-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a6de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a6de-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6a6de-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a6de-107">Результат последнего сканирования, выполненного Защитником Windows</span><span class="sxs-lookup"><span data-stu-id="6a6de-107">Windows Defender last scan result</span></span>

<span data-ttu-id="6a6de-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6a6de-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6a6de-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a6de-109">Properties</span></span>
|<span data-ttu-id="6a6de-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a6de-110">Property</span></span>|<span data-ttu-id="6a6de-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6a6de-111">Type</span></span>|<span data-ttu-id="6a6de-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6a6de-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a6de-113">actionName</span><span class="sxs-lookup"><span data-stu-id="6a6de-113">actionName</span></span>|<span data-ttu-id="6a6de-114">String</span><span class="sxs-lookup"><span data-stu-id="6a6de-114">String</span></span>|<span data-ttu-id="6a6de-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6a6de-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6a6de-116">actionState</span><span class="sxs-lookup"><span data-stu-id="6a6de-116">actionState</span></span>|[<span data-ttu-id="6a6de-117">actionState</span><span class="sxs-lookup"><span data-stu-id="6a6de-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="6a6de-118">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="6a6de-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="6a6de-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="6a6de-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="6a6de-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6a6de-120">startDateTime</span></span>|<span data-ttu-id="6a6de-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a6de-121">DateTimeOffset</span></span>|<span data-ttu-id="6a6de-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6a6de-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6a6de-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a6de-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="6a6de-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a6de-124">DateTimeOffset</span></span>|<span data-ttu-id="6a6de-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="6a6de-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6a6de-126">scanType</span><span class="sxs-lookup"><span data-stu-id="6a6de-126">scanType</span></span>|<span data-ttu-id="6a6de-127">String</span><span class="sxs-lookup"><span data-stu-id="6a6de-127">String</span></span>|<span data-ttu-id="6a6de-128">Тип сканирования (полное или краткое).</span><span class="sxs-lookup"><span data-stu-id="6a6de-128">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a6de-129">Связи</span><span class="sxs-lookup"><span data-stu-id="6a6de-129">Relationships</span></span>
<span data-ttu-id="6a6de-130">Нет</span><span class="sxs-lookup"><span data-stu-id="6a6de-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6a6de-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a6de-131">JSON Representation</span></span>
<span data-ttu-id="6a6de-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a6de-132">Here is a JSON representation of the resource.</span></span>
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





