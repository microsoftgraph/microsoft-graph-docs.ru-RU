# <a name="list-organizations"></a><span data-ttu-id="b8f4d-101">Список организаций</span><span class="sxs-lookup"><span data-stu-id="b8f4d-101">List organizations</span></span>

> <span data-ttu-id="b8f4d-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b8f4d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8f4d-103">Список свойств и связей объектов [organization](../resources/intune_onboarding_organization.md).</span><span class="sxs-lookup"><span data-stu-id="b8f4d-103">List properties and relationships of the [organization](../resources/intune_onboarding_organization.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b8f4d-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b8f4d-104">Prerequisites</span></span>
<span data-ttu-id="b8f4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b8f4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b8f4d-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8f4d-107">Permission type</span></span>|<span data-ttu-id="b8f4d-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8f4d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8f4d-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8f4d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b8f4d-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b8f4d-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b8f4d-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8f4d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8f4d-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8f4d-112">Not supported.</span></span>|
|<span data-ttu-id="b8f4d-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8f4d-113">Application</span></span>|<span data-ttu-id="b8f4d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8f4d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8f4d-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8f4d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization
```

## <a name="request-headers"></a><span data-ttu-id="b8f4d-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8f4d-116">Request headers</span></span>
|<span data-ttu-id="b8f4d-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8f4d-117">Header</span></span>|<span data-ttu-id="b8f4d-118">Значение</span><span class="sxs-lookup"><span data-stu-id="b8f4d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8f4d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8f4d-119">Authorization</span></span>|<span data-ttu-id="b8f4d-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8f4d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8f4d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b8f4d-121">Accept</span></span>|<span data-ttu-id="b8f4d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b8f4d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8f4d-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8f4d-123">Request body</span></span>
<span data-ttu-id="b8f4d-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b8f4d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8f4d-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8f4d-125">Response</span></span>
<span data-ttu-id="b8f4d-126">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [organization](../resources/intune_onboarding_organization.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b8f4d-126">If successful, this method returns a `200 OK` response code and a collection of [organization](../resources/intune_onboarding_organization.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8f4d-127">Пример</span><span class="sxs-lookup"><span data-stu-id="b8f4d-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="b8f4d-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8f4d-128">Request</span></span>
<span data-ttu-id="b8f4d-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8f4d-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/organization
```

### <a name="response"></a><span data-ttu-id="b8f4d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b8f4d-130">Response</span></span>
<span data-ttu-id="b8f4d-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b8f4d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 196

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.organization",
      "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
      "mobileDeviceManagementAuthority": "intune"
    }
  ]
}
```



