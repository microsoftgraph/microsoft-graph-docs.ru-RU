# <a name="devicegeolocation-resource-type"></a><span data-ttu-id="12d10-101">Тип ресурса deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="12d10-101">deviceGeoLocation resource type</span></span>

> <span data-ttu-id="12d10-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="12d10-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12d10-103">Расположение устройства</span><span class="sxs-lookup"><span data-stu-id="12d10-103">Device location</span></span>
## <a name="properties"></a><span data-ttu-id="12d10-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="12d10-104">Properties</span></span>
|<span data-ttu-id="12d10-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="12d10-105">Property</span></span>|<span data-ttu-id="12d10-106">Тип</span><span class="sxs-lookup"><span data-stu-id="12d10-106">Type</span></span>|<span data-ttu-id="12d10-107">Описание</span><span class="sxs-lookup"><span data-stu-id="12d10-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12d10-108">lastCollectedDateTime</span><span class="sxs-lookup"><span data-stu-id="12d10-108">lastCollectedDateTime</span></span>|<span data-ttu-id="12d10-109">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12d10-109">DateTimeOffset</span></span>|<span data-ttu-id="12d10-110">Время записи расположения относительно времени UTC</span><span class="sxs-lookup"><span data-stu-id="12d10-110">Time at which location was recorded, relative to UTC</span></span>|
|<span data-ttu-id="12d10-111">longitude</span><span class="sxs-lookup"><span data-stu-id="12d10-111">longitude</span></span>|<span data-ttu-id="12d10-112">Double</span><span class="sxs-lookup"><span data-stu-id="12d10-112">Double</span></span>|<span data-ttu-id="12d10-113">Долгота расположения устройства</span><span class="sxs-lookup"><span data-stu-id="12d10-113">Longitude coordinate of the device's location</span></span>|
|<span data-ttu-id="12d10-114">latitude</span><span class="sxs-lookup"><span data-stu-id="12d10-114">latitude</span></span>|<span data-ttu-id="12d10-115">Double</span><span class="sxs-lookup"><span data-stu-id="12d10-115">Double</span></span>|<span data-ttu-id="12d10-116">Широта расположения устройства</span><span class="sxs-lookup"><span data-stu-id="12d10-116">Latitude coordinate of the device's location</span></span>|
|<span data-ttu-id="12d10-117">altitude</span><span class="sxs-lookup"><span data-stu-id="12d10-117">altitude</span></span>|<span data-ttu-id="12d10-118">Double</span><span class="sxs-lookup"><span data-stu-id="12d10-118">Double</span></span>|<span data-ttu-id="12d10-119">Высота (метров над уровнем моря)</span><span class="sxs-lookup"><span data-stu-id="12d10-119">Altitude, given in meters above sea level</span></span>|
|<span data-ttu-id="12d10-120">horizontalAccuracy</span><span class="sxs-lookup"><span data-stu-id="12d10-120">horizontalAccuracy</span></span>|<span data-ttu-id="12d10-121">Double</span><span class="sxs-lookup"><span data-stu-id="12d10-121">Double</span></span>|<span data-ttu-id="12d10-122">Точность долготы и широты (м)</span><span class="sxs-lookup"><span data-stu-id="12d10-122">Accuracy of longitude and latitude in meters</span></span>|
|<span data-ttu-id="12d10-123">verticalAccuracy</span><span class="sxs-lookup"><span data-stu-id="12d10-123">verticalAccuracy</span></span>|<span data-ttu-id="12d10-124">Double</span><span class="sxs-lookup"><span data-stu-id="12d10-124">Double</span></span>|<span data-ttu-id="12d10-125">Точность высоты (м)</span><span class="sxs-lookup"><span data-stu-id="12d10-125">Accuracy of altitude in meters</span></span>|
|<span data-ttu-id="12d10-126">heading</span><span class="sxs-lookup"><span data-stu-id="12d10-126">heading</span></span>|<span data-ttu-id="12d10-127">Double</span><span class="sxs-lookup"><span data-stu-id="12d10-127">Double</span></span>|<span data-ttu-id="12d10-128">Направление от географического севера (градусов)</span><span class="sxs-lookup"><span data-stu-id="12d10-128">Heading in degrees from true north</span></span>|
|<span data-ttu-id="12d10-129">speed</span><span class="sxs-lookup"><span data-stu-id="12d10-129">speed</span></span>|<span data-ttu-id="12d10-130">Double</span><span class="sxs-lookup"><span data-stu-id="12d10-130">Double</span></span>|<span data-ttu-id="12d10-131">Скорость передвижения устройства (м/с)</span><span class="sxs-lookup"><span data-stu-id="12d10-131">Speed the device is traveling in meters per second</span></span>|

## <a name="relationships"></a><span data-ttu-id="12d10-132">Связи</span><span class="sxs-lookup"><span data-stu-id="12d10-132">Relationships</span></span>
<span data-ttu-id="12d10-133">Нет</span><span class="sxs-lookup"><span data-stu-id="12d10-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="12d10-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="12d10-134">JSON Representation</span></span>
<span data-ttu-id="12d10-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12d10-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "lastCollectedDateTime": "String (timestamp)",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "altitude": "<Unknown Primitive Type Edm.Double>",
  "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
  "heading": "<Unknown Primitive Type Edm.Double>",
  "speed": "<Unknown Primitive Type Edm.Double>"
}
```



