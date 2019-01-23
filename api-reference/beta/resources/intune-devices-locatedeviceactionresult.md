---
title: Тип ресурса locateDeviceActionResult
description: Результат действия "Поиск устройства"
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 682b2267369a80b3d2cb37d17dd1b2aafdef1f63
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416890"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="112c2-103">Тип ресурса locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="112c2-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="112c2-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="112c2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="112c2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="112c2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="112c2-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="112c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="112c2-107">Результат действия "Поиск устройства"</span><span class="sxs-lookup"><span data-stu-id="112c2-107">Locate device action result</span></span>


<span data-ttu-id="112c2-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="112c2-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="112c2-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="112c2-109">Properties</span></span>
|<span data-ttu-id="112c2-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="112c2-110">Property</span></span>|<span data-ttu-id="112c2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="112c2-111">Type</span></span>|<span data-ttu-id="112c2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="112c2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="112c2-113">actionName</span><span class="sxs-lookup"><span data-stu-id="112c2-113">actionName</span></span>|<span data-ttu-id="112c2-114">String</span><span class="sxs-lookup"><span data-stu-id="112c2-114">String</span></span>|<span data-ttu-id="112c2-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="112c2-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="112c2-116">actionState</span><span class="sxs-lookup"><span data-stu-id="112c2-116">actionState</span></span>|[<span data-ttu-id="112c2-117">actionState</span><span class="sxs-lookup"><span data-stu-id="112c2-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="112c2-118">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="112c2-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="112c2-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="112c2-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="112c2-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="112c2-120">startDateTime</span></span>|<span data-ttu-id="112c2-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="112c2-121">DateTimeOffset</span></span>|<span data-ttu-id="112c2-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="112c2-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="112c2-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="112c2-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="112c2-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="112c2-124">DateTimeOffset</span></span>|<span data-ttu-id="112c2-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="112c2-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="112c2-126">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="112c2-126">deviceLocation</span></span>|[<span data-ttu-id="112c2-127">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="112c2-127">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="112c2-128">Местоположение устройства</span><span class="sxs-lookup"><span data-stu-id="112c2-128">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="112c2-129">Связи</span><span class="sxs-lookup"><span data-stu-id="112c2-129">Relationships</span></span>
<span data-ttu-id="112c2-130">Нет</span><span class="sxs-lookup"><span data-stu-id="112c2-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="112c2-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="112c2-131">JSON Representation</span></span>
<span data-ttu-id="112c2-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="112c2-132">Here is a JSON representation of the resource.</span></span>
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
    "lastCollectedDateTimeUtc": "String (timestamp)",
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




