# <a name="create-devicecategory"></a><span data-ttu-id="1c892-101">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="1c892-101">Create deviceCategory</span></span>

> <span data-ttu-id="1c892-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1c892-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c892-103">Создание объекта [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="1c892-103">Create a new [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1c892-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1c892-104">Prerequisites</span></span>
<span data-ttu-id="1c892-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1c892-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1c892-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c892-107">Permission type</span></span>|<span data-ttu-id="1c892-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c892-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c892-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c892-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1c892-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c892-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1c892-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c892-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c892-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c892-112">Not supported.</span></span>|
|<span data-ttu-id="1c892-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c892-113">Application</span></span>|<span data-ttu-id="1c892-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c892-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c892-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c892-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="1c892-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1c892-116">Request headers</span></span>
|<span data-ttu-id="1c892-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c892-117">Header</span></span>|<span data-ttu-id="1c892-118">Значение</span><span class="sxs-lookup"><span data-stu-id="1c892-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c892-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c892-119">Authorization</span></span>|<span data-ttu-id="1c892-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c892-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c892-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1c892-121">Accept</span></span>|<span data-ttu-id="1c892-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1c892-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c892-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1c892-123">Request body</span></span>
<span data-ttu-id="1c892-124">В теле запроса добавьте представление объекта deviceCategory в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c892-124">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="1c892-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="1c892-125">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="1c892-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c892-126">Property</span></span>|<span data-ttu-id="1c892-127">Тип</span><span class="sxs-lookup"><span data-stu-id="1c892-127">Type</span></span>|<span data-ttu-id="1c892-128">Описание</span><span class="sxs-lookup"><span data-stu-id="1c892-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c892-129">id</span><span class="sxs-lookup"><span data-stu-id="1c892-129">id</span></span>|<span data-ttu-id="1c892-130">String</span><span class="sxs-lookup"><span data-stu-id="1c892-130">String</span></span>|<span data-ttu-id="1c892-131">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="1c892-131">Unique identifier for the device category.</span></span> <span data-ttu-id="1c892-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1c892-132">Read-only.</span></span>|
|<span data-ttu-id="1c892-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1c892-133">displayName</span></span>|<span data-ttu-id="1c892-134">String</span><span class="sxs-lookup"><span data-stu-id="1c892-134">String</span></span>|<span data-ttu-id="1c892-135">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="1c892-135">Display name for the device category.</span></span>|
|<span data-ttu-id="1c892-136">description</span><span class="sxs-lookup"><span data-stu-id="1c892-136">description</span></span>|<span data-ttu-id="1c892-137">String</span><span class="sxs-lookup"><span data-stu-id="1c892-137">String</span></span>|<span data-ttu-id="1c892-138">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="1c892-138">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="1c892-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c892-139">Response</span></span>
<span data-ttu-id="1c892-140">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCategory](../resources/intune_shared_devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1c892-140">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c892-141">Пример</span><span class="sxs-lookup"><span data-stu-id="1c892-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="1c892-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c892-142">Request</span></span>
<span data-ttu-id="1c892-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c892-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="1c892-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c892-144">Response</span></span>
<span data-ttu-id="1c892-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1c892-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



