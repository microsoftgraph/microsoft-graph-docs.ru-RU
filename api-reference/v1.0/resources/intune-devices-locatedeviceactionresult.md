---
title: Тип ресурса locateDeviceActionResult
description: Результат действия "Поиск устройства"
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c335ac49bcf053e58381f7c1111caf5ae70cb0fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570364"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="5f426-103">Тип ресурса locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="5f426-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="5f426-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f426-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f426-105">Результат действия "Поиск устройства"</span><span class="sxs-lookup"><span data-stu-id="5f426-105">Locate device action result</span></span>


<span data-ttu-id="5f426-106">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5f426-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5f426-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f426-107">Properties</span></span>
|<span data-ttu-id="5f426-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f426-108">Property</span></span>|<span data-ttu-id="5f426-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5f426-109">Type</span></span>|<span data-ttu-id="5f426-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5f426-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f426-111">actionName</span><span class="sxs-lookup"><span data-stu-id="5f426-111">actionName</span></span>|<span data-ttu-id="5f426-112">String</span><span class="sxs-lookup"><span data-stu-id="5f426-112">String</span></span>|<span data-ttu-id="5f426-113">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="5f426-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5f426-114">actionState</span><span class="sxs-lookup"><span data-stu-id="5f426-114">actionState</span></span>|[<span data-ttu-id="5f426-115">actionState</span><span class="sxs-lookup"><span data-stu-id="5f426-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="5f426-116">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="5f426-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="5f426-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="5f426-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="5f426-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5f426-118">startDateTime</span></span>|<span data-ttu-id="5f426-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f426-119">DateTimeOffset</span></span>|<span data-ttu-id="5f426-120">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="5f426-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5f426-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f426-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="5f426-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f426-122">DateTimeOffset</span></span>|<span data-ttu-id="5f426-123">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5f426-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5f426-124">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="5f426-124">deviceLocation</span></span>|[<span data-ttu-id="5f426-125">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="5f426-125">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="5f426-126">Местоположение устройства</span><span class="sxs-lookup"><span data-stu-id="5f426-126">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f426-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="5f426-127">Relationships</span></span>
<span data-ttu-id="5f426-128">Нет</span><span class="sxs-lookup"><span data-stu-id="5f426-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f426-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f426-129">JSON Representation</span></span>
<span data-ttu-id="5f426-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f426-130">Here is a JSON representation of the resource.</span></span>
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



