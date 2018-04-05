# <a name="list-iosmobileappconfigurations"></a><span data-ttu-id="7fa90-101">Список iosMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="7fa90-101">List iosMobileAppConfigurations</span></span>

> <span data-ttu-id="7fa90-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7fa90-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7fa90-103">Список свойств и связей объектов [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7fa90-103">List properties and relationships of the [managedMobileApp](../resources/intune_apps_iosmobileappconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7fa90-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7fa90-104">Prerequisites</span></span>
<span data-ttu-id="7fa90-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7fa90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7fa90-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fa90-107">Permission type</span></span>|<span data-ttu-id="7fa90-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fa90-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7fa90-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fa90-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7fa90-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7fa90-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7fa90-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fa90-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7fa90-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fa90-112">Not supported.</span></span>|
|<span data-ttu-id="7fa90-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7fa90-113">Application</span></span>|<span data-ttu-id="7fa90-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fa90-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fa90-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fa90-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7fa90-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7fa90-116">Request headers</span></span>
|<span data-ttu-id="7fa90-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7fa90-117">Header</span></span>|<span data-ttu-id="7fa90-118">Значение</span><span class="sxs-lookup"><span data-stu-id="7fa90-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7fa90-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fa90-119">Authorization</span></span>|<span data-ttu-id="7fa90-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7fa90-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7fa90-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7fa90-121">Accept</span></span>|<span data-ttu-id="7fa90-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7fa90-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7fa90-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7fa90-123">Request body</span></span>
<span data-ttu-id="7fa90-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7fa90-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7fa90-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="7fa90-125">Response</span></span>
<span data-ttu-id="7fa90-126">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [iosMobileAppConfiguration](../resources/intune_apps_iosmobileappconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7fa90-126">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/intune_apps_iosmobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fa90-127">Пример</span><span class="sxs-lookup"><span data-stu-id="7fa90-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="7fa90-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fa90-128">Request</span></span>
<span data-ttu-id="7fa90-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fa90-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="7fa90-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7fa90-130">Response</span></span>
<span data-ttu-id="7fa90-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7fa90-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 815

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
      "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
      "targetedMobileApps": [
        "Targeted Mobile Apps value"
      ],
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
      "settings": [
        {
          "@odata.type": "microsoft.graph.appConfigurationSettingItem",
          "appConfigKey": "App Config Key value",
          "appConfigKeyType": "integerType",
          "appConfigKeyValue": "App Config Key Value value"
        }
      ]
    }
  ]
}
```



