---
title: Тип ресурса locateDeviceActionResult
description: Результат действия "Поиск устройства"
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 246fcae2a9a51822f97d7f193ff6056bee55db26
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923497"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="584f3-103">Тип ресурса locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="584f3-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="584f3-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="584f3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="584f3-105">Результат действия "Поиск устройства"</span><span class="sxs-lookup"><span data-stu-id="584f3-105">Locate device action result</span></span>

<span data-ttu-id="584f3-106">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="584f3-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="584f3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="584f3-107">Properties</span></span>
|<span data-ttu-id="584f3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="584f3-108">Property</span></span>|<span data-ttu-id="584f3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="584f3-109">Type</span></span>|<span data-ttu-id="584f3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="584f3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="584f3-111">actionName</span><span class="sxs-lookup"><span data-stu-id="584f3-111">actionName</span></span>|<span data-ttu-id="584f3-112">String</span><span class="sxs-lookup"><span data-stu-id="584f3-112">String</span></span>|<span data-ttu-id="584f3-113">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="584f3-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="584f3-114">actionState</span><span class="sxs-lookup"><span data-stu-id="584f3-114">actionState</span></span>|[<span data-ttu-id="584f3-115">actionState</span><span class="sxs-lookup"><span data-stu-id="584f3-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="584f3-116">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="584f3-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="584f3-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="584f3-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="584f3-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="584f3-118">startDateTime</span></span>|<span data-ttu-id="584f3-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="584f3-119">DateTimeOffset</span></span>|<span data-ttu-id="584f3-120">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="584f3-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="584f3-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="584f3-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="584f3-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="584f3-122">DateTimeOffset</span></span>|<span data-ttu-id="584f3-123">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="584f3-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="584f3-124">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="584f3-124">deviceLocation</span></span>|[<span data-ttu-id="584f3-125">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="584f3-125">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="584f3-126">Местоположение устройства</span><span class="sxs-lookup"><span data-stu-id="584f3-126">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="584f3-127">Связи</span><span class="sxs-lookup"><span data-stu-id="584f3-127">Relationships</span></span>
<span data-ttu-id="584f3-128">Нет</span><span class="sxs-lookup"><span data-stu-id="584f3-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="584f3-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="584f3-129">JSON Representation</span></span>
<span data-ttu-id="584f3-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="584f3-130">Here is a JSON representation of the resource.</span></span>
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



