# <a name="geteffectivepermissions-function"></a><span data-ttu-id="8c838-101">Функция getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="8c838-101">getEffectivePermissions function</span></span>

> <span data-ttu-id="8c838-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8c838-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c838-103">Получает действующие разрешения пользователя, прошедшего проверку подлинности</span><span class="sxs-lookup"><span data-stu-id="8c838-103">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c838-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8c838-104">Prerequisites</span></span>
<span data-ttu-id="8c838-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8c838-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8c838-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c838-107">Permission type</span></span>|<span data-ttu-id="8c838-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c838-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c838-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c838-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8c838-110">&nbsp;&nbsp; Управления доступом на основе ролей</span><span class="sxs-lookup"><span data-stu-id="8c838-110">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="8c838-111">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c838-111">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="8c838-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c838-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c838-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c838-113">Not supported.</span></span>|
|<span data-ttu-id="8c838-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c838-114">Application</span></span>|<span data-ttu-id="8c838-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c838-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c838-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c838-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="8c838-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c838-117">Request headers</span></span>
|<span data-ttu-id="8c838-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c838-118">Header</span></span>|<span data-ttu-id="8c838-119">Значение</span><span class="sxs-lookup"><span data-stu-id="8c838-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c838-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c838-120">Authorization</span></span>|<span data-ttu-id="8c838-121">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8c838-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c838-122">Accept</span><span class="sxs-lookup"><span data-stu-id="8c838-122">Accept</span></span>|<span data-ttu-id="8c838-123">application/json</span><span class="sxs-lookup"><span data-stu-id="8c838-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c838-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c838-124">Request body</span></span>
<span data-ttu-id="8c838-125">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="8c838-125">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="8c838-126">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="8c838-126">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="8c838-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c838-127">Property</span></span>|<span data-ttu-id="8c838-128">Тип</span><span class="sxs-lookup"><span data-stu-id="8c838-128">Type</span></span>|<span data-ttu-id="8c838-129">Описание</span><span class="sxs-lookup"><span data-stu-id="8c838-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c838-130">scope</span><span class="sxs-lookup"><span data-stu-id="8c838-130">scope</span></span>|<span data-ttu-id="8c838-131">String</span><span class="sxs-lookup"><span data-stu-id="8c838-131">String</span></span>|<span data-ttu-id="8c838-132">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8c838-132">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="8c838-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c838-133">Response</span></span>
<span data-ttu-id="8c838-134">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [rolePermission](../resources/intune_rbac_rolepermission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8c838-134">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune_rbac_rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c838-135">Пример</span><span class="sxs-lookup"><span data-stu-id="8c838-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c838-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c838-136">Request</span></span>
<span data-ttu-id="8c838-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c838-137">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="8c838-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c838-138">Response</span></span>
<span data-ttu-id="8c838-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8c838-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "value": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
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
  ]
}
```



