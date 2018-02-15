# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="1c66d-101">Тип ресурса locateDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="1c66d-101">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="1c66d-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1c66d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c66d-103">Результат действия "Поиск устройства"</span><span class="sxs-lookup"><span data-stu-id="1c66d-103">Locate device action result</span></span>

<span data-ttu-id="1c66d-104">Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1c66d-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1c66d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1c66d-105">Properties</span></span>
|<span data-ttu-id="1c66d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c66d-106">Property</span></span>|<span data-ttu-id="1c66d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1c66d-107">Type</span></span>|<span data-ttu-id="1c66d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1c66d-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c66d-109">actionName</span><span class="sxs-lookup"><span data-stu-id="1c66d-109">actionName</span></span>|<span data-ttu-id="1c66d-110">String</span><span class="sxs-lookup"><span data-stu-id="1c66d-110">String</span></span>|<span data-ttu-id="1c66d-111">Название действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1c66d-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="1c66d-112">actionState</span><span class="sxs-lookup"><span data-stu-id="1c66d-112">actionState</span></span>|<span data-ttu-id="1c66d-113">String</span><span class="sxs-lookup"><span data-stu-id="1c66d-113">String</span></span>|<span data-ttu-id="1c66d-114">Состояние действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md). Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="1c66d-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1c66d-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1c66d-115">startDateTime</span></span>|<span data-ttu-id="1c66d-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c66d-116">DateTimeOffset</span></span>|<span data-ttu-id="1c66d-117">Время начала действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1c66d-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="1c66d-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c66d-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="1c66d-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c66d-119">DateTimeOffset</span></span>|<span data-ttu-id="1c66d-120">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1c66d-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="1c66d-121">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="1c66d-121">deviceLocation</span></span>|[<span data-ttu-id="1c66d-122">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="1c66d-122">deviceGeoLocation</span></span>](../resources/intune_devices_devicegeolocation.md)|<span data-ttu-id="1c66d-123">Местоположение устройства</span><span class="sxs-lookup"><span data-stu-id="1c66d-123">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c66d-124">Связи</span><span class="sxs-lookup"><span data-stu-id="1c66d-124">Relationships</span></span>
<span data-ttu-id="1c66d-125">Нет</span><span class="sxs-lookup"><span data-stu-id="1c66d-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1c66d-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1c66d-126">JSON Representation</span></span>
<span data-ttu-id="1c66d-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c66d-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



