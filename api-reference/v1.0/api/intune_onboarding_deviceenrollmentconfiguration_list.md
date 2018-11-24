# <a name="list-deviceenrollmentconfigurations"></a><span data-ttu-id="081fd-101">Перечисление объектов deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="081fd-101">List deviceEnrollmentConfigurations</span></span>

> <span data-ttu-id="081fd-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="081fd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="081fd-103">Список свойств и связей объектов [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="081fd-103">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="081fd-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="081fd-104">Prerequisites</span></span>
<span data-ttu-id="081fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="081fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="081fd-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="081fd-107">Permission type</span></span>|<span data-ttu-id="081fd-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="081fd-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="081fd-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="081fd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="081fd-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="081fd-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="081fd-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="081fd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="081fd-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="081fd-112">Not supported.</span></span>|
|<span data-ttu-id="081fd-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="081fd-113">Application</span></span>|<span data-ttu-id="081fd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="081fd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="081fd-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="081fd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="081fd-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="081fd-116">Request headers</span></span>
|<span data-ttu-id="081fd-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="081fd-117">Header</span></span>|<span data-ttu-id="081fd-118">Значение</span><span class="sxs-lookup"><span data-stu-id="081fd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="081fd-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="081fd-119">Authorization</span></span>|<span data-ttu-id="081fd-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="081fd-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="081fd-121">Accept</span><span class="sxs-lookup"><span data-stu-id="081fd-121">Accept</span></span>|<span data-ttu-id="081fd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="081fd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="081fd-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="081fd-123">Request body</span></span>
<span data-ttu-id="081fd-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="081fd-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="081fd-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="081fd-125">Response</span></span>
<span data-ttu-id="081fd-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="081fd-126">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="081fd-127">Пример</span><span class="sxs-lookup"><span data-stu-id="081fd-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="081fd-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="081fd-128">Request</span></span>
<span data-ttu-id="081fd-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="081fd-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="081fd-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="081fd-130">Response</span></span>
<span data-ttu-id="081fd-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="081fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
      "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7
    }
  ]
}
```



