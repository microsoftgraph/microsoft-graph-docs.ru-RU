---
title: Тип ресурса locateDeviceActionResult
description: Результат действия "Поиск устройства"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e7f32d1eb4a47e86f072d17e2e3bcf81160f835b
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612065"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="1263c-103">Тип ресурса locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="1263c-103">locateDeviceActionResult resource type</span></span>

<span data-ttu-id="1263c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1263c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1263c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1263c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1263c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1263c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1263c-107">Результат действия "Поиск устройства"</span><span class="sxs-lookup"><span data-stu-id="1263c-107">Locate device action result</span></span>


<span data-ttu-id="1263c-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1263c-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1263c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1263c-109">Properties</span></span>
|<span data-ttu-id="1263c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1263c-110">Property</span></span>|<span data-ttu-id="1263c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1263c-111">Type</span></span>|<span data-ttu-id="1263c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1263c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1263c-113">actionName</span><span class="sxs-lookup"><span data-stu-id="1263c-113">actionName</span></span>|<span data-ttu-id="1263c-114">String</span><span class="sxs-lookup"><span data-stu-id="1263c-114">String</span></span>|<span data-ttu-id="1263c-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="1263c-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1263c-116">actionState</span><span class="sxs-lookup"><span data-stu-id="1263c-116">actionState</span></span>|[<span data-ttu-id="1263c-117">actionState</span><span class="sxs-lookup"><span data-stu-id="1263c-117">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="1263c-118">Состояние действия, унаследованной от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="1263c-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="1263c-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="1263c-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1263c-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1263c-120">startDateTime</span></span>|<span data-ttu-id="1263c-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1263c-121">DateTimeOffset</span></span>|<span data-ttu-id="1263c-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="1263c-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1263c-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1263c-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="1263c-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1263c-124">DateTimeOffset</span></span>|<span data-ttu-id="1263c-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1263c-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1263c-126">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="1263c-126">deviceLocation</span></span>|[<span data-ttu-id="1263c-127">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="1263c-127">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="1263c-128">Местоположение устройства</span><span class="sxs-lookup"><span data-stu-id="1263c-128">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="1263c-129">Связи</span><span class="sxs-lookup"><span data-stu-id="1263c-129">Relationships</span></span>
<span data-ttu-id="1263c-130">Нет</span><span class="sxs-lookup"><span data-stu-id="1263c-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1263c-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1263c-131">JSON Representation</span></span>
<span data-ttu-id="1263c-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1263c-132">Here is a JSON representation of the resource.</span></span>
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




