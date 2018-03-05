# <a name="get-userinstallstatesummary"></a><span data-ttu-id="4099d-101">Get userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="4099d-101">Get userInstallStateSummary</span></span>

> <span data-ttu-id="4099d-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4099d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4099d-103">Чтение свойств и связей объекта [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="4099d-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_books_userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4099d-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4099d-104">Prerequisites</span></span>
<span data-ttu-id="4099d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4099d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4099d-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4099d-107">Permission type</span></span>|<span data-ttu-id="4099d-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4099d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4099d-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4099d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4099d-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4099d-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4099d-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4099d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4099d-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4099d-112">Not supported.</span></span>|
|<span data-ttu-id="4099d-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4099d-113">Application</span></span>|<span data-ttu-id="4099d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4099d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4099d-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4099d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4099d-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4099d-116">Optional query parameters</span></span>
<span data-ttu-id="4099d-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4099d-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/ru-RU/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4099d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4099d-118">Request headers</span></span>
|<span data-ttu-id="4099d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4099d-119">Header</span></span>|<span data-ttu-id="4099d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4099d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4099d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4099d-121">Authorization</span></span>|<span data-ttu-id="4099d-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4099d-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4099d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4099d-123">Accept</span></span>|<span data-ttu-id="4099d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4099d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4099d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4099d-125">Request body</span></span>
<span data-ttu-id="4099d-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4099d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4099d-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="4099d-127">Response</span></span>
<span data-ttu-id="4099d-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4099d-128">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/intune_books_userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4099d-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4099d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="4099d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4099d-130">Request</span></span>
<span data-ttu-id="4099d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4099d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="4099d-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="4099d-132">Response</span></span>
<span data-ttu-id="4099d-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4099d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "value": {
    "@odata.type": "#microsoft.graph.userInstallStateSummary",
    "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
    "userName": "User Name value",
    "installedDeviceCount": 4,
    "failedDeviceCount": 1,
    "notInstalledDeviceCount": 7
  }
}
```



