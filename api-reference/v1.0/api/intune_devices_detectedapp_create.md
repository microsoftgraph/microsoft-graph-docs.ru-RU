# <a name="create-detectedapp"></a><span data-ttu-id="65359-101">Создание объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="65359-101">Create detectedApp</span></span>

> <span data-ttu-id="65359-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="65359-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65359-103">Создание объекта [detectedApp](../resources/intune_devices_detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="65359-103">Create a new [detectedApp](../resources/intune_devices_detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="65359-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="65359-104">Prerequisites</span></span>
<span data-ttu-id="65359-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="65359-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="65359-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65359-107">Permission type</span></span>|<span data-ttu-id="65359-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="65359-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65359-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65359-109">Delegated (work or school account)</span></span>|<span data-ttu-id="65359-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65359-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="65359-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65359-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65359-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65359-112">Not supported.</span></span>|
|<span data-ttu-id="65359-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65359-113">Application</span></span>|<span data-ttu-id="65359-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65359-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65359-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65359-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="65359-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65359-116">Request headers</span></span>
|<span data-ttu-id="65359-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65359-117">Header</span></span>|<span data-ttu-id="65359-118">Значение</span><span class="sxs-lookup"><span data-stu-id="65359-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65359-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="65359-119">Authorization</span></span>|<span data-ttu-id="65359-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65359-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65359-121">Accept</span><span class="sxs-lookup"><span data-stu-id="65359-121">Accept</span></span>|<span data-ttu-id="65359-122">application/json</span><span class="sxs-lookup"><span data-stu-id="65359-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65359-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="65359-123">Request body</span></span>
<span data-ttu-id="65359-124">В теле запроса добавьте представление объекта detectedApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65359-124">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="65359-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта detectedApp.</span><span class="sxs-lookup"><span data-stu-id="65359-125">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="65359-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="65359-126">Property</span></span>|<span data-ttu-id="65359-127">Тип</span><span class="sxs-lookup"><span data-stu-id="65359-127">Type</span></span>|<span data-ttu-id="65359-128">Описание</span><span class="sxs-lookup"><span data-stu-id="65359-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65359-129">id</span><span class="sxs-lookup"><span data-stu-id="65359-129">id</span></span>|<span data-ttu-id="65359-130">String</span><span class="sxs-lookup"><span data-stu-id="65359-130">String</span></span>|<span data-ttu-id="65359-131">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="65359-131">The unique Identifier for the detected application.</span></span> <span data-ttu-id="65359-132">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="65359-132">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="65359-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65359-133">Read-only.</span></span>|
|<span data-ttu-id="65359-134">displayName</span><span class="sxs-lookup"><span data-stu-id="65359-134">displayName</span></span>|<span data-ttu-id="65359-135">String</span><span class="sxs-lookup"><span data-stu-id="65359-135">String</span></span>|<span data-ttu-id="65359-136">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="65359-136">Name of the discovered application.</span></span> <span data-ttu-id="65359-137">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="65359-137">Read-only</span></span>|
|<span data-ttu-id="65359-138">version</span><span class="sxs-lookup"><span data-stu-id="65359-138">version</span></span>|<span data-ttu-id="65359-139">String</span><span class="sxs-lookup"><span data-stu-id="65359-139">String</span></span>|<span data-ttu-id="65359-140">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="65359-140">Version of the discovered application.</span></span> <span data-ttu-id="65359-141">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="65359-141">Read-only</span></span>|
|<span data-ttu-id="65359-142">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="65359-142">sizeInByte</span></span>|<span data-ttu-id="65359-143">Int64</span><span class="sxs-lookup"><span data-stu-id="65359-143">Int64</span></span>|<span data-ttu-id="65359-144">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="65359-144">Discovered application size in bytes.</span></span> <span data-ttu-id="65359-145">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="65359-145">Read-only</span></span>|
|<span data-ttu-id="65359-146">deviceCount</span><span class="sxs-lookup"><span data-stu-id="65359-146">deviceCount</span></span>|<span data-ttu-id="65359-147">Int32</span><span class="sxs-lookup"><span data-stu-id="65359-147">Int32</span></span>|<span data-ttu-id="65359-148">Количество устройств, на которых успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="65359-148">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="65359-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="65359-149">Response</span></span>
<span data-ttu-id="65359-150">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [detectedApp](../resources/intune_devices_detectedapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="65359-150">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune_devices_detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65359-151">Пример</span><span class="sxs-lookup"><span data-stu-id="65359-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="65359-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="65359-152">Request</span></span>
<span data-ttu-id="65359-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65359-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/detectedApps
Content-type: application/json
Content-length: 167

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="65359-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="65359-154">Response</span></span>
<span data-ttu-id="65359-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="65359-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 216

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```



