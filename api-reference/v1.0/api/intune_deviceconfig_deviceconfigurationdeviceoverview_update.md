# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="f69c9-101">Обновление объекта deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f69c9-101">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="f69c9-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f69c9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f69c9-103">Обновление свойств объекта [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="f69c9-103">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f69c9-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f69c9-104">Prerequisites</span></span>
<span data-ttu-id="f69c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f69c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f69c9-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f69c9-107">Permission type</span></span>|<span data-ttu-id="f69c9-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f69c9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f69c9-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f69c9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f69c9-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f69c9-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f69c9-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f69c9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f69c9-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f69c9-112">Not supported.</span></span>|
|<span data-ttu-id="f69c9-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f69c9-113">Application</span></span>|<span data-ttu-id="f69c9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f69c9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f69c9-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f69c9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="f69c9-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f69c9-116">Request headers</span></span>
|<span data-ttu-id="f69c9-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f69c9-117">Header</span></span>|<span data-ttu-id="f69c9-118">Значение</span><span class="sxs-lookup"><span data-stu-id="f69c9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f69c9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f69c9-119">Authorization</span></span>|<span data-ttu-id="f69c9-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f69c9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f69c9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f69c9-121">Accept</span></span>|<span data-ttu-id="f69c9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f69c9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f69c9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f69c9-123">Request body</span></span>
<span data-ttu-id="f69c9-124">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f69c9-124">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="f69c9-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="f69c9-125">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="f69c9-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="f69c9-126">Property</span></span>|<span data-ttu-id="f69c9-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f69c9-127">Type</span></span>|<span data-ttu-id="f69c9-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f69c9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f69c9-129">id</span><span class="sxs-lookup"><span data-stu-id="f69c9-129">id</span></span>|<span data-ttu-id="f69c9-130">String</span><span class="sxs-lookup"><span data-stu-id="f69c9-130">String</span></span>|<span data-ttu-id="f69c9-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f69c9-131">Key of the entity.</span></span>|
|<span data-ttu-id="f69c9-132">pendingCount</span><span class="sxs-lookup"><span data-stu-id="f69c9-132">pendingCount</span></span>|<span data-ttu-id="f69c9-133">Int32</span><span class="sxs-lookup"><span data-stu-id="f69c9-133">Int32</span></span>|<span data-ttu-id="f69c9-134">Количество ожидающих устройств.</span><span class="sxs-lookup"><span data-stu-id="f69c9-134">Number of pending devices</span></span>|
|<span data-ttu-id="f69c9-135">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f69c9-135">notApplicableCount</span></span>|<span data-ttu-id="f69c9-136">Int32</span><span class="sxs-lookup"><span data-stu-id="f69c9-136">Int32</span></span>|<span data-ttu-id="f69c9-137">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="f69c9-137">Number of not applicable devices</span></span>|
|<span data-ttu-id="f69c9-138">successCount</span><span class="sxs-lookup"><span data-stu-id="f69c9-138">successCount</span></span>|<span data-ttu-id="f69c9-139">Int32</span><span class="sxs-lookup"><span data-stu-id="f69c9-139">Int32</span></span>|<span data-ttu-id="f69c9-140">Количество успешных устройств.</span><span class="sxs-lookup"><span data-stu-id="f69c9-140">Number of succeeded devices</span></span>|
|<span data-ttu-id="f69c9-141">errorCount</span><span class="sxs-lookup"><span data-stu-id="f69c9-141">errorCount</span></span>|<span data-ttu-id="f69c9-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f69c9-142">Int32</span></span>|<span data-ttu-id="f69c9-143">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="f69c9-143">Number of error devices</span></span>|
|<span data-ttu-id="f69c9-144">failedCount</span><span class="sxs-lookup"><span data-stu-id="f69c9-144">failedCount</span></span>|<span data-ttu-id="f69c9-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f69c9-145">Int32</span></span>|<span data-ttu-id="f69c9-146">Число устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="f69c9-146">Number of failed devices</span></span>|
|<span data-ttu-id="f69c9-147">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f69c9-147">lastUpdateDateTime</span></span>|<span data-ttu-id="f69c9-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f69c9-148">DateTimeOffset</span></span>|<span data-ttu-id="f69c9-149">Время последнего обновления.</span><span class="sxs-lookup"><span data-stu-id="f69c9-149">Last update time</span></span>|
|<span data-ttu-id="f69c9-150">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="f69c9-150">configurationVersion</span></span>|<span data-ttu-id="f69c9-151">Int32</span><span class="sxs-lookup"><span data-stu-id="f69c9-151">Int32</span></span>|<span data-ttu-id="f69c9-152">Версия политики для этого обзора.</span><span class="sxs-lookup"><span data-stu-id="f69c9-152">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="f69c9-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="f69c9-153">Response</span></span>
<span data-ttu-id="f69c9-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f69c9-154">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f69c9-155">Пример</span><span class="sxs-lookup"><span data-stu-id="f69c9-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="f69c9-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="f69c9-156">Request</span></span>
<span data-ttu-id="f69c9-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f69c9-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 284

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="f69c9-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="f69c9-158">Response</span></span>
<span data-ttu-id="f69c9-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f69c9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 333

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



