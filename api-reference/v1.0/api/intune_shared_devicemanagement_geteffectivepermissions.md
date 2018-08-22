# <a name="geteffectivepermissions-function"></a><span data-ttu-id="adc31-101">Функция getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="adc31-101">getEffectivePermissions function</span></span>

> <span data-ttu-id="adc31-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="adc31-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="adc31-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="adc31-103">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="adc31-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="adc31-104">Prerequisites</span></span>
<span data-ttu-id="adc31-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="adc31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="adc31-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="adc31-107">Permission type</span></span>|<span data-ttu-id="adc31-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="adc31-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adc31-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="adc31-109">Delegated (work or school account)</span></span>|<span data-ttu-id="adc31-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="adc31-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="adc31-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="adc31-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adc31-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adc31-112">Not supported.</span></span>|
|<span data-ttu-id="adc31-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="adc31-113">Application</span></span>|<span data-ttu-id="adc31-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adc31-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="adc31-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="adc31-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="adc31-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="adc31-116">Request headers</span></span>
|<span data-ttu-id="adc31-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="adc31-117">Header</span></span>|<span data-ttu-id="adc31-118">Значение</span><span class="sxs-lookup"><span data-stu-id="adc31-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adc31-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="adc31-119">Authorization</span></span>|<span data-ttu-id="adc31-120">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="adc31-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adc31-121">Accept</span><span class="sxs-lookup"><span data-stu-id="adc31-121">Accept</span></span>|<span data-ttu-id="adc31-122">application/json</span><span class="sxs-lookup"><span data-stu-id="adc31-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adc31-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="adc31-123">Request body</span></span>
<span data-ttu-id="adc31-124">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="adc31-124">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="adc31-125">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="adc31-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="adc31-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="adc31-126">Property</span></span>|<span data-ttu-id="adc31-127">Тип</span><span class="sxs-lookup"><span data-stu-id="adc31-127">Type</span></span>|<span data-ttu-id="adc31-128">Описание</span><span class="sxs-lookup"><span data-stu-id="adc31-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adc31-129">scope</span><span class="sxs-lookup"><span data-stu-id="adc31-129">scope</span></span>|<span data-ttu-id="adc31-130">String</span><span class="sxs-lookup"><span data-stu-id="adc31-130">String</span></span>|<span data-ttu-id="adc31-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="adc31-131">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="adc31-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="adc31-132">Response</span></span>
<span data-ttu-id="adc31-133">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [rolePermission](../resources/intune_rbac_rolepermission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="adc31-133">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune_rbac_rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adc31-134">Пример</span><span class="sxs-lookup"><span data-stu-id="adc31-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="adc31-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="adc31-135">Request</span></span>
<span data-ttu-id="adc31-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adc31-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="adc31-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="adc31-137">Response</span></span>
<span data-ttu-id="adc31-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="adc31-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



