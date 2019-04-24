---
title: Тип ресурса locateDeviceActionResult
description: Результат действия "Поиск устройства"
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f38422c419d4f50901cbc015b82ca51c470ddfe4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522204"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="98636-103">Тип ресурса locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="98636-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="98636-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98636-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98636-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98636-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98636-106">Результат действия "Поиск устройства"</span><span class="sxs-lookup"><span data-stu-id="98636-106">Locate device action result</span></span>


<span data-ttu-id="98636-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="98636-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="98636-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="98636-108">Properties</span></span>
|<span data-ttu-id="98636-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="98636-109">Property</span></span>|<span data-ttu-id="98636-110">Тип</span><span class="sxs-lookup"><span data-stu-id="98636-110">Type</span></span>|<span data-ttu-id="98636-111">Описание</span><span class="sxs-lookup"><span data-stu-id="98636-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98636-112">actionName</span><span class="sxs-lookup"><span data-stu-id="98636-112">actionName</span></span>|<span data-ttu-id="98636-113">String</span><span class="sxs-lookup"><span data-stu-id="98636-113">String</span></span>|<span data-ttu-id="98636-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="98636-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="98636-115">actionState</span><span class="sxs-lookup"><span data-stu-id="98636-115">actionState</span></span>|[<span data-ttu-id="98636-116">actionState</span><span class="sxs-lookup"><span data-stu-id="98636-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="98636-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="98636-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="98636-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="98636-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="98636-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="98636-119">startDateTime</span></span>|<span data-ttu-id="98636-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98636-120">DateTimeOffset</span></span>|<span data-ttu-id="98636-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="98636-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="98636-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="98636-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="98636-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98636-123">DateTimeOffset</span></span>|<span data-ttu-id="98636-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="98636-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="98636-125">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="98636-125">deviceLocation</span></span>|[<span data-ttu-id="98636-126">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="98636-126">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="98636-127">Местоположение устройства</span><span class="sxs-lookup"><span data-stu-id="98636-127">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="98636-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="98636-128">Relationships</span></span>
<span data-ttu-id="98636-129">Нет</span><span class="sxs-lookup"><span data-stu-id="98636-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98636-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98636-130">JSON Representation</span></span>
<span data-ttu-id="98636-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98636-131">Here is a JSON representation of the resource.</span></span>
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





