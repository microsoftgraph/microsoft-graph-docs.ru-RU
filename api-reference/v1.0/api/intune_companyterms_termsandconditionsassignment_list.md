# <a name="list-termsandconditionsassignments"></a><span data-ttu-id="2b981-101">Перечисление объектов termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="2b981-101">List termsAndConditionsAssignments</span></span>

> <span data-ttu-id="2b981-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2b981-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b981-103">Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2b981-103">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2b981-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2b981-104">Prerequisites</span></span>
<span data-ttu-id="2b981-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2b981-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2b981-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b981-107">Permission type</span></span>|<span data-ttu-id="2b981-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b981-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b981-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b981-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2b981-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b981-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2b981-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b981-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b981-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b981-112">Not supported.</span></span>|
|<span data-ttu-id="2b981-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b981-113">Application</span></span>|<span data-ttu-id="2b981-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b981-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b981-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b981-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="2b981-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b981-116">Request headers</span></span>
|<span data-ttu-id="2b981-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b981-117">Header</span></span>|<span data-ttu-id="2b981-118">Значение</span><span class="sxs-lookup"><span data-stu-id="2b981-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b981-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b981-119">Authorization</span></span>|<span data-ttu-id="2b981-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b981-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b981-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2b981-121">Accept</span></span>|<span data-ttu-id="2b981-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2b981-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b981-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b981-123">Request body</span></span>
<span data-ttu-id="2b981-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b981-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b981-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b981-125">Response</span></span>
<span data-ttu-id="2b981-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b981-126">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b981-127">Пример</span><span class="sxs-lookup"><span data-stu-id="2b981-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="2b981-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b981-128">Request</span></span>
<span data-ttu-id="2b981-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b981-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

### <a name="response"></a><span data-ttu-id="2b981-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b981-130">Response</span></span>
<span data-ttu-id="2b981-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2b981-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
      "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



