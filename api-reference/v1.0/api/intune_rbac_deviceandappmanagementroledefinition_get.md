# <a name="get-deviceandappmanagementroledefinition"></a><span data-ttu-id="b1998-101">Получение deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="b1998-101">Get deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="b1998-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b1998-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1998-103">Считывание свойств и связей объекта [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="b1998-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b1998-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b1998-104">Prerequisites</span></span>
<span data-ttu-id="b1998-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b1998-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b1998-107">Тип разрешений</span><span class="sxs-lookup"><span data-stu-id="b1998-107">Permission type</span></span>|<span data-ttu-id="b1998-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1998-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1998-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1998-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b1998-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1998-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="b1998-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1998-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1998-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1998-112">Not supported.</span></span>|
|<span data-ttu-id="b1998-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1998-113">Application</span></span>|<span data-ttu-id="b1998-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1998-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1998-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1998-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b1998-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b1998-116">Optional query parameters</span></span>
<span data-ttu-id="b1998-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b1998-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b1998-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1998-118">Request headers</span></span>
|<span data-ttu-id="b1998-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1998-119">Header</span></span>|<span data-ttu-id="b1998-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b1998-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1998-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1998-121">Authorization</span></span>|<span data-ttu-id="b1998-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1998-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b1998-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b1998-123">Accept</span></span>|<span data-ttu-id="b1998-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b1998-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1998-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1998-125">Request body</span></span>
<span data-ttu-id="b1998-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1998-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1998-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1998-127">Response</span></span>
<span data-ttu-id="b1998-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b1998-128">If successful, this method returns a `200 OK` response code and [Contract](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1998-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b1998-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="b1998-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1998-130">Request</span></span>
<span data-ttu-id="b1998-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1998-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="b1998-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1998-132">Response</span></span>
<span data-ttu-id="b1998-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b1998-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 712

{
  "value": {
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
}
```



