# <a name="devicemanagement-resource-type"></a><span data-ttu-id="c8616-101">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c8616-101">deviceManagement resource type</span></span>

> <span data-ttu-id="c8616-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c8616-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8616-103">Ресурс deviceManagement представляет идентификаторы устройств из коллекции клиента, которые были предварительно подготовлены в Intune, и профили регистрации, которые можно назначать идентификаторам устройств, поддерживающим конфигурацию до регистрации.</span><span class="sxs-lookup"><span data-stu-id="c8616-103">The deviceManagement resource represents a tenant's collection device identities that have been pre-staged in Intune, and the enrollment profiles that may be assigned to device identities that support pre-enrollment configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="c8616-104">Методы</span><span class="sxs-lookup"><span data-stu-id="c8616-104">Methods</span></span>
|<span data-ttu-id="c8616-105">Метод</span><span class="sxs-lookup"><span data-stu-id="c8616-105">Method</span></span>|<span data-ttu-id="c8616-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c8616-106">Return Type</span></span>|<span data-ttu-id="c8616-107">Описание</span><span class="sxs-lookup"><span data-stu-id="c8616-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c8616-108">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c8616-108">Get deviceManagement</span></span>](../api/intune_enrollment_devicemanagement_get.md)|[<span data-ttu-id="c8616-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c8616-109">deviceManagement</span></span>](../resources/intune_enrollment_devicemanagement.md)|<span data-ttu-id="c8616-110">Чтение свойств и связей объекта [deviceManagement](../resources/intune_enrollment_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="c8616-110">Read properties and relationships of the [deviceManagement](../resources/intune_enrollment_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="c8616-111">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c8616-111">Update deviceManagement</span></span>](../api/intune_enrollment_devicemanagement_update.md)|[<span data-ttu-id="c8616-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="c8616-112">deviceManagement</span></span>](../resources/intune_enrollment_devicemanagement.md)|<span data-ttu-id="c8616-113">Обновление свойств объекта [deviceManagement](../resources/intune_enrollment_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="c8616-113">Update the properties of a [deviceManagement](../resources/intune_enrollment_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c8616-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8616-114">Properties</span></span>
|<span data-ttu-id="c8616-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8616-115">Property</span></span>|<span data-ttu-id="c8616-116">Тип</span><span class="sxs-lookup"><span data-stu-id="c8616-116">Type</span></span>|<span data-ttu-id="c8616-117">Описание</span><span class="sxs-lookup"><span data-stu-id="c8616-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8616-118">id</span><span class="sxs-lookup"><span data-stu-id="c8616-118">id</span></span>|<span data-ttu-id="c8616-119">String</span><span class="sxs-lookup"><span data-stu-id="c8616-119">String</span></span>|<span data-ttu-id="c8616-120">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="c8616-120">The GUID for the object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8616-121">Связи</span><span class="sxs-lookup"><span data-stu-id="c8616-121">Relationships</span></span>
|<span data-ttu-id="c8616-122">Связь</span><span class="sxs-lookup"><span data-stu-id="c8616-122">Relationship</span></span>|<span data-ttu-id="c8616-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c8616-123">Type</span></span>|<span data-ttu-id="c8616-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c8616-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8616-125">importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="c8616-125">importedWindowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="c8616-126">Коллекция [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="c8616-126">[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="c8616-127">Коллекция импортированных устройств Windows AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="c8616-127">Collection of imported Windows autopilot devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c8616-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c8616-128">JSON Representation</span></span>
<span data-ttu-id="c8616-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8616-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



