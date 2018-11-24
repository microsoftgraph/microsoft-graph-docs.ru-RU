# <a name="list-appledevicefeaturesconfigurationbases"></a><span data-ttu-id="b8410-101">Перечисление объектов appleDeviceFeaturesConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="b8410-101">List appleDeviceFeaturesConfigurationBases</span></span>

> <span data-ttu-id="b8410-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b8410-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8410-103">Список свойств и связей объектов [appleDeviceFeaturesConfigurationBase](../resources/intune_deviceconfig_appledevicefeaturesconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="b8410-103">List properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/intune_deviceconfig_appledevicefeaturesconfigurationbase.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b8410-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b8410-104">Prerequisites</span></span>
<span data-ttu-id="b8410-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b8410-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b8410-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8410-107">Permission type</span></span>|<span data-ttu-id="b8410-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8410-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8410-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8410-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b8410-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8410-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b8410-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8410-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8410-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8410-112">Not supported.</span></span>|
|<span data-ttu-id="b8410-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8410-113">Application</span></span>|<span data-ttu-id="b8410-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8410-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8410-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8410-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b8410-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8410-116">Request headers</span></span>
|<span data-ttu-id="b8410-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8410-117">Header</span></span>|<span data-ttu-id="b8410-118">Значение</span><span class="sxs-lookup"><span data-stu-id="b8410-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8410-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8410-119">Authorization</span></span>|<span data-ttu-id="b8410-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8410-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8410-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b8410-121">Accept</span></span>|<span data-ttu-id="b8410-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b8410-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8410-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8410-123">Request body</span></span>
<span data-ttu-id="b8410-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b8410-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8410-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8410-125">Response</span></span>
<span data-ttu-id="b8410-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [appleDeviceFeaturesConfigurationBase](../resources/intune_deviceconfig_appledevicefeaturesconfigurationbase.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b8410-126">If successful, this method returns a `200 OK` response code and a collection of [appleDeviceFeaturesConfigurationBase](../resources/intune_deviceconfig_appledevicefeaturesconfigurationbase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8410-127">Пример</span><span class="sxs-lookup"><span data-stu-id="b8410-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8410-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8410-128">Request</span></span>
<span data-ttu-id="b8410-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8410-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="b8410-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b8410-130">Response</span></span>
<span data-ttu-id="b8410-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b8410-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 407

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appleDeviceFeaturesConfigurationBase",
      "id": "ca0bb5ff-b5ff-ca0b-ffb5-0bcaffb50bca",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```



