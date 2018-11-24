# <a name="get-softwareupdatestatussummary"></a><span data-ttu-id="71807-101">Получение объекта softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="71807-101">Get softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="71807-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="71807-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71807-103">Чтение свойств и связей объекта [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="71807-103">Read properties and relationships of the [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="71807-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="71807-104">Prerequisites</span></span>
<span data-ttu-id="71807-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="71807-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="71807-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71807-107">Permission type</span></span>|<span data-ttu-id="71807-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="71807-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71807-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71807-109">Delegated (work or school account)</span></span>|<span data-ttu-id="71807-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="71807-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="71807-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71807-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71807-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71807-112">Not supported.</span></span>|
|<span data-ttu-id="71807-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71807-113">Application</span></span>|<span data-ttu-id="71807-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71807-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71807-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71807-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/softwareUpdateStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="71807-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="71807-116">Optional query parameters</span></span>
<span data-ttu-id="71807-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="71807-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="71807-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71807-118">Request headers</span></span>
|<span data-ttu-id="71807-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71807-119">Header</span></span>|<span data-ttu-id="71807-120">Значение</span><span class="sxs-lookup"><span data-stu-id="71807-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71807-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="71807-121">Authorization</span></span>|<span data-ttu-id="71807-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71807-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71807-123">Accept</span><span class="sxs-lookup"><span data-stu-id="71807-123">Accept</span></span>|<span data-ttu-id="71807-124">application/json</span><span class="sxs-lookup"><span data-stu-id="71807-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71807-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71807-125">Request body</span></span>
<span data-ttu-id="71807-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71807-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71807-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="71807-127">Response</span></span>
<span data-ttu-id="71807-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71807-128">If successful, this method returns a `200 OK` response code and [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71807-129">Пример</span><span class="sxs-lookup"><span data-stu-id="71807-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="71807-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="71807-130">Request</span></span>
<span data-ttu-id="71807-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71807-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
```

### <a name="response"></a><span data-ttu-id="71807-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="71807-132">Response</span></span>
<span data-ttu-id="71807-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="71807-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 620

{
  "value": {
    "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
    "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
    "displayName": "Display Name value",
    "compliantDeviceCount": 4,
    "nonCompliantDeviceCount": 7,
    "remediatedDeviceCount": 5,
    "errorDeviceCount": 0,
    "unknownDeviceCount": 2,
    "conflictDeviceCount": 3,
    "notApplicableDeviceCount": 8,
    "compliantUserCount": 2,
    "nonCompliantUserCount": 5,
    "remediatedUserCount": 3,
    "errorUserCount": 14,
    "unknownUserCount": 0,
    "conflictUserCount": 1,
    "notApplicableUserCount": 6
  }
}
```



