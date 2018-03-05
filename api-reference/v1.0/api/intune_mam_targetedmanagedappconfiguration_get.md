# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="b768e-101">Получение targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b768e-101">Get targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="b768e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b768e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b768e-103">Чтение свойств и связей объекта [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b768e-103">Read properties and relationships of [plannerPlanDetails](../resources/intune_mam_targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b768e-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b768e-104">Prerequisites</span></span>
<span data-ttu-id="b768e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b768e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b768e-107">Тип разрешений</span><span class="sxs-lookup"><span data-stu-id="b768e-107">Permission type</span></span>|<span data-ttu-id="b768e-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b768e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b768e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b768e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b768e-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b768e-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b768e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b768e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b768e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b768e-112">Not supported.</span></span>|
|<span data-ttu-id="b768e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b768e-113">Application</span></span>|<span data-ttu-id="b768e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b768e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b768e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b768e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b768e-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b768e-116">Optional query parameters</span></span>
<span data-ttu-id="b768e-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b768e-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b768e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b768e-118">Request headers</span></span>
|<span data-ttu-id="b768e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b768e-119">Header</span></span>|<span data-ttu-id="b768e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b768e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b768e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b768e-121">Authorization</span></span>|<span data-ttu-id="b768e-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b768e-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b768e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b768e-123">Accept</span></span>|<span data-ttu-id="b768e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b768e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b768e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b768e-125">Request body</span></span>
<span data-ttu-id="b768e-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b768e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b768e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b768e-127">Response</span></span>
<span data-ttu-id="b768e-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b768e-128">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/intune_mam_targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b768e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b768e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="b768e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b768e-130">Request</span></span>
<span data-ttu-id="b768e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b768e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b768e-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="b768e-132">Response</span></span>
<span data-ttu-id="b768e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b768e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 611

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "2444e029-e029-2444-29e0-442429e04424",
    "version": "Version value",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "deployedAppCount": 0,
    "isAssigned": true
  }
}
```



