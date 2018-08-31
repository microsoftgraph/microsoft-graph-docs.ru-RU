# <a name="roledefinition-resource-type"></a><span data-ttu-id="9860d-101">Тип ресурса roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9860d-101">roleDefinition resource type</span></span>

> <span data-ttu-id="9860d-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9860d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9860d-103">Ресурс "Определение роли".</span><span class="sxs-lookup"><span data-stu-id="9860d-103">The Role Definition resource.</span></span> <span data-ttu-id="9860d-104">Определение роли лежит в основе доступа на основе ролей в Intune.</span><span class="sxs-lookup"><span data-stu-id="9860d-104">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="9860d-105">Роль сочетает в себе ресурс Intune, например мобильное приложение, и связанные разрешения роли для ресурса, такие как создание или чтение.</span><span class="sxs-lookup"><span data-stu-id="9860d-105">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="9860d-106">Есть роли двух типов: встроенные и настраиваемые.</span><span class="sxs-lookup"><span data-stu-id="9860d-106">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="9860d-107">Встроенные роли невозможно изменить.</span><span class="sxs-lookup"><span data-stu-id="9860d-107">Built-in roles cannot be modified.</span></span> <span data-ttu-id="9860d-108">Как встроенные, так и настраиваемые роли должны включать применяемые назначения.</span><span class="sxs-lookup"><span data-stu-id="9860d-108">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="9860d-109">Создайте настраиваемые роли, чтобы определить роль, которая позволяет объединить любые доступные ресурсы и разрешения роли.</span><span class="sxs-lookup"><span data-stu-id="9860d-109">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>
## <a name="methods"></a><span data-ttu-id="9860d-110">Методы</span><span class="sxs-lookup"><span data-stu-id="9860d-110">Methods</span></span>
|<span data-ttu-id="9860d-111">Метод</span><span class="sxs-lookup"><span data-stu-id="9860d-111">Method</span></span>|<span data-ttu-id="9860d-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9860d-112">Return Type</span></span>|<span data-ttu-id="9860d-113">Описание</span><span class="sxs-lookup"><span data-stu-id="9860d-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9860d-114">Перечисление объектов roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9860d-114">List roleDefinitions</span></span>](../api/intune_rbac_roledefinition_list.md)|<span data-ttu-id="9860d-115">Коллекция [roleDefinition](../resources/intune_rbac_roledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="9860d-115">[roleDefinition](../resources/intune_rbac_roledefinition.md) collection</span></span>|<span data-ttu-id="9860d-116">Список свойств и связей объектов [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9860d-116">List properties and relationships of the [roleDefinition](../resources/intune_rbac_roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="9860d-117">Получение объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9860d-117">Get roleDefinition</span></span>](../api/intune_rbac_roledefinition_get.md)|[<span data-ttu-id="9860d-118">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9860d-118">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="9860d-119">Чтение свойств и связей объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9860d-119">Read properties and relationships of the [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>|
|[<span data-ttu-id="9860d-120">Создание объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9860d-120">Create roleDefinition</span></span>](../api/intune_rbac_roledefinition_create.md)|[<span data-ttu-id="9860d-121">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9860d-121">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="9860d-122">Создание объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9860d-122">Create a new [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>|
|[<span data-ttu-id="9860d-123">Удаление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9860d-123">Delete roleDefinition</span></span>](../api/intune_rbac_roledefinition_delete.md)|<span data-ttu-id="9860d-124">Нет</span><span class="sxs-lookup"><span data-stu-id="9860d-124">None</span></span>|<span data-ttu-id="9860d-125">Удаление объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9860d-125">Deletes a [roleDefinition](../resources/intune_rbac_roledefinition.md).</span></span>|
|[<span data-ttu-id="9860d-126">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9860d-126">Update roleDefinition</span></span>](../api/intune_rbac_roledefinition_update.md)|[<span data-ttu-id="9860d-127">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="9860d-127">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="9860d-128">Обновление свойств объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9860d-128">Update the properties of a [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9860d-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="9860d-129">Properties</span></span>
|<span data-ttu-id="9860d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9860d-130">Property</span></span>|<span data-ttu-id="9860d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9860d-131">Type</span></span>|<span data-ttu-id="9860d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9860d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9860d-133">id</span><span class="sxs-lookup"><span data-stu-id="9860d-133">id</span></span>|<span data-ttu-id="9860d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9860d-134">String</span></span>|<span data-ttu-id="9860d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9860d-135">Key of the entity.</span></span> <span data-ttu-id="9860d-136">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="9860d-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="9860d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9860d-137">displayName</span></span>|<span data-ttu-id="9860d-138">String (строка)</span><span class="sxs-lookup"><span data-stu-id="9860d-138">String</span></span>|<span data-ttu-id="9860d-139">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="9860d-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="9860d-140">description</span><span class="sxs-lookup"><span data-stu-id="9860d-140">description</span></span>|<span data-ttu-id="9860d-141">String (строка)</span><span class="sxs-lookup"><span data-stu-id="9860d-141">String</span></span>|<span data-ttu-id="9860d-142">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="9860d-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="9860d-143">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="9860d-143">rolePermissions</span></span>|<span data-ttu-id="9860d-144">Коллекция [rolePermission](../resources/intune_rbac_rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="9860d-144">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="9860d-145">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="9860d-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="9860d-146">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="9860d-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="9860d-147">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="9860d-147">isBuiltIn</span></span>|<span data-ttu-id="9860d-148">Boolean (логический)</span><span class="sxs-lookup"><span data-stu-id="9860d-148">Boolean</span></span>|<span data-ttu-id="9860d-149">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="9860d-149">Type of Role.</span></span> <span data-ttu-id="9860d-150">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="9860d-150">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9860d-151">Связи</span><span class="sxs-lookup"><span data-stu-id="9860d-151">Relationships</span></span>
|<span data-ttu-id="9860d-152">Связь</span><span class="sxs-lookup"><span data-stu-id="9860d-152">Relationship</span></span>|<span data-ttu-id="9860d-153">Тип</span><span class="sxs-lookup"><span data-stu-id="9860d-153">Type</span></span>|<span data-ttu-id="9860d-154">Описание</span><span class="sxs-lookup"><span data-stu-id="9860d-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9860d-155">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="9860d-155">roleAssignments</span></span>|<span data-ttu-id="9860d-156">Коллекция объектов [roleAssignment](../resources/intune_rbac_roleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9860d-156">[roleAssignment](../resources/intune_rbac_roleassignment.md) collection</span></span>|<span data-ttu-id="9860d-157">Список назначений ролей для определения роли.</span><span class="sxs-lookup"><span data-stu-id="9860d-157">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9860d-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9860d-158">JSON Representation</span></span>
<span data-ttu-id="9860d-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9860d-159">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.roleDefinition"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```



