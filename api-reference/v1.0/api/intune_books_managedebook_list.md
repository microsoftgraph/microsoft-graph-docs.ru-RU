# <a name="list-managedebooks"></a><span data-ttu-id="8ebf1-101">Перечисление объектов managedEBook</span><span class="sxs-lookup"><span data-stu-id="8ebf1-101">List managedEBooks</span></span>

> <span data-ttu-id="8ebf1-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8ebf1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ebf1-103">Список свойств и связей объектов [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="8ebf1-103">List properties and relationships of the [managedEBook](../resources/intune_books_managedebook.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8ebf1-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8ebf1-104">Prerequisites</span></span>
<span data-ttu-id="8ebf1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8ebf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8ebf1-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ebf1-107">Permission type</span></span>|<span data-ttu-id="8ebf1-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ebf1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ebf1-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ebf1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8ebf1-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ebf1-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8ebf1-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ebf1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ebf1-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ebf1-112">Not supported.</span></span>|
|<span data-ttu-id="8ebf1-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ebf1-113">Application</span></span>|<span data-ttu-id="8ebf1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ebf1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ebf1-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ebf1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="8ebf1-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ebf1-116">Request headers</span></span>
|<span data-ttu-id="8ebf1-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ebf1-117">Header</span></span>|<span data-ttu-id="8ebf1-118">Значение</span><span class="sxs-lookup"><span data-stu-id="8ebf1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ebf1-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ebf1-119">Authorization</span></span>|<span data-ttu-id="8ebf1-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="8ebf1-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ebf1-121">Принять</span><span class="sxs-lookup"><span data-stu-id="8ebf1-121">Accept</span></span>|<span data-ttu-id="8ebf1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8ebf1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ebf1-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ebf1-123">Request body</span></span>
<span data-ttu-id="8ebf1-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8ebf1-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ebf1-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ebf1-125">Response</span></span>
<span data-ttu-id="8ebf1-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedEBook](../resources/intune_books_managedebook.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8ebf1-126">If successful, this method returns a `200 OK` response code and a collection of [managedEBook](../resources/intune_books_managedebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ebf1-127">Пример</span><span class="sxs-lookup"><span data-stu-id="8ebf1-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="8ebf1-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ebf1-128">Request</span></span>
<span data-ttu-id="8ebf1-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ebf1-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="8ebf1-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="8ebf1-130">Response</span></span>
<span data-ttu-id="8ebf1-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ebf1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBook",
      "id": "1fbd3558-3558-1fbd-5835-bd1f5835bd1f",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
      "largeCover": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "informationUrl": "https://example.com/informationUrl/",
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/"
    }
  ]
}
```








