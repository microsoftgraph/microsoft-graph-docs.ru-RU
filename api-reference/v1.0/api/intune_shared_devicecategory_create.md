# <a name="create-devicecategory"></a><span data-ttu-id="05456-101">Создание объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="05456-101">Create deviceCategory</span></span>

> <span data-ttu-id="05456-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="05456-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05456-103">Создание объекта [deviceCategory](../resources/intune_shared_devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="05456-103">Create a new [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05456-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="05456-104">Prerequisites</span></span>
<span data-ttu-id="05456-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="05456-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="05456-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05456-107">Permission type</span></span>|<span data-ttu-id="05456-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05456-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05456-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05456-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="05456-110">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="05456-110">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="05456-111">DeviceManagementManaged Devices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05456-111">DeviceManagementManaged Devices.ReadWrite.All</span></span>|
|<span data-ttu-id="05456-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05456-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05456-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05456-113">Not supported.</span></span>|
|<span data-ttu-id="05456-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05456-114">Application</span></span>|<span data-ttu-id="05456-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05456-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05456-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05456-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="05456-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05456-117">Request headers</span></span>
|<span data-ttu-id="05456-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05456-118">Header</span></span>|<span data-ttu-id="05456-119">Значение</span><span class="sxs-lookup"><span data-stu-id="05456-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05456-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="05456-120">Authorization</span></span>|<span data-ttu-id="05456-121">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="05456-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05456-122">Accept</span><span class="sxs-lookup"><span data-stu-id="05456-122">Accept</span></span>|<span data-ttu-id="05456-123">application/json</span><span class="sxs-lookup"><span data-stu-id="05456-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05456-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05456-124">Request body</span></span>
<span data-ttu-id="05456-125">В теле запроса добавьте представление объекта deviceCategory в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05456-125">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="05456-126">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceCategory.</span><span class="sxs-lookup"><span data-stu-id="05456-126">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="05456-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="05456-127">Property</span></span>|<span data-ttu-id="05456-128">Тип</span><span class="sxs-lookup"><span data-stu-id="05456-128">Type</span></span>|<span data-ttu-id="05456-129">Описание</span><span class="sxs-lookup"><span data-stu-id="05456-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05456-130">id</span><span class="sxs-lookup"><span data-stu-id="05456-130">id</span></span>|<span data-ttu-id="05456-131">String</span><span class="sxs-lookup"><span data-stu-id="05456-131">String</span></span>|<span data-ttu-id="05456-132">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="05456-132">Unique identifier for the device category.</span></span> <span data-ttu-id="05456-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="05456-133">Read-only.</span></span>|
|<span data-ttu-id="05456-134">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="05456-134">**Onboarding**</span></span>|
|<span data-ttu-id="05456-135">displayName</span><span class="sxs-lookup"><span data-stu-id="05456-135">displayName</span></span>|<span data-ttu-id="05456-136">String</span><span class="sxs-lookup"><span data-stu-id="05456-136">String</span></span>|<span data-ttu-id="05456-137">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="05456-137">Display name for the device category.</span></span>|
|<span data-ttu-id="05456-138">описание</span><span class="sxs-lookup"><span data-stu-id="05456-138">description</span></span>|<span data-ttu-id="05456-139">String</span><span class="sxs-lookup"><span data-stu-id="05456-139">String</span></span>|<span data-ttu-id="05456-140">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="05456-140">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="05456-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="05456-141">Response</span></span>
<span data-ttu-id="05456-142">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceCategory](../resources/intune_shared_devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="05456-142">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05456-143">Пример</span><span class="sxs-lookup"><span data-stu-id="05456-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="05456-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="05456-144">Request</span></span>
<span data-ttu-id="05456-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05456-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="05456-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="05456-146">Response</span></span>
<span data-ttu-id="05456-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="05456-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



