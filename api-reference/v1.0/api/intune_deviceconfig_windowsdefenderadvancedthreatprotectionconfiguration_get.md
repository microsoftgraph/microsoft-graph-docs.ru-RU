# <a name="get-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="27564-101">Получение объекта windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="27564-101">Get windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="27564-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="27564-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27564-103">Чтение свойств и связей объекта [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="27564-103">Read properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="27564-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="27564-104">Prerequisites</span></span>
<span data-ttu-id="27564-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="27564-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="27564-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27564-107">Permission type</span></span>|<span data-ttu-id="27564-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="27564-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27564-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27564-109">Delegated (work or school account)</span></span>|<span data-ttu-id="27564-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="27564-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="27564-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27564-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27564-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27564-112">Not supported.</span></span>|
|<span data-ttu-id="27564-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27564-113">Application</span></span>|<span data-ttu-id="27564-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27564-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27564-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27564-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="27564-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="27564-116">Optional query parameters</span></span>
<span data-ttu-id="27564-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="27564-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="27564-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27564-118">Request headers</span></span>
|<span data-ttu-id="27564-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="27564-119">Header</span></span>|<span data-ttu-id="27564-120">Значение</span><span class="sxs-lookup"><span data-stu-id="27564-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27564-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27564-121">Authorization</span></span>|<span data-ttu-id="27564-122">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="27564-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27564-123">Принять</span><span class="sxs-lookup"><span data-stu-id="27564-123">Accept</span></span>|<span data-ttu-id="27564-124">application/json</span><span class="sxs-lookup"><span data-stu-id="27564-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27564-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27564-125">Request body</span></span>
<span data-ttu-id="27564-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="27564-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27564-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="27564-127">Response</span></span>
<span data-ttu-id="27564-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="27564-128">If successful, this method returns a `200 OK` response code and [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27564-129">Пример</span><span class="sxs-lookup"><span data-stu-id="27564-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="27564-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="27564-130">Request</span></span>
<span data-ttu-id="27564-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27564-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="27564-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="27564-132">Response</span></span>
<span data-ttu-id="27564-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27564-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 476

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
    "id": "294373aa-73aa-2943-aa73-4329aa734329",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "allowSampleSharing": true,
    "enableExpeditedTelemetryReporting": true
  }
}
```








