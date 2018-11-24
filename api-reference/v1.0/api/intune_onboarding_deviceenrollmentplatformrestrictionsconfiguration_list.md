# <a name="list-deviceenrollmentplatformrestrictionsconfigurations"></a><span data-ttu-id="64931-101">Перечисление объектов deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="64931-101">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>

> <span data-ttu-id="64931-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="64931-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64931-103">Список свойств и связей объектов [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64931-103">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="64931-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="64931-104">Prerequisites</span></span>
<span data-ttu-id="64931-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="64931-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="64931-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64931-107">Permission type</span></span>|<span data-ttu-id="64931-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64931-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64931-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64931-109">Delegated (work or school account)</span></span>|<span data-ttu-id="64931-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="64931-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="64931-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64931-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64931-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64931-112">Not supported.</span></span>|
|<span data-ttu-id="64931-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64931-113">Application</span></span>|<span data-ttu-id="64931-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64931-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64931-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64931-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="64931-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64931-116">Request headers</span></span>
|<span data-ttu-id="64931-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64931-117">Header</span></span>|<span data-ttu-id="64931-118">Значение</span><span class="sxs-lookup"><span data-stu-id="64931-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64931-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="64931-119">Authorization</span></span>|<span data-ttu-id="64931-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64931-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64931-121">Accept</span><span class="sxs-lookup"><span data-stu-id="64931-121">Accept</span></span>|<span data-ttu-id="64931-122">application/json</span><span class="sxs-lookup"><span data-stu-id="64931-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64931-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64931-123">Request body</span></span>
<span data-ttu-id="64931-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64931-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64931-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="64931-125">Response</span></span>
<span data-ttu-id="64931-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="64931-126">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64931-127">Пример</span><span class="sxs-lookup"><span data-stu-id="64931-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="64931-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="64931-128">Request</span></span>
<span data-ttu-id="64931-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64931-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="64931-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="64931-130">Response</span></span>
<span data-ttu-id="64931-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="64931-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2027

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
      "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "iosRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "windowsRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "windowsMobileRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "androidRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "macOSRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      }
    }
  ]
}
```



