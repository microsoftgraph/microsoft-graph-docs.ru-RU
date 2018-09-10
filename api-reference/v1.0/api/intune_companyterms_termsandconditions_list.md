# <a name="list-termsandconditionses"></a><span data-ttu-id="a9048-101">Перечисление объектов termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="a9048-101">List termsAndConditionses</span></span>

> <span data-ttu-id="a9048-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a9048-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9048-103">Список свойств и связей объектов [termsAndConditions](../resources/intune_companyterms_termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="a9048-103">List properties and relationships of the [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a9048-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a9048-104">Prerequisites</span></span>
<span data-ttu-id="a9048-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a9048-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a9048-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9048-107">Permission type</span></span>|<span data-ttu-id="a9048-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9048-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9048-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9048-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a9048-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9048-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a9048-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9048-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9048-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9048-112">Not supported.</span></span>|
|<span data-ttu-id="a9048-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9048-113">Application</span></span>|<span data-ttu-id="a9048-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9048-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9048-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9048-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="a9048-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9048-116">Request headers</span></span>
|<span data-ttu-id="a9048-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9048-117">Header</span></span>|<span data-ttu-id="a9048-118">Значение</span><span class="sxs-lookup"><span data-stu-id="a9048-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9048-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9048-119">Authorization</span></span>|<span data-ttu-id="a9048-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="a9048-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9048-121">Принять</span><span class="sxs-lookup"><span data-stu-id="a9048-121">Accept</span></span>|<span data-ttu-id="a9048-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a9048-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9048-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9048-123">Request body</span></span>
<span data-ttu-id="a9048-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a9048-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9048-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9048-125">Response</span></span>
<span data-ttu-id="a9048-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a9048-126">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9048-127">Пример</span><span class="sxs-lookup"><span data-stu-id="a9048-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="a9048-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9048-128">Request</span></span>
<span data-ttu-id="a9048-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9048-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
```

### <a name="response"></a><span data-ttu-id="a9048-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9048-130">Response</span></span>
<span data-ttu-id="a9048-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9048-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditions",
      "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "title": "Title value",
      "bodyText": "Body Text value",
      "acceptanceStatement": "Acceptance Statement value",
      "version": 7
    }
  ]
}
```








