# <a name="update-roledefinition"></a><span data-ttu-id="04e50-101">Обновление объекта roleDefinition</span><span class="sxs-lookup"><span data-stu-id="04e50-101">Update roleDefinition</span></span>

> <span data-ttu-id="04e50-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="04e50-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04e50-103">Обновление свойств объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="04e50-103">Update the properties of a [calendar](../resources/intune_rbac_roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="04e50-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="04e50-104">Prerequisites</span></span>
<span data-ttu-id="04e50-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="04e50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="04e50-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04e50-107">Permission type</span></span>|<span data-ttu-id="04e50-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="04e50-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04e50-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04e50-109">Delegated (work or school account)</span></span>|<span data-ttu-id="04e50-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04e50-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="04e50-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04e50-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04e50-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04e50-112">Not supported.</span></span>|
|<span data-ttu-id="04e50-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04e50-113">Application</span></span>|<span data-ttu-id="04e50-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04e50-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04e50-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04e50-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="04e50-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04e50-116">Request headers</span></span>
|<span data-ttu-id="04e50-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04e50-117">Header</span></span>|<span data-ttu-id="04e50-118">Значение</span><span class="sxs-lookup"><span data-stu-id="04e50-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04e50-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="04e50-119">Authorization</span></span>|<span data-ttu-id="04e50-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04e50-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="04e50-121">Accept</span><span class="sxs-lookup"><span data-stu-id="04e50-121">Accept</span></span>|<span data-ttu-id="04e50-122">application/json</span><span class="sxs-lookup"><span data-stu-id="04e50-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04e50-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="04e50-123">Request body</span></span>
<span data-ttu-id="04e50-124">В теле запроса добавьте представление объекта [roleDefinition](../resources/intune_rbac_roledefinition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04e50-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_rbac_roledefinition.md) object.</span></span>

<span data-ttu-id="04e50-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [roleDefinition](../resources/intune_rbac_roledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="04e50-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="04e50-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="04e50-126">Property</span></span>|<span data-ttu-id="04e50-127">Тип</span><span class="sxs-lookup"><span data-stu-id="04e50-127">Type</span></span>|<span data-ttu-id="04e50-128">Описание</span><span class="sxs-lookup"><span data-stu-id="04e50-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04e50-129">id</span><span class="sxs-lookup"><span data-stu-id="04e50-129">id</span></span>|<span data-ttu-id="04e50-130">String</span><span class="sxs-lookup"><span data-stu-id="04e50-130">String</span></span>|<span data-ttu-id="04e50-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="04e50-131">Key of the setting.</span></span> <span data-ttu-id="04e50-132">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="04e50-132">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="04e50-133">displayName</span><span class="sxs-lookup"><span data-stu-id="04e50-133">displayName</span></span>|<span data-ttu-id="04e50-134">String</span><span class="sxs-lookup"><span data-stu-id="04e50-134">String</span></span>|<span data-ttu-id="04e50-135">Отображаемое имя определения роли.</span><span class="sxs-lookup"><span data-stu-id="04e50-135">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="04e50-136">description</span><span class="sxs-lookup"><span data-stu-id="04e50-136">description</span></span>|<span data-ttu-id="04e50-137">String</span><span class="sxs-lookup"><span data-stu-id="04e50-137">String</span></span>|<span data-ttu-id="04e50-138">Описание определения роли.</span><span class="sxs-lookup"><span data-stu-id="04e50-138">Description of the Role definition.</span></span>|
|<span data-ttu-id="04e50-139">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="04e50-139">rolePermissions</span></span>|<span data-ttu-id="04e50-140">Коллекция [rolePermission](../resources/intune_rbac_rolepermission.md)</span><span class="sxs-lookup"><span data-stu-id="04e50-140">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="04e50-141">Список разрешений, активированных для роли.</span><span class="sxs-lookup"><span data-stu-id="04e50-141">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="04e50-142">Они должны соответствовать объекту actionName, который определен как часть rolePermission.</span><span class="sxs-lookup"><span data-stu-id="04e50-142">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="04e50-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="04e50-143">isBuiltIn</span></span>|<span data-ttu-id="04e50-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e50-144">Boolean</span></span>|<span data-ttu-id="04e50-145">Тип роли.</span><span class="sxs-lookup"><span data-stu-id="04e50-145">Type of Role.</span></span> <span data-ttu-id="04e50-146">Для встроенного определения роли задается значение True, а для настраиваемого — False.</span><span class="sxs-lookup"><span data-stu-id="04e50-146">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="04e50-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="04e50-147">Response</span></span>
<span data-ttu-id="04e50-148">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [roleDefinition](../resources/intune_rbac_roledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="04e50-148">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_rbac_roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04e50-149">Пример</span><span class="sxs-lookup"><span data-stu-id="04e50-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="04e50-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="04e50-150">Request</span></span>
<span data-ttu-id="04e50-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04e50-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 527

{
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

### <a name="response"></a><span data-ttu-id="04e50-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="04e50-152">Response</span></span>
<span data-ttu-id="04e50-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="04e50-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 629

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
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



