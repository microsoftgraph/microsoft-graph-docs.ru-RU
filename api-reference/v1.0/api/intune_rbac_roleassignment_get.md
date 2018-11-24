# <a name="get-roleassignment"></a><span data-ttu-id="a4b46-101">Get roleAssignment</span><span class="sxs-lookup"><span data-stu-id="a4b46-101">Get roleAssignment</span></span>

> <span data-ttu-id="a4b46-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a4b46-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4b46-103">Чтение свойств и связей объекта [roleAssignment](../resources/intune_rbac_roleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a4b46-103">Read properties and relationships of the [roleAssignment](../resources/intune_rbac_roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a4b46-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a4b46-104">Prerequisites</span></span>
<span data-ttu-id="a4b46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a4b46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a4b46-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4b46-107">Permission type</span></span>|<span data-ttu-id="a4b46-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4b46-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4b46-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4b46-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a4b46-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4b46-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="a4b46-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4b46-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4b46-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4b46-112">Not supported.</span></span>|
|<span data-ttu-id="a4b46-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4b46-113">Application</span></span>|<span data-ttu-id="a4b46-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4b46-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4b46-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4b46-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4b46-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a4b46-116">Optional query parameters</span></span>
<span data-ttu-id="a4b46-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a4b46-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a4b46-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4b46-118">Request headers</span></span>
|<span data-ttu-id="a4b46-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4b46-119">Header</span></span>|<span data-ttu-id="a4b46-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a4b46-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4b46-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4b46-121">Authorization</span></span>|<span data-ttu-id="a4b46-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4b46-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4b46-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a4b46-123">Accept</span></span>|<span data-ttu-id="a4b46-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a4b46-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4b46-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4b46-125">Request body</span></span>
<span data-ttu-id="a4b46-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a4b46-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4b46-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="a4b46-127">Response</span></span>
<span data-ttu-id="a4b46-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [roleAssignment](../resources/intune_rbac_roleassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a4b46-128">If successful, this method returns a `200 OK` response code and [roleAssignment](../resources/intune_rbac_roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4b46-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a4b46-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="a4b46-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4b46-130">Request</span></span>
<span data-ttu-id="a4b46-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4b46-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="a4b46-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="a4b46-132">Response</span></span>
<span data-ttu-id="a4b46-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a4b46-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "value": {
    "@odata.type": "#microsoft.graph.roleAssignment",
    "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
    "displayName": "Display Name value",
    "description": "Description value",
    "resourceScopes": [
      "Resource Scopes value"
    ]
  }
}
```



