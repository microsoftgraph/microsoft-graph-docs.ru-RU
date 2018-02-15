# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="3299c-101">Тип ресурса deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="3299c-101">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="3299c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3299c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3299c-103">Объект назначения конфигурации устройств назначает группу AAD определенной конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="3299c-103">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="3299c-104">Методы</span><span class="sxs-lookup"><span data-stu-id="3299c-104">Methods</span></span>
|<span data-ttu-id="3299c-105">Метод</span><span class="sxs-lookup"><span data-stu-id="3299c-105">Method</span></span>|<span data-ttu-id="3299c-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3299c-106">Return Type</span></span>|<span data-ttu-id="3299c-107">Описание</span><span class="sxs-lookup"><span data-stu-id="3299c-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3299c-108">Список объектов deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="3299c-108">List deviceConfigurationAssignments</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_list.md)|<span data-ttu-id="3299c-109">Коллекция [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3299c-109">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3299c-110">Список свойств и связей объектов [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3299c-110">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="3299c-111">Получение объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="3299c-111">Get deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_get.md)|[<span data-ttu-id="3299c-112">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="3299c-112">deviceConfigurationAssignment</span></span>](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|<span data-ttu-id="3299c-113">Чтение свойств и связей объекта [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3299c-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="3299c-114">Создание объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="3299c-114">Create deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_create.md)|[<span data-ttu-id="3299c-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="3299c-115">deviceConfigurationAssignment</span></span>](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|<span data-ttu-id="3299c-116">Создание объекта [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3299c-116">Create a new [plannerBucket](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="3299c-117">Удаление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="3299c-117">Delete deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_delete.md)|<span data-ttu-id="3299c-118">Нет</span><span class="sxs-lookup"><span data-stu-id="3299c-118">None</span></span>|<span data-ttu-id="3299c-119">Удаляет объект [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3299c-119">Deletes a [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="3299c-120">Обновление объекта deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="3299c-120">Update deviceConfigurationAssignment</span></span>](../api/intune_deviceconfig_deviceconfigurationassignment_update.md)|[<span data-ttu-id="3299c-121">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="3299c-121">deviceConfigurationAssignment</span></span>](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|<span data-ttu-id="3299c-122">Обновление свойств объекта [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3299c-122">Update the properties of a [calendar](../resources/intune_deviceconfig_deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3299c-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="3299c-123">Properties</span></span>
|<span data-ttu-id="3299c-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="3299c-124">Property</span></span>|<span data-ttu-id="3299c-125">Тип</span><span class="sxs-lookup"><span data-stu-id="3299c-125">Type</span></span>|<span data-ttu-id="3299c-126">Описание</span><span class="sxs-lookup"><span data-stu-id="3299c-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3299c-127">id</span><span class="sxs-lookup"><span data-stu-id="3299c-127">id</span></span>|<span data-ttu-id="3299c-128">String</span><span class="sxs-lookup"><span data-stu-id="3299c-128">String</span></span>|<span data-ttu-id="3299c-129">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="3299c-129">The key of the setting.</span></span>|
|<span data-ttu-id="3299c-130">target</span><span class="sxs-lookup"><span data-stu-id="3299c-130">target</span></span>|[<span data-ttu-id="3299c-131">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3299c-131">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_deviceconfig_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3299c-132">Цель назначения для конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="3299c-132">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3299c-133">Связи</span><span class="sxs-lookup"><span data-stu-id="3299c-133">Relationships</span></span>
<span data-ttu-id="3299c-134">Нет</span><span class="sxs-lookup"><span data-stu-id="3299c-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3299c-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3299c-135">JSON Representation</span></span>
<span data-ttu-id="3299c-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3299c-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



