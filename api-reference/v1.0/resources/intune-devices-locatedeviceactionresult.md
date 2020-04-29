---
title: Тип ресурса locateDeviceActionResult
description: Результат действия "Поиск устройства"
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f0d1a6dac5c6eb0bd62e3313bb44041d436af86a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472394"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="2f44c-103">Тип ресурса locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="2f44c-103">locateDeviceActionResult resource type</span></span>

<span data-ttu-id="2f44c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f44c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f44c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f44c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f44c-106">Результат действия "Поиск устройства"</span><span class="sxs-lookup"><span data-stu-id="2f44c-106">Locate device action result</span></span>


<span data-ttu-id="2f44c-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2f44c-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2f44c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f44c-108">Properties</span></span>
|<span data-ttu-id="2f44c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f44c-109">Property</span></span>|<span data-ttu-id="2f44c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2f44c-110">Type</span></span>|<span data-ttu-id="2f44c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2f44c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f44c-112">actionName</span><span class="sxs-lookup"><span data-stu-id="2f44c-112">actionName</span></span>|<span data-ttu-id="2f44c-113">String</span><span class="sxs-lookup"><span data-stu-id="2f44c-113">String</span></span>|<span data-ttu-id="2f44c-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="2f44c-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2f44c-115">actionState</span><span class="sxs-lookup"><span data-stu-id="2f44c-115">actionState</span></span>|[<span data-ttu-id="2f44c-116">actionState</span><span class="sxs-lookup"><span data-stu-id="2f44c-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="2f44c-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="2f44c-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="2f44c-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="2f44c-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="2f44c-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2f44c-119">startDateTime</span></span>|<span data-ttu-id="2f44c-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f44c-120">DateTimeOffset</span></span>|<span data-ttu-id="2f44c-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="2f44c-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2f44c-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f44c-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="2f44c-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f44c-123">DateTimeOffset</span></span>|<span data-ttu-id="2f44c-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2f44c-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2f44c-125">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="2f44c-125">deviceLocation</span></span>|[<span data-ttu-id="2f44c-126">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="2f44c-126">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="2f44c-127">Местоположение устройства</span><span class="sxs-lookup"><span data-stu-id="2f44c-127">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f44c-128">Связи</span><span class="sxs-lookup"><span data-stu-id="2f44c-128">Relationships</span></span>
<span data-ttu-id="2f44c-129">Нет</span><span class="sxs-lookup"><span data-stu-id="2f44c-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f44c-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f44c-130">JSON Representation</span></span>
<span data-ttu-id="2f44c-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f44c-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.locateDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locateDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "deviceLocation": {
    "@odata.type": "microsoft.graph.deviceGeoLocation",
    "lastCollectedDateTime": "String (timestamp)",
    "longitude": "<Unknown Primitive Type Edm.Double>",
    "latitude": "<Unknown Primitive Type Edm.Double>",
    "altitude": "<Unknown Primitive Type Edm.Double>",
    "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
    "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
    "heading": "<Unknown Primitive Type Edm.Double>",
    "speed": "<Unknown Primitive Type Edm.Double>"
  }
}
```







