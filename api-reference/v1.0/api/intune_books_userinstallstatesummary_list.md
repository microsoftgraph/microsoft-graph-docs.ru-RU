# <a name="list-userinstallstatesummaries"></a><span data-ttu-id="4ba45-101">Перечисление объектов userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="4ba45-101">List userInstallStateSummaries</span></span>

> <span data-ttu-id="4ba45-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4ba45-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ba45-103">Список свойств и связей объектов [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="4ba45-103">List properties and relationships of the [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ba45-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4ba45-104">Prerequisites</span></span>
<span data-ttu-id="4ba45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4ba45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4ba45-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ba45-107">Permission type</span></span>|<span data-ttu-id="4ba45-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ba45-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ba45-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ba45-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4ba45-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4ba45-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4ba45-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ba45-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ba45-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ba45-112">Not supported.</span></span>|
|<span data-ttu-id="4ba45-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ba45-113">Application</span></span>|<span data-ttu-id="4ba45-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ba45-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ba45-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ba45-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="4ba45-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ba45-116">Request headers</span></span>
|<span data-ttu-id="4ba45-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4ba45-117">Header</span></span>|<span data-ttu-id="4ba45-118">Значение</span><span class="sxs-lookup"><span data-stu-id="4ba45-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ba45-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ba45-119">Authorization</span></span>|<span data-ttu-id="4ba45-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ba45-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4ba45-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4ba45-121">Accept</span></span>|<span data-ttu-id="4ba45-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4ba45-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ba45-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ba45-123">Request body</span></span>
<span data-ttu-id="4ba45-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4ba45-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ba45-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ba45-125">Response</span></span>
<span data-ttu-id="4ba45-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4ba45-126">If successful, this method returns a `200 OK` response code and collection of [workbookRangeView](../resources/intune_books_userinstallstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ba45-127">Пример</span><span class="sxs-lookup"><span data-stu-id="4ba45-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ba45-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ba45-128">Request</span></span>
<span data-ttu-id="4ba45-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4ba45-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

### <a name="response"></a><span data-ttu-id="4ba45-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ba45-130">Response</span></span>
<span data-ttu-id="4ba45-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4ba45-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userInstallStateSummary",
      "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
      "userName": "User Name value",
      "installedDeviceCount": 4,
      "failedDeviceCount": 1,
      "notInstalledDeviceCount": 7
    }
  ]
}
```



