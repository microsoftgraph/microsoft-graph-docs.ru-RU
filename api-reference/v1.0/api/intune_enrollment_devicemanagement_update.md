# <a name="update-devicemanagement"></a><span data-ttu-id="e7317-101">Обновление объекта deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e7317-101">Update deviceManagement</span></span>

> <span data-ttu-id="e7317-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e7317-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7317-103">Обновление свойств объекта [deviceManagement](../resources/intune_enrollment_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="e7317-103">Update the properties of a [calendar](../resources/intune_enrollment_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7317-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e7317-104">Prerequisites</span></span>
<span data-ttu-id="e7317-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e7317-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e7317-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7317-107">Permission type</span></span>|<span data-ttu-id="e7317-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7317-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7317-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7317-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e7317-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7317-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e7317-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7317-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7317-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7317-112">Not supported.</span></span>|
|<span data-ttu-id="e7317-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7317-113">Application</span></span>|<span data-ttu-id="e7317-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7317-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7317-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7317-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="e7317-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7317-116">Request headers</span></span>
|<span data-ttu-id="e7317-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e7317-117">Header</span></span>|<span data-ttu-id="e7317-118">Значение</span><span class="sxs-lookup"><span data-stu-id="e7317-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7317-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7317-119">Authorization</span></span>|<span data-ttu-id="e7317-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7317-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e7317-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e7317-121">Accept</span></span>|<span data-ttu-id="e7317-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e7317-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7317-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e7317-123">Request body</span></span>
<span data-ttu-id="e7317-124">В теле запроса добавьте представление объекта [deviceManagement](../resources/intune_enrollment_devicemanagement.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7317-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_enrollment_devicemanagement.md) object.</span></span>

<span data-ttu-id="e7317-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceManagement](../resources/intune_enrollment_devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="e7317-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="e7317-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7317-126">Property</span></span>|<span data-ttu-id="e7317-127">Тип</span><span class="sxs-lookup"><span data-stu-id="e7317-127">Type</span></span>|<span data-ttu-id="e7317-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e7317-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7317-129">id</span><span class="sxs-lookup"><span data-stu-id="e7317-129">id</span></span>|<span data-ttu-id="e7317-130">String</span><span class="sxs-lookup"><span data-stu-id="e7317-130">String</span></span>|<span data-ttu-id="e7317-131">GUID объекта.</span><span class="sxs-lookup"><span data-stu-id="e7317-131">The resource GUID for the security object is not valid.</span></span>|



## <a name="response"></a><span data-ttu-id="e7317-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7317-132">Response</span></span>
<span data-ttu-id="e7317-133">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagement](../resources/intune_enrollment_devicemanagement.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e7317-133">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_enrollment_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7317-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e7317-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7317-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7317-135">Request</span></span>
<span data-ttu-id="e7317-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7317-136">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="e7317-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="e7317-137">Response</span></span>
<span data-ttu-id="e7317-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e7317-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b"
}
```



