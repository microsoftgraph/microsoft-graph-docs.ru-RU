# <a name="devicemanagement-resource-type"></a><span data-ttu-id="65a7c-101">Тип ресурса deviceManagement</span><span class="sxs-lookup"><span data-stu-id="65a7c-101">deviceManagement resource type</span></span>

> <span data-ttu-id="65a7c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="65a7c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65a7c-103">Одноэлементный объект, служащий контейнером для всех функций управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="65a7c-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="65a7c-104">Методы</span><span class="sxs-lookup"><span data-stu-id="65a7c-104">Methods</span></span>
|<span data-ttu-id="65a7c-105">Метод</span><span class="sxs-lookup"><span data-stu-id="65a7c-105">Method</span></span>|<span data-ttu-id="65a7c-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="65a7c-106">Return Type</span></span>|<span data-ttu-id="65a7c-107">Описание</span><span class="sxs-lookup"><span data-stu-id="65a7c-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="65a7c-108">Получение объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="65a7c-108">Get deviceManagement</span></span>](../api/intune_rbac_devicemanagement_get.md)|[<span data-ttu-id="65a7c-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="65a7c-109">deviceManagement</span></span>](../resources/intune_rbac_devicemanagement.md)|<span data-ttu-id="65a7c-110">Чтение свойств и связей объекта [deviceManagement](../resources/intune_rbac_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="65a7c-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_rbac_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="65a7c-111">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="65a7c-111">Update deviceManagement</span></span>](../api/intune_rbac_devicemanagement_update.md)|[<span data-ttu-id="65a7c-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="65a7c-112">deviceManagement</span></span>](../resources/intune_rbac_devicemanagement.md)|<span data-ttu-id="65a7c-113">Обновление свойств объекта [deviceManagement](../resources/intune_rbac_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="65a7c-113">Update the properties of a [calendar](../resources/intune_rbac_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="65a7c-114">Функция getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="65a7c-114">getEffectivePermissions function</span></span>](../api/intune_rbac_devicemanagement_geteffectivepermissions.md)|<span data-ttu-id="65a7c-115">Коллекция [rolePermission](../resources/intune_rbac_rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="65a7c-115">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="65a7c-116">Получает действующие разрешения пользователя, прошедшего проверку подлинности</span><span class="sxs-lookup"><span data-stu-id="65a7c-116">Retrieves the effective permissions of the currently authenticated user</span></span>|

## <a name="properties"></a><span data-ttu-id="65a7c-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="65a7c-117">Properties</span></span>
|<span data-ttu-id="65a7c-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="65a7c-118">Property</span></span>|<span data-ttu-id="65a7c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="65a7c-119">Type</span></span>|<span data-ttu-id="65a7c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="65a7c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65a7c-121">id</span><span class="sxs-lookup"><span data-stu-id="65a7c-121">id</span></span>|<span data-ttu-id="65a7c-122">String</span><span class="sxs-lookup"><span data-stu-id="65a7c-122">String</span></span>|<span data-ttu-id="65a7c-123">Н/Д</span><span class="sxs-lookup"><span data-stu-id="65a7c-123">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="65a7c-124">Связи</span><span class="sxs-lookup"><span data-stu-id="65a7c-124">Relationships</span></span>
|<span data-ttu-id="65a7c-125">Связь</span><span class="sxs-lookup"><span data-stu-id="65a7c-125">Relationship</span></span>|<span data-ttu-id="65a7c-126">Тип</span><span class="sxs-lookup"><span data-stu-id="65a7c-126">Type</span></span>|<span data-ttu-id="65a7c-127">Описание</span><span class="sxs-lookup"><span data-stu-id="65a7c-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65a7c-128">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="65a7c-128">roleDefinitions</span></span>|<span data-ttu-id="65a7c-129">Коллекция [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="65a7c-129">[roleDefinition](../resources/intune_rbac_roledefinition.md) collection</span></span>|<span data-ttu-id="65a7c-130">Определения ролей.</span><span class="sxs-lookup"><span data-stu-id="65a7c-130">The Role Definitions.</span></span>|
|<span data-ttu-id="65a7c-131">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="65a7c-131">roleAssignments</span></span>|<span data-ttu-id="65a7c-132">Коллекция [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="65a7c-132">[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="65a7c-133">Назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="65a7c-133">The Role Assignments.</span></span>|
|<span data-ttu-id="65a7c-134">resourceOperations</span><span class="sxs-lookup"><span data-stu-id="65a7c-134">resourceOperations</span></span>|<span data-ttu-id="65a7c-135">Коллекция [resourceOperation](../resources/intune_rbac_resourceoperation.md)</span><span class="sxs-lookup"><span data-stu-id="65a7c-135">[resourceOperation](../resources/intune_rbac_resourceoperation.md) collection</span></span>|<span data-ttu-id="65a7c-136">Операции с ресурсами.</span><span class="sxs-lookup"><span data-stu-id="65a7c-136">The Resource Operations.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65a7c-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65a7c-137">JSON Representation</span></span>
<span data-ttu-id="65a7c-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65a7c-138">Here is a JSON representation of the resource.</span></span>
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



