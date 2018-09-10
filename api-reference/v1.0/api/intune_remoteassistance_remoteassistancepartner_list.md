# <a name="list-remoteassistancepartners"></a><span data-ttu-id="d5888-101">Список объектов remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="d5888-101">List remoteAssistancePartners</span></span>

> <span data-ttu-id="d5888-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d5888-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5888-103">Список свойств и связей объектов [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).</span><span class="sxs-lookup"><span data-stu-id="d5888-103">List properties and relationships of the [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d5888-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d5888-104">Prerequisites</span></span>
<span data-ttu-id="d5888-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d5888-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d5888-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5888-107">Permission type</span></span>|<span data-ttu-id="d5888-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5888-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5888-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5888-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d5888-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5888-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d5888-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5888-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5888-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5888-112">Not supported.</span></span>|
|<span data-ttu-id="d5888-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5888-113">Application</span></span>|<span data-ttu-id="d5888-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5888-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5888-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5888-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="d5888-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5888-116">Request headers</span></span>
|<span data-ttu-id="d5888-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5888-117">Header</span></span>|<span data-ttu-id="d5888-118">Значение</span><span class="sxs-lookup"><span data-stu-id="d5888-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5888-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5888-119">Authorization</span></span>|<span data-ttu-id="d5888-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="d5888-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5888-121">Принять</span><span class="sxs-lookup"><span data-stu-id="d5888-121">Accept</span></span>|<span data-ttu-id="d5888-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d5888-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5888-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5888-123">Request body</span></span>
<span data-ttu-id="d5888-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d5888-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5888-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5888-125">Response</span></span>
<span data-ttu-id="d5888-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d5888-126">If successful, this method returns a `200 OK` response code and a collection of [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5888-127">Пример</span><span class="sxs-lookup"><span data-stu-id="d5888-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="d5888-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5888-128">Request</span></span>
<span data-ttu-id="d5888-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5888-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners
```

### <a name="response"></a><span data-ttu-id="d5888-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d5888-130">Response</span></span>
<span data-ttu-id="d5888-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5888-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.remoteAssistancePartner",
      "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
      "displayName": "Display Name value",
      "onboardingUrl": "https://example.com/onboardingUrl/",
      "onboardingStatus": "onboarding",
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
    }
  ]
}
```








