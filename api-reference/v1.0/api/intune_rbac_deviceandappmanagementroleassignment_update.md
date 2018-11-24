# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="4b14c-101">Обновление объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4b14c-101">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="4b14c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4b14c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b14c-103">Обновление свойств объекта [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4b14c-103">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4b14c-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4b14c-104">Prerequisites</span></span>
<span data-ttu-id="4b14c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4b14c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4b14c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b14c-107">Permission type</span></span>|<span data-ttu-id="4b14c-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b14c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b14c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b14c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4b14c-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b14c-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="4b14c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b14c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b14c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b14c-112">Not supported.</span></span>|
|<span data-ttu-id="4b14c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b14c-113">Application</span></span>|<span data-ttu-id="4b14c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b14c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b14c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b14c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="4b14c-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b14c-116">Request headers</span></span>
|<span data-ttu-id="4b14c-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b14c-117">Header</span></span>|<span data-ttu-id="4b14c-118">Значение</span><span class="sxs-lookup"><span data-stu-id="4b14c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b14c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b14c-119">Authorization</span></span>|<span data-ttu-id="4b14c-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b14c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b14c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4b14c-121">Accept</span></span>|<span data-ttu-id="4b14c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4b14c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b14c-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4b14c-123">Request body</span></span>
<span data-ttu-id="4b14c-124">В теле запроса добавьте представление объекта [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b14c-124">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="4b14c-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4b14c-125">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="4b14c-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b14c-126">Property</span></span>|<span data-ttu-id="4b14c-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4b14c-127">Type</span></span>|<span data-ttu-id="4b14c-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4b14c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b14c-129">id</span><span class="sxs-lookup"><span data-stu-id="4b14c-129">id</span></span>|<span data-ttu-id="4b14c-130">String</span><span class="sxs-lookup"><span data-stu-id="4b14c-130">String</span></span>|<span data-ttu-id="4b14c-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4b14c-131">Key of the entity.</span></span> <span data-ttu-id="4b14c-132">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="4b14c-132">This is read-only and automatically generated.</span></span> <span data-ttu-id="4b14c-133">Наследуется от объекта [roleAssignment](../resources/intune_rbac_roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4b14c-133">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="4b14c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="4b14c-134">displayName</span></span>|<span data-ttu-id="4b14c-135">String</span><span class="sxs-lookup"><span data-stu-id="4b14c-135">String</span></span>|<span data-ttu-id="4b14c-136">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="4b14c-136">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="4b14c-137">Наследуется от объекта [roleAssignment](../resources/intune_rbac_roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4b14c-137">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="4b14c-138">description</span><span class="sxs-lookup"><span data-stu-id="4b14c-138">description</span></span>|<span data-ttu-id="4b14c-139">String</span><span class="sxs-lookup"><span data-stu-id="4b14c-139">String</span></span>|<span data-ttu-id="4b14c-140">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="4b14c-140">Description of the Role Assignment.</span></span> <span data-ttu-id="4b14c-141">Наследуется от объекта [roleAssignment](../resources/intune_rbac_roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4b14c-141">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="4b14c-142">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="4b14c-142">resourceScopes</span></span>|<span data-ttu-id="4b14c-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b14c-143">String collection</span></span>|<span data-ttu-id="4b14c-144">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="4b14c-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="4b14c-145">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4b14c-145">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="4b14c-146">Наследуется от объекта [roleAssignment](../resources/intune_rbac_roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4b14c-146">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="4b14c-147">members</span><span class="sxs-lookup"><span data-stu-id="4b14c-147">members</span></span>|<span data-ttu-id="4b14c-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b14c-148">String collection</span></span>|<span data-ttu-id="4b14c-149">Список идентификаторов групп безопасности с элементами ролей.</span><span class="sxs-lookup"><span data-stu-id="4b14c-149">The list of ids of role member security groups.</span></span> <span data-ttu-id="4b14c-150">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4b14c-150">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="4b14c-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b14c-151">Response</span></span>
<span data-ttu-id="4b14c-152">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4b14c-152">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b14c-153">Пример</span><span class="sxs-lookup"><span data-stu-id="4b14c-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="4b14c-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b14c-154">Request</span></span>
<span data-ttu-id="4b14c-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b14c-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="4b14c-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b14c-156">Response</span></span>
<span data-ttu-id="4b14c-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4b14c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```



