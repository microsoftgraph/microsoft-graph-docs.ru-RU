# <a name="update-roleassignment"></a><span data-ttu-id="9cd5b-101">Обновление объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="9cd5b-101">Update roleAssignment</span></span>

> <span data-ttu-id="9cd5b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9cd5b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9cd5b-103">Обновление свойств объекта [roleAssignment](../resources/intune_rbac_roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9cd5b-103">Update the properties of a [roleAssignment](../resources/intune_rbac_roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9cd5b-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9cd5b-104">Prerequisites</span></span>
<span data-ttu-id="9cd5b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9cd5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9cd5b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9cd5b-107">Permission type</span></span>|<span data-ttu-id="9cd5b-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9cd5b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cd5b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9cd5b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9cd5b-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cd5b-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="9cd5b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9cd5b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cd5b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cd5b-112">Not supported.</span></span>|
|<span data-ttu-id="9cd5b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9cd5b-113">Application</span></span>|<span data-ttu-id="9cd5b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cd5b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cd5b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9cd5b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9cd5b-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9cd5b-116">Request headers</span></span>
|<span data-ttu-id="9cd5b-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9cd5b-117">Header</span></span>|<span data-ttu-id="9cd5b-118">Значение</span><span class="sxs-lookup"><span data-stu-id="9cd5b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cd5b-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9cd5b-119">Authorization</span></span>|<span data-ttu-id="9cd5b-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="9cd5b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cd5b-121">Принять</span><span class="sxs-lookup"><span data-stu-id="9cd5b-121">Accept</span></span>|<span data-ttu-id="9cd5b-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="9cd5b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cd5b-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9cd5b-123">Request body</span></span>
<span data-ttu-id="9cd5b-124">В теле запроса добавьте представление объекта [roleAssignment](../resources/intune_rbac_roleassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9cd5b-124">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune_rbac_roleassignment.md) object.</span></span>

<span data-ttu-id="9cd5b-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [roleAssignment](../resources/intune_rbac_roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9cd5b-125">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune_rbac_roleassignment.md).</span></span>

|<span data-ttu-id="9cd5b-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="9cd5b-126">Property</span></span>|<span data-ttu-id="9cd5b-127">Тип</span><span class="sxs-lookup"><span data-stu-id="9cd5b-127">Type</span></span>|<span data-ttu-id="9cd5b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="9cd5b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cd5b-129">ИД</span><span class="sxs-lookup"><span data-stu-id="9cd5b-129">id</span></span>|<span data-ttu-id="9cd5b-130">Строка</span><span class="sxs-lookup"><span data-stu-id="9cd5b-130">String</span></span>|<span data-ttu-id="9cd5b-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9cd5b-131">Key of the entity.</span></span> <span data-ttu-id="9cd5b-132">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="9cd5b-132">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="9cd5b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9cd5b-133">displayName</span></span>|<span data-ttu-id="9cd5b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9cd5b-134">String</span></span>|<span data-ttu-id="9cd5b-135">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="9cd5b-135">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="9cd5b-136">описание</span><span class="sxs-lookup"><span data-stu-id="9cd5b-136">description</span></span>|<span data-ttu-id="9cd5b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="9cd5b-137">String</span></span>|<span data-ttu-id="9cd5b-138">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="9cd5b-138">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="9cd5b-139">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="9cd5b-139">resourceScopes</span></span>|<span data-ttu-id="9cd5b-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9cd5b-140">String collection</span></span>|<span data-ttu-id="9cd5b-141">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="9cd5b-141">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="9cd5b-142">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9cd5b-142">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="9cd5b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cd5b-143">Response</span></span>
<span data-ttu-id="9cd5b-144">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [roleAssignment](../resources/intune_rbac_roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9cd5b-144">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune_rbac_roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cd5b-145">Пример</span><span class="sxs-lookup"><span data-stu-id="9cd5b-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="9cd5b-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="9cd5b-146">Request</span></span>
<span data-ttu-id="9cd5b-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9cd5b-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
Content-type: application/json
Content-length: 140

{
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="9cd5b-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="9cd5b-148">Response</span></span>
<span data-ttu-id="9cd5b-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9cd5b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```








