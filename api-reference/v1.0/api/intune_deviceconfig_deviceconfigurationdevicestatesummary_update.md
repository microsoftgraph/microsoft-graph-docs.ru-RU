# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="9f5f7-101">Обновление объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9f5f7-101">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="9f5f7-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9f5f7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f5f7-103">Обновление свойств объекта [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="9f5f7-103">Update the properties of a [calendar](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f5f7-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9f5f7-104">Prerequisites</span></span>
<span data-ttu-id="9f5f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9f5f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9f5f7-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f5f7-107">Permission type</span></span>|<span data-ttu-id="9f5f7-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f5f7-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f5f7-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f5f7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9f5f7-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f5f7-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f5f7-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f5f7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f5f7-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f5f7-112">Not supported.</span></span>|
|<span data-ttu-id="9f5f7-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f5f7-113">Application</span></span>|<span data-ttu-id="9f5f7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f5f7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f5f7-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f5f7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="9f5f7-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f5f7-116">Request headers</span></span>
|<span data-ttu-id="9f5f7-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f5f7-117">Header</span></span>|<span data-ttu-id="9f5f7-118">Значение</span><span class="sxs-lookup"><span data-stu-id="9f5f7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f5f7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f5f7-119">Authorization</span></span>|<span data-ttu-id="9f5f7-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f5f7-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9f5f7-121">Accept</span><span class="sxs-lookup"><span data-stu-id="9f5f7-121">Accept</span></span>|<span data-ttu-id="9f5f7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9f5f7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f5f7-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f5f7-123">Request body</span></span>
<span data-ttu-id="9f5f7-124">В тексте запроса добавьте представление объекта [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f5f7-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="9f5f7-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="9f5f7-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="9f5f7-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f5f7-126">Property</span></span>|<span data-ttu-id="9f5f7-127">Тип</span><span class="sxs-lookup"><span data-stu-id="9f5f7-127">Type</span></span>|<span data-ttu-id="9f5f7-128">Описание</span><span class="sxs-lookup"><span data-stu-id="9f5f7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f5f7-129">id</span><span class="sxs-lookup"><span data-stu-id="9f5f7-129">id</span></span>|<span data-ttu-id="9f5f7-130">String</span><span class="sxs-lookup"><span data-stu-id="9f5f7-130">String</span></span>|<span data-ttu-id="9f5f7-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9f5f7-131">Key of the setting.</span></span>|
|<span data-ttu-id="9f5f7-132">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9f5f7-132">unknownDeviceCount</span></span>|<span data-ttu-id="9f5f7-133">Int32</span><span class="sxs-lookup"><span data-stu-id="9f5f7-133">Int32</span></span>|<span data-ttu-id="9f5f7-134">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="9f5f7-134">Number of unknown devices</span></span>|
|<span data-ttu-id="9f5f7-135">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9f5f7-135">notApplicableDeviceCount</span></span>|<span data-ttu-id="9f5f7-136">Int32</span><span class="sxs-lookup"><span data-stu-id="9f5f7-136">Int32</span></span>|<span data-ttu-id="9f5f7-137">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="9f5f7-137">Number of not applicable devices</span></span>|
|<span data-ttu-id="9f5f7-138">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9f5f7-138">compliantDeviceCount</span></span>|<span data-ttu-id="9f5f7-139">Int32</span><span class="sxs-lookup"><span data-stu-id="9f5f7-139">Int32</span></span>|<span data-ttu-id="9f5f7-140">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="9f5f7-140">Number of compliant devices</span></span>|
|<span data-ttu-id="9f5f7-141">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9f5f7-141">remediatedDeviceCount</span></span>|<span data-ttu-id="9f5f7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="9f5f7-142">Int32</span></span>|<span data-ttu-id="9f5f7-143">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="9f5f7-143">Number of remediated devices</span></span>|
|<span data-ttu-id="9f5f7-144">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9f5f7-144">nonCompliantDeviceCount</span></span>|<span data-ttu-id="9f5f7-145">Int32</span><span class="sxs-lookup"><span data-stu-id="9f5f7-145">Int32</span></span>|<span data-ttu-id="9f5f7-146">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="9f5f7-146">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="9f5f7-147">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9f5f7-147">errorDeviceCount</span></span>|<span data-ttu-id="9f5f7-148">Int32</span><span class="sxs-lookup"><span data-stu-id="9f5f7-148">Int32</span></span>|<span data-ttu-id="9f5f7-149">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="9f5f7-149">Number of error devices</span></span>|
|<span data-ttu-id="9f5f7-150">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9f5f7-150">conflictDeviceCount</span></span>|<span data-ttu-id="9f5f7-151">Int32</span><span class="sxs-lookup"><span data-stu-id="9f5f7-151">Int32</span></span>|<span data-ttu-id="9f5f7-152">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="9f5f7-152">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="9f5f7-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f5f7-153">Response</span></span>
<span data-ttu-id="9f5f7-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceStateSummary](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f5f7-154">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f5f7-155">Пример</span><span class="sxs-lookup"><span data-stu-id="9f5f7-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f5f7-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f5f7-156">Request</span></span>
<span data-ttu-id="9f5f7-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f5f7-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 214

{
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="9f5f7-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f5f7-158">Response</span></span>
<span data-ttu-id="9f5f7-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9f5f7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



