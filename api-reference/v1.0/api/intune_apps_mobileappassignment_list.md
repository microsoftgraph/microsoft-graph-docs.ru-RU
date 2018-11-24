# <a name="list-mobileappassignments"></a><span data-ttu-id="1c78c-101">Перечисление объектов mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="1c78c-101">List mobileAppAssignments</span></span>

> <span data-ttu-id="1c78c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1c78c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c78c-103">Список свойств и связей объектов [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1c78c-103">List properties and relationships of the [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1c78c-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1c78c-104">Prerequisites</span></span>
<span data-ttu-id="1c78c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1c78c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1c78c-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c78c-107">Permission type</span></span>|<span data-ttu-id="1c78c-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c78c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c78c-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c78c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1c78c-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c78c-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1c78c-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c78c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c78c-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c78c-112">Not supported.</span></span>|
|<span data-ttu-id="1c78c-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c78c-113">Application</span></span>|<span data-ttu-id="1c78c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c78c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c78c-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c78c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1c78c-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c78c-116">Request headers</span></span>
|<span data-ttu-id="1c78c-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c78c-117">Header</span></span>|<span data-ttu-id="1c78c-118">Значение</span><span class="sxs-lookup"><span data-stu-id="1c78c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c78c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c78c-119">Authorization</span></span>|<span data-ttu-id="1c78c-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c78c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c78c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1c78c-121">Accept</span></span>|<span data-ttu-id="1c78c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1c78c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c78c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c78c-123">Request body</span></span>
<span data-ttu-id="1c78c-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c78c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c78c-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c78c-125">Response</span></span>
<span data-ttu-id="1c78c-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1c78c-126">If successful, this method returns a `200 OK` response code and a collection of [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c78c-127">Пример</span><span class="sxs-lookup"><span data-stu-id="1c78c-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="1c78c-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c78c-128">Request</span></span>
<span data-ttu-id="1c78c-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c78c-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

### <a name="response"></a><span data-ttu-id="1c78c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c78c-130">Response</span></span>
<span data-ttu-id="1c78c-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1c78c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "settings": {
        "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
      }
    }
  ]
}
```



