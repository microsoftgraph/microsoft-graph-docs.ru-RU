# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="994dc-101">Тип ресурса updateWindowsDeviceAccountActionParameter</span><span class="sxs-lookup"><span data-stu-id="994dc-101">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="994dc-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="994dc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="994dc-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="994dc-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="994dc-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="994dc-104">Properties</span></span>
|<span data-ttu-id="994dc-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="994dc-105">Property</span></span>|<span data-ttu-id="994dc-106">Тип</span><span class="sxs-lookup"><span data-stu-id="994dc-106">Type</span></span>|<span data-ttu-id="994dc-107">Описание</span><span class="sxs-lookup"><span data-stu-id="994dc-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="994dc-108">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="994dc-108">deviceAccount</span></span>|[<span data-ttu-id="994dc-109">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="994dc-109">windowsDeviceAccount</span></span>](../resources/intune_devices_windowsdeviceaccount.md)|<span data-ttu-id="994dc-110">Н/Д</span><span class="sxs-lookup"><span data-stu-id="994dc-110">Not yet documented</span></span>|
|<span data-ttu-id="994dc-111">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="994dc-111">passwordRotationEnabled</span></span>|<span data-ttu-id="994dc-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="994dc-112">Boolean</span></span>|<span data-ttu-id="994dc-113">Н/Д</span><span class="sxs-lookup"><span data-stu-id="994dc-113">Not yet documented</span></span>|
|<span data-ttu-id="994dc-114">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="994dc-114">calendarSyncEnabled</span></span>|<span data-ttu-id="994dc-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="994dc-115">Boolean</span></span>|<span data-ttu-id="994dc-116">Н/Д</span><span class="sxs-lookup"><span data-stu-id="994dc-116">Not yet documented</span></span>|
|<span data-ttu-id="994dc-117">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="994dc-117">deviceAccountEmail</span></span>|<span data-ttu-id="994dc-118">String</span><span class="sxs-lookup"><span data-stu-id="994dc-118">String</span></span>|<span data-ttu-id="994dc-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="994dc-119">Not yet documented</span></span>|
|<span data-ttu-id="994dc-120">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="994dc-120">exchangeServer</span></span>|<span data-ttu-id="994dc-121">String</span><span class="sxs-lookup"><span data-stu-id="994dc-121">String</span></span>|<span data-ttu-id="994dc-122">Н/Д</span><span class="sxs-lookup"><span data-stu-id="994dc-122">Not yet documented</span></span>|
|<span data-ttu-id="994dc-123">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="994dc-123">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="994dc-124">String</span><span class="sxs-lookup"><span data-stu-id="994dc-124">String</span></span>|<span data-ttu-id="994dc-125">Н/Д</span><span class="sxs-lookup"><span data-stu-id="994dc-125">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="994dc-126">Связи</span><span class="sxs-lookup"><span data-stu-id="994dc-126">Relationships</span></span>
<span data-ttu-id="994dc-127">Нет</span><span class="sxs-lookup"><span data-stu-id="994dc-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="994dc-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="994dc-128">JSON Representation</span></span>
<span data-ttu-id="994dc-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="994dc-129">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}-->
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








