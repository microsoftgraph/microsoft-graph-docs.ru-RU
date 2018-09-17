# <a name="create-roleassignment"></a><span data-ttu-id="b67c5-101">Создание объекта roleAssignment</span><span class="sxs-lookup"><span data-stu-id="b67c5-101">Create roleAssignment</span></span>

> <span data-ttu-id="b67c5-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b67c5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b67c5-103">Создание объекта [roleAssignment](../resources/intune_rbac_roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b67c5-103">Create a new [roleAssignment](../resources/intune_rbac_roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b67c5-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b67c5-104">Prerequisites</span></span>
<span data-ttu-id="b67c5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b67c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b67c5-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b67c5-107">Permission type</span></span>|<span data-ttu-id="b67c5-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b67c5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b67c5-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b67c5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b67c5-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b67c5-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b67c5-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b67c5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b67c5-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b67c5-112">Not supported.</span></span>|
|<span data-ttu-id="b67c5-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b67c5-113">Application</span></span>|<span data-ttu-id="b67c5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b67c5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b67c5-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b67c5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="b67c5-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b67c5-116">Request headers</span></span>
|<span data-ttu-id="b67c5-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b67c5-117">Header</span></span>|<span data-ttu-id="b67c5-118">Значение</span><span class="sxs-lookup"><span data-stu-id="b67c5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b67c5-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b67c5-119">Authorization</span></span>|<span data-ttu-id="b67c5-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="b67c5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b67c5-121">Принять</span><span class="sxs-lookup"><span data-stu-id="b67c5-121">Accept</span></span>|<span data-ttu-id="b67c5-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="b67c5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b67c5-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b67c5-123">Request body</span></span>
<span data-ttu-id="b67c5-124">В теле запроса добавьте представление объекта roleAssignment в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b67c5-124">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="b67c5-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="b67c5-125">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="b67c5-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="b67c5-126">Property</span></span>|<span data-ttu-id="b67c5-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b67c5-127">Type</span></span>|<span data-ttu-id="b67c5-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b67c5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b67c5-129">ИД</span><span class="sxs-lookup"><span data-stu-id="b67c5-129">id</span></span>|<span data-ttu-id="b67c5-130">Строка</span><span class="sxs-lookup"><span data-stu-id="b67c5-130">String</span></span>|<span data-ttu-id="b67c5-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b67c5-131">Key of the entity.</span></span> <span data-ttu-id="b67c5-132">Это свойство доступно только для чтения и создается автоматически.</span><span class="sxs-lookup"><span data-stu-id="b67c5-132">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="b67c5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b67c5-133">displayName</span></span>|<span data-ttu-id="b67c5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b67c5-134">String</span></span>|<span data-ttu-id="b67c5-135">Отображаемое или понятное имя назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b67c5-135">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="b67c5-136">описание</span><span class="sxs-lookup"><span data-stu-id="b67c5-136">description</span></span>|<span data-ttu-id="b67c5-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b67c5-137">String</span></span>|<span data-ttu-id="b67c5-138">Описание назначения роли.</span><span class="sxs-lookup"><span data-stu-id="b67c5-138">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="b67c5-139">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="b67c5-139">resourceScopes</span></span>|<span data-ttu-id="b67c5-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b67c5-140">String collection</span></span>|<span data-ttu-id="b67c5-141">Список идентификаторов групп безопасности с элементами области применения ролей.</span><span class="sxs-lookup"><span data-stu-id="b67c5-141">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="b67c5-142">Эти идентификаторы берутся из Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b67c5-142">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="b67c5-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b67c5-143">Response</span></span>
<span data-ttu-id="b67c5-144">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [roleAssignment](../resources/intune_rbac_roleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b67c5-144">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune_rbac_roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b67c5-145">Пример</span><span class="sxs-lookup"><span data-stu-id="b67c5-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="b67c5-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="b67c5-146">Request</span></span>
<span data-ttu-id="b67c5-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b67c5-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b67c5-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="b67c5-148">Response</span></span>
<span data-ttu-id="b67c5-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b67c5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








