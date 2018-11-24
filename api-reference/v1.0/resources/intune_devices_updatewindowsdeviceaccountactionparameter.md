# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="d3bae-101">Тип ресурса updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="d3bae-101">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="d3bae-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d3bae-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3bae-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d3bae-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="d3bae-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3bae-104">Properties</span></span>
|<span data-ttu-id="d3bae-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3bae-105">Property</span></span>|<span data-ttu-id="d3bae-106">Тип</span><span class="sxs-lookup"><span data-stu-id="d3bae-106">Type</span></span>|<span data-ttu-id="d3bae-107">Описание</span><span class="sxs-lookup"><span data-stu-id="d3bae-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3bae-108">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="d3bae-108">deviceAccount</span></span>|[<span data-ttu-id="d3bae-109">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="d3bae-109">windowsDeviceAccount</span></span>](../resources/intune_devices_windowsdeviceaccount.md)|<span data-ttu-id="d3bae-110">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d3bae-110">Not yet documented</span></span>|
|<span data-ttu-id="d3bae-111">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="d3bae-111">passwordRotationEnabled</span></span>|<span data-ttu-id="d3bae-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3bae-112">Boolean</span></span>|<span data-ttu-id="d3bae-113">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d3bae-113">Not yet documented</span></span>|
|<span data-ttu-id="d3bae-114">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="d3bae-114">calendarSyncEnabled</span></span>|<span data-ttu-id="d3bae-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3bae-115">Boolean</span></span>|<span data-ttu-id="d3bae-116">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d3bae-116">Not yet documented</span></span>|
|<span data-ttu-id="d3bae-117">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="d3bae-117">deviceAccountEmail</span></span>|<span data-ttu-id="d3bae-118">String</span><span class="sxs-lookup"><span data-stu-id="d3bae-118">String</span></span>|<span data-ttu-id="d3bae-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d3bae-119">Not yet documented</span></span>|
|<span data-ttu-id="d3bae-120">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="d3bae-120">exchangeServer</span></span>|<span data-ttu-id="d3bae-121">String</span><span class="sxs-lookup"><span data-stu-id="d3bae-121">String</span></span>|<span data-ttu-id="d3bae-122">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d3bae-122">Not yet documented</span></span>|
|<span data-ttu-id="d3bae-123">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="d3bae-123">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="d3bae-124">String</span><span class="sxs-lookup"><span data-stu-id="d3bae-124">String</span></span>|<span data-ttu-id="d3bae-125">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d3bae-125">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3bae-126">Связи</span><span class="sxs-lookup"><span data-stu-id="d3bae-126">Relationships</span></span>
<span data-ttu-id="d3bae-127">Нет</span><span class="sxs-lookup"><span data-stu-id="d3bae-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d3bae-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3bae-128">JSON Representation</span></span>
<span data-ttu-id="d3bae-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3bae-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.updateWindowsDeviceAccountActionParameter",
  "deviceAccount": {
    "@odata.type": "microsoft.graph.windowsDeviceAccount",
    "password": "String"
  },
  "passwordRotationEnabled": true,
  "calendarSyncEnabled": true,
  "deviceAccountEmail": "String",
  "exchangeServer": "String",
  "sessionInitiationProtocalAddress": "String"
}
```



