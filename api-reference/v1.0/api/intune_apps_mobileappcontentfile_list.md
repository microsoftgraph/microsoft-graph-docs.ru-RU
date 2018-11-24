# <a name="list-mobileappcontentfiles"></a><span data-ttu-id="c8020-101">Перечисление объектов mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="c8020-101">List mobileAppContentFiles</span></span>

> <span data-ttu-id="c8020-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c8020-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8020-103">Список свойств и связей объектов [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="c8020-103">List properties and relationships of the [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c8020-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c8020-104">Prerequisites</span></span>
<span data-ttu-id="c8020-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c8020-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c8020-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8020-107">Permission type</span></span>|<span data-ttu-id="c8020-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8020-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8020-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8020-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c8020-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8020-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c8020-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8020-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8020-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8020-112">Not supported.</span></span>|
|<span data-ttu-id="c8020-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8020-113">Application</span></span>|<span data-ttu-id="c8020-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8020-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8020-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8020-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="c8020-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8020-116">Request headers</span></span>
|<span data-ttu-id="c8020-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8020-117">Header</span></span>|<span data-ttu-id="c8020-118">Значение</span><span class="sxs-lookup"><span data-stu-id="c8020-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8020-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8020-119">Authorization</span></span>|<span data-ttu-id="c8020-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8020-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8020-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c8020-121">Accept</span></span>|<span data-ttu-id="c8020-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c8020-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8020-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8020-123">Request body</span></span>
<span data-ttu-id="c8020-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8020-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8020-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8020-125">Response</span></span>
<span data-ttu-id="c8020-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c8020-126">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8020-127">Пример</span><span class="sxs-lookup"><span data-stu-id="c8020-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8020-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8020-128">Request</span></span>
<span data-ttu-id="c8020-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8020-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

### <a name="response"></a><span data-ttu-id="c8020-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c8020-130">Response</span></span>
<span data-ttu-id="c8020-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c8020-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 527

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppContentFile",
      "azureStorageUri": "Azure Storage Uri value",
      "isCommitted": true,
      "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "name": "Name value",
      "size": 4,
      "sizeEncrypted": 13,
      "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
      "manifest": "bWFuaWZlc3Q=",
      "uploadState": "transientError"
    }
  ]
}
```



