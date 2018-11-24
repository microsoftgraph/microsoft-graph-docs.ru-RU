# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="cec8a-101">Обновление объекта deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="cec8a-101">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="cec8a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cec8a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cec8a-103">Обновление свойств объекта [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cec8a-103">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cec8a-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="cec8a-104">Prerequisites</span></span>
<span data-ttu-id="cec8a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cec8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cec8a-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cec8a-107">Permission type</span></span>|<span data-ttu-id="cec8a-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cec8a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cec8a-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cec8a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cec8a-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cec8a-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="cec8a-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cec8a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cec8a-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cec8a-112">Not supported.</span></span>|
|<span data-ttu-id="cec8a-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cec8a-113">Application</span></span>|<span data-ttu-id="cec8a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cec8a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cec8a-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cec8a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="cec8a-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cec8a-116">Request headers</span></span>
|<span data-ttu-id="cec8a-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cec8a-117">Header</span></span>|<span data-ttu-id="cec8a-118">Значение</span><span class="sxs-lookup"><span data-stu-id="cec8a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cec8a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="cec8a-119">Authorization</span></span>|<span data-ttu-id="cec8a-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cec8a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cec8a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="cec8a-121">Accept</span></span>|<span data-ttu-id="cec8a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="cec8a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cec8a-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cec8a-123">Request body</span></span>
<span data-ttu-id="cec8a-124">В теле запроса добавьте представление объекта [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cec8a-124">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="cec8a-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cec8a-125">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="cec8a-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="cec8a-126">Property</span></span>|<span data-ttu-id="cec8a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="cec8a-127">Type</span></span>|<span data-ttu-id="cec8a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="cec8a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cec8a-129">id</span><span class="sxs-lookup"><span data-stu-id="cec8a-129">id</span></span>|<span data-ttu-id="cec8a-130">String</span><span class="sxs-lookup"><span data-stu-id="cec8a-130">String</span></span>|<span data-ttu-id="cec8a-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cec8a-131">Key of the entity.</span></span> <span data-ttu-id="cec8a-132">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="cec8a-132">This is read-only and automatically generated.</span></span> <span data-ttu-id="cec8a-133">Наследуется от объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cec8a-133">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="cec8a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="cec8a-134">displayName</span></span>|<span data-ttu-id="cec8a-135">String</span><span class="sxs-lookup"><span data-stu-id="cec8a-135">String</span></span>|<span data-ttu-id="cec8a-136">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="cec8a-136">Display Name of the Role definition.</span></span> <span data-ttu-id="cec8a-137">Наследуется от объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cec8a-137">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="cec8a-138">description</span><span class="sxs-lookup"><span data-stu-id="cec8a-138">description</span></span>|<span data-ttu-id="cec8a-139">String</span><span class="sxs-lookup"><span data-stu-id="cec8a-139">String</span></span>|<span data-ttu-id="cec8a-140">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="cec8a-140">Description of the Role definition.</span></span> <span data-ttu-id="cec8a-141">Наследуется от объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cec8a-141">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="cec8a-142">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="cec8a-142">rolePermissions</span></span>|<span data-ttu-id="cec8a-143">Коллекция [rolePermission](../resources/intune_rbac_rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="cec8a-143">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="cec8a-144">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="cec8a-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="cec8a-145">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="cec8a-145">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="cec8a-146">Наследуется от объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cec8a-146">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="cec8a-147">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="cec8a-147">isBuiltIn</span></span>|<span data-ttu-id="cec8a-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="cec8a-148">Boolean</span></span>|<span data-ttu-id="cec8a-149">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="cec8a-149">Type of Role.</span></span> <span data-ttu-id="cec8a-150">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="cec8a-150">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="cec8a-151">Наследуется от объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cec8a-151">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="cec8a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="cec8a-152">Response</span></span>
<span data-ttu-id="cec8a-153">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cec8a-153">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cec8a-154">Пример</span><span class="sxs-lookup"><span data-stu-id="cec8a-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="cec8a-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="cec8a-155">Request</span></span>
<span data-ttu-id="cec8a-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cec8a-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="cec8a-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="cec8a-157">Response</span></span>
<span data-ttu-id="cec8a-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cec8a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```



