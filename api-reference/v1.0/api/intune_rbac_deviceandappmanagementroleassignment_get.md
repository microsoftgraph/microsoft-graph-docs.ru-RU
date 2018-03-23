# <a name="get-deviceandappmanagementroleassignment"></a><span data-ttu-id="bf19c-101">Получение объекта deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="bf19c-101">Get deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="bf19c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bf19c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf19c-103">Чтение свойств и связей объекта [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bf19c-103">Read properties and relationships of [plannerProgressTaskBoardTaskFormat](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bf19c-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bf19c-104">Prerequisites</span></span>
<span data-ttu-id="bf19c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bf19c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bf19c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf19c-107">Permission type</span></span>|<span data-ttu-id="bf19c-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf19c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf19c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf19c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bf19c-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf19c-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="bf19c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf19c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf19c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf19c-112">Not supported.</span></span>|
|<span data-ttu-id="bf19c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf19c-113">Application</span></span>|<span data-ttu-id="bf19c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf19c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf19c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf19c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bf19c-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bf19c-116">Optional query parameters</span></span>
<span data-ttu-id="bf19c-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bf19c-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bf19c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf19c-118">Request headers</span></span>
|<span data-ttu-id="bf19c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf19c-119">Header</span></span>|<span data-ttu-id="bf19c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="bf19c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf19c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf19c-121">Authorization</span></span>|<span data-ttu-id="bf19c-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf19c-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bf19c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bf19c-123">Accept</span></span>|<span data-ttu-id="bf19c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bf19c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf19c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf19c-125">Request body</span></span>
<span data-ttu-id="bf19c-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf19c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf19c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf19c-127">Response</span></span>
<span data-ttu-id="bf19c-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bf19c-128">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf19c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="bf19c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="bf19c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf19c-130">Request</span></span>
<span data-ttu-id="bf19c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf19c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="bf19c-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="bf19c-132">Response</span></span>
<span data-ttu-id="bf19c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bf19c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
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
}
```



