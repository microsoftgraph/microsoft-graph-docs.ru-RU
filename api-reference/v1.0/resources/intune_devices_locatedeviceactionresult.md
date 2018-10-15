# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="ee05c-101">Тип ресурса locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="ee05c-101">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="ee05c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ee05c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee05c-103">Результат действия "Поиск устройства"</span><span class="sxs-lookup"><span data-stu-id="ee05c-103">Locate device action result</span></span>

<span data-ttu-id="ee05c-104">Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ee05c-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ee05c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee05c-105">Properties</span></span>
|<span data-ttu-id="ee05c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee05c-106">Property</span></span>|<span data-ttu-id="ee05c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ee05c-107">Type</span></span>|<span data-ttu-id="ee05c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ee05c-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee05c-109">actionName</span><span class="sxs-lookup"><span data-stu-id="ee05c-109">actionName</span></span>|<span data-ttu-id="ee05c-110">Строка</span><span class="sxs-lookup"><span data-stu-id="ee05c-110">String</span></span>|<span data-ttu-id="ee05c-111">Название действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ee05c-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="ee05c-112">actionState</span><span class="sxs-lookup"><span data-stu-id="ee05c-112">actionState</span></span>|[<span data-ttu-id="ee05c-113">actionState</span><span class="sxs-lookup"><span data-stu-id="ee05c-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="ee05c-p101">Состояние действия наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md). Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="ee05c-p101">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ee05c-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ee05c-116">startDateTime</span></span>|<span data-ttu-id="ee05c-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee05c-117">DateTimeOffset</span></span>|<span data-ttu-id="ee05c-118">Время начала действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ee05c-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="ee05c-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ee05c-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="ee05c-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee05c-120">DateTimeOffset</span></span>|<span data-ttu-id="ee05c-121">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ee05c-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="ee05c-122">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="ee05c-122">deviceLocation</span></span>|[<span data-ttu-id="ee05c-123">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="ee05c-123">deviceGeoLocation</span></span>](../resources/intune_devices_devicegeolocation.md)|<span data-ttu-id="ee05c-124">Местоположение устройства</span><span class="sxs-lookup"><span data-stu-id="ee05c-124">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee05c-125">Связи</span><span class="sxs-lookup"><span data-stu-id="ee05c-125">Relationships</span></span>
<span data-ttu-id="ee05c-126">Нет</span><span class="sxs-lookup"><span data-stu-id="ee05c-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ee05c-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee05c-127">JSON Representation</span></span>
<span data-ttu-id="ee05c-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ee05c-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.locateDeviceActionResult"
}-->
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








