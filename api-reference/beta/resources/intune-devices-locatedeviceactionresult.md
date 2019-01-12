---
title: Тип ресурса locateDeviceActionResult
description: Результат действия "Поиск устройства"
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f342f26916b1144a317d02871364e25da2d8c4d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912458"
---
# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="af801-103">Тип ресурса locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="af801-103">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="af801-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="af801-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af801-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af801-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af801-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="af801-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af801-107">Результат действия "Поиск устройства"</span><span class="sxs-lookup"><span data-stu-id="af801-107">Locate device action result</span></span>

<span data-ttu-id="af801-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="af801-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="af801-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="af801-109">Properties</span></span>
|<span data-ttu-id="af801-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="af801-110">Property</span></span>|<span data-ttu-id="af801-111">Тип</span><span class="sxs-lookup"><span data-stu-id="af801-111">Type</span></span>|<span data-ttu-id="af801-112">Описание</span><span class="sxs-lookup"><span data-stu-id="af801-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af801-113">actionName</span><span class="sxs-lookup"><span data-stu-id="af801-113">actionName</span></span>|<span data-ttu-id="af801-114">String</span><span class="sxs-lookup"><span data-stu-id="af801-114">String</span></span>|<span data-ttu-id="af801-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="af801-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="af801-116">actionState</span><span class="sxs-lookup"><span data-stu-id="af801-116">actionState</span></span>|[<span data-ttu-id="af801-117">actionState</span><span class="sxs-lookup"><span data-stu-id="af801-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="af801-118">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="af801-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="af801-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="af801-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="af801-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="af801-120">startDateTime</span></span>|<span data-ttu-id="af801-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af801-121">DateTimeOffset</span></span>|<span data-ttu-id="af801-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="af801-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="af801-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="af801-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="af801-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af801-124">DateTimeOffset</span></span>|<span data-ttu-id="af801-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="af801-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="af801-126">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="af801-126">deviceLocation</span></span>|[<span data-ttu-id="af801-127">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="af801-127">deviceGeoLocation</span></span>](../resources/intune-devices-devicegeolocation.md)|<span data-ttu-id="af801-128">Местоположение устройства</span><span class="sxs-lookup"><span data-stu-id="af801-128">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="af801-129">Связи</span><span class="sxs-lookup"><span data-stu-id="af801-129">Relationships</span></span>
<span data-ttu-id="af801-130">Нет</span><span class="sxs-lookup"><span data-stu-id="af801-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="af801-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af801-131">JSON Representation</span></span>
<span data-ttu-id="af801-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af801-132">Here is a JSON representation of the resource.</span></span>
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





