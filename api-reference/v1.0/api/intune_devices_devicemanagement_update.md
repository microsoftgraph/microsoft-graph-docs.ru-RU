# <a name="update-devicemanagement"></a><span data-ttu-id="f96fb-101">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="f96fb-101">Update deviceManagement</span></span>

> <span data-ttu-id="f96fb-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f96fb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f96fb-103">Обновление свойств объекта [deviceManagement](../resources/intune_devices_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="f96fb-103">Update the properties of a [calendar](../resources/intune_devices_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f96fb-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f96fb-104">Prerequisites</span></span>
<span data-ttu-id="f96fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f96fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f96fb-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f96fb-107">Permission type</span></span>|<span data-ttu-id="f96fb-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f96fb-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f96fb-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f96fb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f96fb-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f96fb-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f96fb-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f96fb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f96fb-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f96fb-112">Not supported.</span></span>|
|<span data-ttu-id="f96fb-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f96fb-113">Application</span></span>|<span data-ttu-id="f96fb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f96fb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f96fb-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f96fb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="f96fb-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f96fb-116">Request headers</span></span>
|<span data-ttu-id="f96fb-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f96fb-117">Header</span></span>|<span data-ttu-id="f96fb-118">Значение</span><span class="sxs-lookup"><span data-stu-id="f96fb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f96fb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f96fb-119">Authorization</span></span>|<span data-ttu-id="f96fb-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f96fb-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f96fb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f96fb-121">Accept</span></span>|<span data-ttu-id="f96fb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f96fb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f96fb-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f96fb-123">Request body</span></span>
<span data-ttu-id="f96fb-124">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune_devices_devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f96fb-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_devices_devicemanagement.md) object.</span></span>

<span data-ttu-id="f96fb-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune_devices_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="f96fb-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="f96fb-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="f96fb-126">Property</span></span>|<span data-ttu-id="f96fb-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f96fb-127">Type</span></span>|<span data-ttu-id="f96fb-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f96fb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f96fb-129">id</span><span class="sxs-lookup"><span data-stu-id="f96fb-129">id</span></span>|<span data-ttu-id="f96fb-130">String</span><span class="sxs-lookup"><span data-stu-id="f96fb-130">String</span></span>|<span data-ttu-id="f96fb-131">Уникальный идентификатор устройства.</span><span class="sxs-lookup"><span data-stu-id="f96fb-131">Unique Identifier for the device</span></span>|
|<span data-ttu-id="f96fb-132">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="f96fb-132">subscriptionState</span></span>|<span data-ttu-id="f96fb-133">String</span><span class="sxs-lookup"><span data-stu-id="f96fb-133">String</span></span>|<span data-ttu-id="f96fb-134">Состояние подписки на управление мобильными устройствами для клиента.</span><span class="sxs-lookup"><span data-stu-id="f96fb-134">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="f96fb-135">Возможные значения: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="f96fb-135">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="f96fb-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f96fb-136">Response</span></span>
<span data-ttu-id="f96fb-137">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune_devices_devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f96fb-137">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_devices_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f96fb-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f96fb-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="f96fb-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f96fb-139">Request</span></span>
<span data-ttu-id="f96fb-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f96fb-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement
Content-type: application/json
Content-length: 37

{
  "subscriptionState": "active"
}
```

### <a name="response"></a><span data-ttu-id="f96fb-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="f96fb-141">Response</span></span>
<span data-ttu-id="f96fb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f96fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 141

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "subscriptionState": "active"
}
```



