# <a name="get-manageddevicemobileappconfiguration"></a><span data-ttu-id="e111c-101">Получение объекта managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e111c-101">Get managedDeviceMobileAppConfiguration</span></span>

> <span data-ttu-id="e111c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e111c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e111c-103">Чтение свойств и связей объекта [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e111c-103">Read properties and relationships of [plannerProgressTaskBoardTaskFormat](../resources/intune_apps_manageddevicemobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e111c-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e111c-104">Prerequisites</span></span>
<span data-ttu-id="e111c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e111c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e111c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e111c-107">Permission type</span></span>|<span data-ttu-id="e111c-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e111c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e111c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e111c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e111c-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e111c-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e111c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e111c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e111c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e111c-112">Not supported.</span></span>|
|<span data-ttu-id="e111c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e111c-113">Application</span></span>|<span data-ttu-id="e111c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e111c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e111c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e111c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e111c-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e111c-116">Optional query parameters</span></span>
<span data-ttu-id="e111c-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e111c-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e111c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e111c-118">Request headers</span></span>
|<span data-ttu-id="e111c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e111c-119">Header</span></span>|<span data-ttu-id="e111c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e111c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e111c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e111c-121">Authorization</span></span>|<span data-ttu-id="e111c-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e111c-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e111c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e111c-123">Accept</span></span>|<span data-ttu-id="e111c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e111c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e111c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e111c-125">Request body</span></span>
<span data-ttu-id="e111c-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e111c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e111c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e111c-127">Response</span></span>
<span data-ttu-id="e111c-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e111c-128">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/intune_apps_manageddevicemobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e111c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="e111c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="e111c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e111c-130">Request</span></span>
<span data-ttu-id="e111c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e111c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e111c-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="e111c-132">Response</span></span>
<span data-ttu-id="e111c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e111c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 451

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
    "id": "c60e7591-7591-c60e-9175-0ec691750ec6",
    "targetedMobileApps": [
      "Targeted Mobile Apps value"
    ],
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7
  }
}
```



