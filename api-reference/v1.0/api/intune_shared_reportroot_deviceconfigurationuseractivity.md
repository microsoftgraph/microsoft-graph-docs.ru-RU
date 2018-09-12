# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="06ef1-101">Функция deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="06ef1-101">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="06ef1-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="06ef1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06ef1-103">Метаданные для отчета о действиях пользователей с конфигурацией устройств</span><span class="sxs-lookup"><span data-stu-id="06ef1-103">Metadata for the device configuration user activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06ef1-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="06ef1-104">Prerequisites</span></span>
<span data-ttu-id="06ef1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="06ef1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="06ef1-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06ef1-107">Permission type</span></span>|<span data-ttu-id="06ef1-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="06ef1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06ef1-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06ef1-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="06ef1-110">&nbsp; &nbsp; Конфигурация устройства</span><span class="sxs-lookup"><span data-stu-id="06ef1-110">&nbsp; &nbsp;Device Configuration.</span></span> | <span data-ttu-id="06ef1-111">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="06ef1-111">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="06ef1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06ef1-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06ef1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06ef1-113">Not supported.</span></span>|
|<span data-ttu-id="06ef1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06ef1-114">Application</span></span>|<span data-ttu-id="06ef1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06ef1-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06ef1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06ef1-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="06ef1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06ef1-117">Request headers</span></span>
|<span data-ttu-id="06ef1-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="06ef1-118">Header</span></span>|<span data-ttu-id="06ef1-119">Значение</span><span class="sxs-lookup"><span data-stu-id="06ef1-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06ef1-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06ef1-120">Authorization</span></span>|<span data-ttu-id="06ef1-121">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="06ef1-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06ef1-122">Принять</span><span class="sxs-lookup"><span data-stu-id="06ef1-122">Accept</span></span>|<span data-ttu-id="06ef1-123">application/json</span><span class="sxs-lookup"><span data-stu-id="06ef1-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06ef1-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06ef1-124">Request body</span></span>
<span data-ttu-id="06ef1-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06ef1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06ef1-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="06ef1-126">Response</span></span>
<span data-ttu-id="06ef1-127">В случае успешного выполнения эта функция возвращает код отклика `200 OK` и объект [report](../resources/intune_shared_report.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06ef1-127">If successful, this function returns a `200 OK` response code and a [report](../resources/intune_shared_report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06ef1-128">Пример</span><span class="sxs-lookup"><span data-stu-id="06ef1-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="06ef1-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="06ef1-129">Request</span></span>
<span data-ttu-id="06ef1-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06ef1-130">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="06ef1-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="06ef1-131">Response</span></span>
<span data-ttu-id="06ef1-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06ef1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```








