---
title: Тип ресурса locateDeviceActionResult
description: Результат действия "Поиск устройства"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0fc2fa997d56fffd673964a1d387b175bfef2ba1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754562"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="b5901-103">Тип ресурса locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="b5901-103">locateDeviceActionResult resource type</span></span>

<span data-ttu-id="b5901-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5901-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5901-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b5901-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5901-106">Результат действия "Поиск устройства"</span><span class="sxs-lookup"><span data-stu-id="b5901-106">Locate device action result</span></span>


<span data-ttu-id="b5901-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b5901-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b5901-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5901-108">Properties</span></span>
|<span data-ttu-id="b5901-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5901-109">Property</span></span>|<span data-ttu-id="b5901-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b5901-110">Type</span></span>|<span data-ttu-id="b5901-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b5901-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5901-112">actionName</span><span class="sxs-lookup"><span data-stu-id="b5901-112">actionName</span></span>|<span data-ttu-id="b5901-113">String</span><span class="sxs-lookup"><span data-stu-id="b5901-113">String</span></span>|<span data-ttu-id="b5901-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b5901-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b5901-115">actionState</span><span class="sxs-lookup"><span data-stu-id="b5901-115">actionState</span></span>|[<span data-ttu-id="b5901-116">actionState</span><span class="sxs-lookup"><span data-stu-id="b5901-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="b5901-117">Состояние действия, унаследованной от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b5901-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b5901-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b5901-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b5901-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b5901-119">startDateTime</span></span>|<span data-ttu-id="b5901-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5901-120">DateTimeOffset</span></span>|<span data-ttu-id="b5901-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b5901-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b5901-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5901-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="b5901-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5901-123">DateTimeOffset</span></span>|<span data-ttu-id="b5901-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b5901-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b5901-125">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="b5901-125">deviceLocation</span></span>|[<span data-ttu-id="b5901-126">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="b5901-126">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="b5901-127">Местоположение устройства</span><span class="sxs-lookup"><span data-stu-id="b5901-127">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5901-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="b5901-128">Relationships</span></span>
<span data-ttu-id="b5901-129">Нет</span><span class="sxs-lookup"><span data-stu-id="b5901-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5901-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b5901-130">JSON Representation</span></span>
<span data-ttu-id="b5901-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5901-131">Here is a JSON representation of the resource.</span></span>
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




