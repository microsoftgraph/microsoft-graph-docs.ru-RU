# <a name="list-devicecategories"></a><span data-ttu-id="b2d22-101">Перечисление объектов deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b2d22-101">List deviceCategories</span></span>

> <span data-ttu-id="b2d22-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b2d22-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2d22-103">Список свойств и связей объектов [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="b2d22-103">List properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b2d22-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b2d22-104">Prerequisites</span></span>
<span data-ttu-id="b2d22-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b2d22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b2d22-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2d22-107">Permission type</span></span>|<span data-ttu-id="b2d22-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2d22-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2d22-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2d22-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b2d22-110">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="b2d22-110">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b2d22-111">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2d22-111">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b2d22-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2d22-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2d22-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2d22-113">Not supported.</span></span>|
|<span data-ttu-id="b2d22-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2d22-114">Application</span></span>|<span data-ttu-id="b2d22-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2d22-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2d22-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2d22-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="b2d22-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2d22-117">Request headers</span></span>
|<span data-ttu-id="b2d22-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2d22-118">Header</span></span>|<span data-ttu-id="b2d22-119">Значение</span><span class="sxs-lookup"><span data-stu-id="b2d22-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2d22-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2d22-120">Authorization</span></span>|<span data-ttu-id="b2d22-121">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b2d22-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2d22-122">Accept</span><span class="sxs-lookup"><span data-stu-id="b2d22-122">Accept</span></span>|<span data-ttu-id="b2d22-123">application/json</span><span class="sxs-lookup"><span data-stu-id="b2d22-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2d22-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2d22-124">Request body</span></span>
<span data-ttu-id="b2d22-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2d22-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2d22-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2d22-126">Response</span></span>
<span data-ttu-id="b2d22-127">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCategory](../resources/intune_shared_devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b2d22-127">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune_shared_devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2d22-128">Пример</span><span class="sxs-lookup"><span data-stu-id="b2d22-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="b2d22-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2d22-129">Request</span></span>
<span data-ttu-id="b2d22-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2d22-130">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="b2d22-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="b2d22-131">Response</span></span>
<span data-ttu-id="b2d22-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="b2d22-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCategory",
      "id": "f881b841-b841-f881-41b8-81f841b881f8",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```



