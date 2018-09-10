# <a name="list-iosmanagedappregistrations"></a><span data-ttu-id="1aeb3-101">Перечисление объектов iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="1aeb3-101">List iosManagedAppRegistrations</span></span>

> <span data-ttu-id="1aeb3-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1aeb3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1aeb3-103">Список свойств и связей объектов [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md).</span><span class="sxs-lookup"><span data-stu-id="1aeb3-103">List properties and relationships of the [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1aeb3-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1aeb3-104">Prerequisites</span></span>
<span data-ttu-id="1aeb3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1aeb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1aeb3-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1aeb3-107">Permission type</span></span>|<span data-ttu-id="1aeb3-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1aeb3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1aeb3-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1aeb3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1aeb3-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1aeb3-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1aeb3-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1aeb3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1aeb3-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1aeb3-112">Not supported.</span></span>|
|<span data-ttu-id="1aeb3-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1aeb3-113">Application</span></span>|<span data-ttu-id="1aeb3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1aeb3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1aeb3-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1aeb3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="1aeb3-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1aeb3-116">Request headers</span></span>
|<span data-ttu-id="1aeb3-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1aeb3-117">Header</span></span>|<span data-ttu-id="1aeb3-118">Значение</span><span class="sxs-lookup"><span data-stu-id="1aeb3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1aeb3-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1aeb3-119">Authorization</span></span>|<span data-ttu-id="1aeb3-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="1aeb3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1aeb3-121">Принять</span><span class="sxs-lookup"><span data-stu-id="1aeb3-121">Accept</span></span>|<span data-ttu-id="1aeb3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1aeb3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1aeb3-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1aeb3-123">Request body</span></span>
<span data-ttu-id="1aeb3-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1aeb3-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1aeb3-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="1aeb3-125">Response</span></span>
<span data-ttu-id="1aeb3-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1aeb3-126">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1aeb3-127">Пример</span><span class="sxs-lookup"><span data-stu-id="1aeb3-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="1aeb3-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="1aeb3-128">Request</span></span>
<span data-ttu-id="1aeb3-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1aeb3-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="1aeb3-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="1aeb3-130">Response</span></span>
<span data-ttu-id="1aeb3-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1aeb3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 852

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "applicationVersion": "Application Version value",
      "managementSdkVersion": "Management Sdk Version value",
      "platformVersion": "Platform Version value",
      "deviceType": "Device Type value",
      "deviceTag": "Device Tag value",
      "deviceName": "Device Name value",
      "flaggedReasons": [
        "rootedDevice"
      ],
      "userId": "User Id value",
      "appIdentifier": {
        "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
        "bundleId": "Bundle Id value"
      },
      "id": "47632c19-2c19-4763-192c-6347192c6347",
      "version": "Version value"
    }
  ]
}
```








