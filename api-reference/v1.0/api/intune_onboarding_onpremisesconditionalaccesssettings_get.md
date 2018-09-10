# <a name="get-onpremisesconditionalaccesssettings"></a><span data-ttu-id="32272-101">Получение объекта onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="32272-101">Get onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="32272-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="32272-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32272-103">Чтение свойств и связей объекта [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md).</span><span class="sxs-lookup"><span data-stu-id="32272-103">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="32272-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="32272-104">Prerequisites</span></span>
<span data-ttu-id="32272-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="32272-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="32272-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32272-107">Permission type</span></span>|<span data-ttu-id="32272-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32272-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32272-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32272-109">Delegated (work or school account)</span></span>|<span data-ttu-id="32272-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="32272-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="32272-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32272-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32272-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32272-112">Not supported.</span></span>|
|<span data-ttu-id="32272-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32272-113">Application</span></span>|<span data-ttu-id="32272-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32272-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32272-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32272-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/conditionalAccessSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="32272-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="32272-116">Optional query parameters</span></span>
<span data-ttu-id="32272-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="32272-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="32272-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32272-118">Request headers</span></span>
|<span data-ttu-id="32272-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32272-119">Header</span></span>|<span data-ttu-id="32272-120">Значение</span><span class="sxs-lookup"><span data-stu-id="32272-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32272-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32272-121">Authorization</span></span>|<span data-ttu-id="32272-122">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="32272-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32272-123">Принять</span><span class="sxs-lookup"><span data-stu-id="32272-123">Accept</span></span>|<span data-ttu-id="32272-124">application/json</span><span class="sxs-lookup"><span data-stu-id="32272-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32272-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32272-125">Request body</span></span>
<span data-ttu-id="32272-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="32272-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32272-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="32272-127">Response</span></span>
<span data-ttu-id="32272-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="32272-128">If successful, this method returns a `200 OK` response code and [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32272-129">Пример</span><span class="sxs-lookup"><span data-stu-id="32272-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="32272-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="32272-130">Request</span></span>
<span data-ttu-id="32272-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32272-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
```

### <a name="response"></a><span data-ttu-id="32272-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="32272-132">Response</span></span>
<span data-ttu-id="32272-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32272-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 357

{
  "value": {
    "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
    "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
    "enabled": true,
    "includedGroups": [
      "<Unknown Primitive Type Edm.Guid>"
    ],
    "excludedGroups": [
      "<Unknown Primitive Type Edm.Guid>"
    ],
    "overrideDefaultRule": true
  }
}
```








