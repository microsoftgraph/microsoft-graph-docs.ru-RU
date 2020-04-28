---
title: Тип ресурса locateDeviceActionResult
description: Результат действия "Поиск устройства"
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c3dad81d0cb919c421c5dcaaa652a2eeaac788bf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470546"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="a9dba-103">Тип ресурса locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="a9dba-103">locateDeviceActionResult resource type</span></span>

<span data-ttu-id="a9dba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9dba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9dba-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9dba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9dba-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a9dba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9dba-107">Результат действия "Поиск устройства"</span><span class="sxs-lookup"><span data-stu-id="a9dba-107">Locate device action result</span></span>


<span data-ttu-id="a9dba-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a9dba-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a9dba-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9dba-109">Properties</span></span>
|<span data-ttu-id="a9dba-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9dba-110">Property</span></span>|<span data-ttu-id="a9dba-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a9dba-111">Type</span></span>|<span data-ttu-id="a9dba-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a9dba-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9dba-113">actionName</span><span class="sxs-lookup"><span data-stu-id="a9dba-113">actionName</span></span>|<span data-ttu-id="a9dba-114">String</span><span class="sxs-lookup"><span data-stu-id="a9dba-114">String</span></span>|<span data-ttu-id="a9dba-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="a9dba-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a9dba-116">actionState</span><span class="sxs-lookup"><span data-stu-id="a9dba-116">actionState</span></span>|[<span data-ttu-id="a9dba-117">actionState</span><span class="sxs-lookup"><span data-stu-id="a9dba-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="a9dba-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="a9dba-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="a9dba-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="a9dba-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="a9dba-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a9dba-120">startDateTime</span></span>|<span data-ttu-id="a9dba-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9dba-121">DateTimeOffset</span></span>|<span data-ttu-id="a9dba-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="a9dba-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a9dba-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9dba-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="a9dba-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9dba-124">DateTimeOffset</span></span>|<span data-ttu-id="a9dba-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a9dba-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a9dba-126">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="a9dba-126">deviceLocation</span></span>|[<span data-ttu-id="a9dba-127">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="a9dba-127">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="a9dba-128">Местоположение устройства</span><span class="sxs-lookup"><span data-stu-id="a9dba-128">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9dba-129">Связи</span><span class="sxs-lookup"><span data-stu-id="a9dba-129">Relationships</span></span>
<span data-ttu-id="a9dba-130">Нет</span><span class="sxs-lookup"><span data-stu-id="a9dba-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9dba-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9dba-131">JSON Representation</span></span>
<span data-ttu-id="a9dba-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9dba-132">Here is a JSON representation of the resource.</span></span>
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



