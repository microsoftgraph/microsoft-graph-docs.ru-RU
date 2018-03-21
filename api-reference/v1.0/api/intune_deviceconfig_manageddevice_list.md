# <a name="list-manageddevices"></a><span data-ttu-id="1ceda-101">Перечисление объектов managedDevice</span><span class="sxs-lookup"><span data-stu-id="1ceda-101">List managedDevices</span></span>

> <span data-ttu-id="1ceda-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1ceda-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ceda-103">Список свойств и связей объектов [managedDevice](../resources/intune_deviceconfig_manageddevice.md).</span><span class="sxs-lookup"><span data-stu-id="1ceda-103">List properties and relationships of the [managedDevice](../resources/intune_deviceconfig_manageddevice.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ceda-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1ceda-104">Prerequisites</span></span>
<span data-ttu-id="1ceda-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1ceda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1ceda-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ceda-107">Permission type</span></span>|<span data-ttu-id="1ceda-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ceda-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ceda-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ceda-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1ceda-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ceda-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1ceda-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ceda-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ceda-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ceda-112">Not supported.</span></span>|
|<span data-ttu-id="1ceda-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ceda-113">Application</span></span>|<span data-ttu-id="1ceda-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ceda-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ceda-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ceda-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="1ceda-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ceda-116">Request headers</span></span>
|<span data-ttu-id="1ceda-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ceda-117">Header</span></span>|<span data-ttu-id="1ceda-118">Значение</span><span class="sxs-lookup"><span data-stu-id="1ceda-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ceda-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ceda-119">Authorization</span></span>|<span data-ttu-id="1ceda-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ceda-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1ceda-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1ceda-121">Accept</span></span>|<span data-ttu-id="1ceda-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1ceda-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ceda-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ceda-123">Request body</span></span>
<span data-ttu-id="1ceda-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1ceda-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ceda-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ceda-125">Response</span></span>
<span data-ttu-id="1ceda-126">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [managedDevice](../resources/intune_deviceconfig_manageddevice.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1ceda-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/intune_deviceconfig_manageddevice.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ceda-127">Пример</span><span class="sxs-lookup"><span data-stu-id="1ceda-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ceda-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ceda-128">Request</span></span>
<span data-ttu-id="1ceda-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ceda-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/managedDevices
```

### <a name="response"></a><span data-ttu-id="1ceda-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ceda-130">Response</span></span>
<span data-ttu-id="1ceda-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1ceda-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 145

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDevice",
      "id": "705c034c-034c-705c-4c03-5c704c035c70"
    }
  ]
}
```



