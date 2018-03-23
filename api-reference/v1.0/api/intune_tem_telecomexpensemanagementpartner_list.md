# <a name="list-telecomexpensemanagementpartners"></a><span data-ttu-id="8edae-101">Список объектов telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="8edae-101">List telecomExpenseManagementPartners</span></span>

> <span data-ttu-id="8edae-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8edae-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8edae-103">Список свойств и связей объектов [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="8edae-103">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8edae-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8edae-104">Prerequisites</span></span>
<span data-ttu-id="8edae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8edae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8edae-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8edae-107">Permission type</span></span>|<span data-ttu-id="8edae-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8edae-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8edae-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8edae-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8edae-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8edae-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8edae-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8edae-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8edae-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8edae-112">Not supported.</span></span>|
|<span data-ttu-id="8edae-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8edae-113">Application</span></span>|<span data-ttu-id="8edae-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8edae-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8edae-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8edae-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="8edae-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8edae-116">Request headers</span></span>
|<span data-ttu-id="8edae-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8edae-117">Header</span></span>|<span data-ttu-id="8edae-118">Значение</span><span class="sxs-lookup"><span data-stu-id="8edae-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8edae-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8edae-119">Authorization</span></span>|<span data-ttu-id="8edae-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8edae-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8edae-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8edae-121">Accept</span></span>|<span data-ttu-id="8edae-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8edae-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8edae-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8edae-123">Request body</span></span>
<span data-ttu-id="8edae-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8edae-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8edae-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="8edae-125">Response</span></span>
<span data-ttu-id="8edae-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8edae-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/intune_tem_telecomexpensemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8edae-127">Пример</span><span class="sxs-lookup"><span data-stu-id="8edae-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="8edae-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="8edae-128">Request</span></span>
<span data-ttu-id="8edae-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8edae-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
```

### <a name="response"></a><span data-ttu-id="8edae-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="8edae-130">Response</span></span>
<span data-ttu-id="8edae-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8edae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 358

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
      "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
      "displayName": "Display Name value",
      "url": "Url value",
      "appAuthorized": true,
      "enabled": true,
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
    }
  ]
}
```



