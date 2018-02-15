# <a name="manageddevice-resource-type"></a><span data-ttu-id="821d0-101">Тип ресурса managedDevice</span><span class="sxs-lookup"><span data-stu-id="821d0-101">managedDevice resource type</span></span>

> <span data-ttu-id="821d0-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="821d0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="821d0-103">Устройства, которые управляются или предварительно регистрируются с помощью Intune</span><span class="sxs-lookup"><span data-stu-id="821d0-103">Devices that are managed or pre-enrolled through Intune</span></span>
## <a name="methods"></a><span data-ttu-id="821d0-104">Методы</span><span class="sxs-lookup"><span data-stu-id="821d0-104">Methods</span></span>
|<span data-ttu-id="821d0-105">Метод</span><span class="sxs-lookup"><span data-stu-id="821d0-105">Method</span></span>|<span data-ttu-id="821d0-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="821d0-106">Return Type</span></span>|<span data-ttu-id="821d0-107">Описание</span><span class="sxs-lookup"><span data-stu-id="821d0-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="821d0-108">Список объектов managedDevice</span><span class="sxs-lookup"><span data-stu-id="821d0-108">List managedDevices</span></span>](../api/intune_deviceconfig_manageddevice_list.md)|<span data-ttu-id="821d0-109">Коллекция [managedDevice](../resources/intune_deviceconfig_manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="821d0-109">[managedDevice](../resources/intune_deviceconfig_manageddevice.md) collection</span></span>|<span data-ttu-id="821d0-110">Список свойств и связей объектов [managedDevice](../resources/intune_deviceconfig_manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="821d0-110">List properties and relationships of the [managedDevice](../resources/intune_deviceconfig_manageddevice.md) objects.</span></span>|
|[<span data-ttu-id="821d0-111">Получение объекта managedDevice</span><span class="sxs-lookup"><span data-stu-id="821d0-111">Get managedDevice</span></span>](../api/intune_deviceconfig_manageddevice_get.md)|[<span data-ttu-id="821d0-112">managedDevice</span><span class="sxs-lookup"><span data-stu-id="821d0-112">managedDevice</span></span>](../resources/intune_deviceconfig_manageddevice.md)|<span data-ttu-id="821d0-113">Чтение свойств и связей объекта [managedDevice](../resources/intune_deviceconfig_manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="821d0-113">Read properties and relationships of [plannerPlanDetails](../resources/intune_deviceconfig_manageddevice.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="821d0-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="821d0-114">Properties</span></span>
|<span data-ttu-id="821d0-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="821d0-115">Property</span></span>|<span data-ttu-id="821d0-116">Тип</span><span class="sxs-lookup"><span data-stu-id="821d0-116">Type</span></span>|<span data-ttu-id="821d0-117">Описание</span><span class="sxs-lookup"><span data-stu-id="821d0-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="821d0-118">id</span><span class="sxs-lookup"><span data-stu-id="821d0-118">id</span></span>|<span data-ttu-id="821d0-119">String</span><span class="sxs-lookup"><span data-stu-id="821d0-119">String</span></span>|<span data-ttu-id="821d0-120">Н/Д</span><span class="sxs-lookup"><span data-stu-id="821d0-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="821d0-121">Связи</span><span class="sxs-lookup"><span data-stu-id="821d0-121">Relationships</span></span>
|<span data-ttu-id="821d0-122">Связь</span><span class="sxs-lookup"><span data-stu-id="821d0-122">Relationship</span></span>|<span data-ttu-id="821d0-123">Тип</span><span class="sxs-lookup"><span data-stu-id="821d0-123">Type</span></span>|<span data-ttu-id="821d0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="821d0-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="821d0-125">deviceConfigurationStates</span><span class="sxs-lookup"><span data-stu-id="821d0-125">deviceConfigurationStates</span></span>|<span data-ttu-id="821d0-126">Коллекция [deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md)</span><span class="sxs-lookup"><span data-stu-id="821d0-126">[deviceConfigurationState](../resources/intune_deviceconfig_deviceconfigurationstate.md) collection</span></span>|<span data-ttu-id="821d0-127">Состояния конфигурации этого устройства.</span><span class="sxs-lookup"><span data-stu-id="821d0-127">Device configuration states for this device.</span></span>|
|<span data-ttu-id="821d0-128">deviceCompliancePolicyStates</span><span class="sxs-lookup"><span data-stu-id="821d0-128">deviceCompliancePolicyStates</span></span>|<span data-ttu-id="821d0-129">Коллекция [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md)</span><span class="sxs-lookup"><span data-stu-id="821d0-129">[deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) collection</span></span>|<span data-ttu-id="821d0-130">Состояния политики соответствия требованиям для этого устройства.</span><span class="sxs-lookup"><span data-stu-id="821d0-130">Device compliance policy states for this device.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="821d0-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="821d0-131">JSON Representation</span></span>
<span data-ttu-id="821d0-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="821d0-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)"
}
```



