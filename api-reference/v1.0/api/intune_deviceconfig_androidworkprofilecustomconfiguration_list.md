# <a name="list-androidworkprofilecustomconfigurations"></a><span data-ttu-id="73d61-101">Перечисление androidWorkProfileCustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="73d61-101">List androidWorkProfileCustomConfigurations</span></span>

> <span data-ttu-id="73d61-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="73d61-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73d61-103">Свойства списка и связей объектов [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="73d61-103">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73d61-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="73d61-104">Prerequisites</span></span>
<span data-ttu-id="73d61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="73d61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="73d61-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73d61-107">Permission type</span></span>|<span data-ttu-id="73d61-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73d61-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73d61-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73d61-109">Delegated (work or school account)</span></span>|<span data-ttu-id="73d61-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="73d61-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="73d61-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73d61-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73d61-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73d61-112">Not supported.</span></span>|
|<span data-ttu-id="73d61-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73d61-113">Application</span></span>|<span data-ttu-id="73d61-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73d61-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73d61-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73d61-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="73d61-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73d61-116">Request headers</span></span>
|<span data-ttu-id="73d61-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73d61-117">Header</span></span>|<span data-ttu-id="73d61-118">Значение</span><span class="sxs-lookup"><span data-stu-id="73d61-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73d61-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73d61-119">Authorization</span></span>|<span data-ttu-id="73d61-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="73d61-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73d61-121">Принять</span><span class="sxs-lookup"><span data-stu-id="73d61-121">Accept</span></span>|<span data-ttu-id="73d61-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="73d61-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73d61-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73d61-123">Request body</span></span>
<span data-ttu-id="73d61-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73d61-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73d61-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="73d61-125">Response</span></span>
<span data-ttu-id="73d61-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [androidWorkProfileCustomConfiguration](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="73d61-126">If successful, this method returns a `200 OK` response code and collection of [DriveItemVersion](../resources/intune_deviceconfig_androidworkprofilecustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73d61-127">Пример</span><span class="sxs-lookup"><span data-stu-id="73d61-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="73d61-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="73d61-128">Request</span></span>
<span data-ttu-id="73d61-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73d61-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="73d61-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="73d61-130">Response</span></span>
<span data-ttu-id="73d61-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73d61-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 682

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
      "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "omaSettings": [
        {
          "@odata.type": "microsoft.graph.omaSettingInteger",
          "displayName": "Display Name value",
          "description": "Description value",
          "omaUri": "Oma Uri value",
          "value": 5
        }
      ]
    }
  ]
}
```








