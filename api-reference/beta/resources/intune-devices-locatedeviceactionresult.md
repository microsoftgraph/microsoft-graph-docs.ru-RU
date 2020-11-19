---
title: Тип ресурса locateDeviceActionResult
description: Результат действия "Поиск устройства"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ea30fe76b55f65262dabc94fe52394fdc2a4c2cf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49208963"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="df072-103">Тип ресурса locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="df072-103">locateDeviceActionResult resource type</span></span>

<span data-ttu-id="df072-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df072-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df072-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df072-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df072-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="df072-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df072-107">Результат действия "Поиск устройства"</span><span class="sxs-lookup"><span data-stu-id="df072-107">Locate device action result</span></span>


<span data-ttu-id="df072-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="df072-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="df072-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="df072-109">Properties</span></span>
|<span data-ttu-id="df072-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="df072-110">Property</span></span>|<span data-ttu-id="df072-111">Тип</span><span class="sxs-lookup"><span data-stu-id="df072-111">Type</span></span>|<span data-ttu-id="df072-112">Описание</span><span class="sxs-lookup"><span data-stu-id="df072-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df072-113">actionName</span><span class="sxs-lookup"><span data-stu-id="df072-113">actionName</span></span>|<span data-ttu-id="df072-114">String</span><span class="sxs-lookup"><span data-stu-id="df072-114">String</span></span>|<span data-ttu-id="df072-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="df072-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="df072-116">actionState</span><span class="sxs-lookup"><span data-stu-id="df072-116">actionState</span></span>|[<span data-ttu-id="df072-117">actionState</span><span class="sxs-lookup"><span data-stu-id="df072-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="df072-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="df072-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="df072-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="df072-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="df072-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="df072-120">startDateTime</span></span>|<span data-ttu-id="df072-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df072-121">DateTimeOffset</span></span>|<span data-ttu-id="df072-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="df072-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="df072-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="df072-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="df072-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df072-124">DateTimeOffset</span></span>|<span data-ttu-id="df072-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="df072-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="df072-126">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="df072-126">deviceLocation</span></span>|[<span data-ttu-id="df072-127">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="df072-127">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="df072-128">Местоположение устройства</span><span class="sxs-lookup"><span data-stu-id="df072-128">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="df072-129">Связи</span><span class="sxs-lookup"><span data-stu-id="df072-129">Relationships</span></span>
<span data-ttu-id="df072-130">Нет</span><span class="sxs-lookup"><span data-stu-id="df072-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df072-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="df072-131">JSON Representation</span></span>
<span data-ttu-id="df072-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df072-132">Here is a JSON representation of the resource.</span></span>
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
    "longitude": "4.2",
    "latitude": "4.2",
    "altitude": "4.2",
    "horizontalAccuracy": "4.2",
    "verticalAccuracy": "4.2",
    "heading": "4.2",
    "speed": "4.2"
  }
}
```




