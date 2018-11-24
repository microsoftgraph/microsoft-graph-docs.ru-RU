# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="51483-101">Перечисление объектов deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="51483-101">List deviceAndAppManagementRoleDefinitions</span></span>

> <span data-ttu-id="51483-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="51483-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51483-103">Список свойств и связей объектов [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="51483-103">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51483-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="51483-104">Prerequisites</span></span>
<span data-ttu-id="51483-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="51483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="51483-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51483-107">Permission type</span></span>|<span data-ttu-id="51483-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51483-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51483-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51483-109">Delegated (work or school account)</span></span>|<span data-ttu-id="51483-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="51483-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="51483-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51483-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51483-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51483-112">Not supported.</span></span>|
|<span data-ttu-id="51483-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51483-113">Application</span></span>|<span data-ttu-id="51483-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51483-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51483-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51483-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="51483-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51483-116">Request headers</span></span>
|<span data-ttu-id="51483-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51483-117">Header</span></span>|<span data-ttu-id="51483-118">Значение</span><span class="sxs-lookup"><span data-stu-id="51483-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51483-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="51483-119">Authorization</span></span>|<span data-ttu-id="51483-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51483-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51483-121">Accept</span><span class="sxs-lookup"><span data-stu-id="51483-121">Accept</span></span>|<span data-ttu-id="51483-122">application/json</span><span class="sxs-lookup"><span data-stu-id="51483-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51483-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51483-123">Request body</span></span>
<span data-ttu-id="51483-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51483-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51483-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="51483-125">Response</span></span>
<span data-ttu-id="51483-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="51483-126">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51483-127">Пример</span><span class="sxs-lookup"><span data-stu-id="51483-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="51483-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="51483-128">Request</span></span>
<span data-ttu-id="51483-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51483-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="51483-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="51483-130">Response</span></span>
<span data-ttu-id="51483-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="51483-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 768

{
  "value": [
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
  ]
}
```



