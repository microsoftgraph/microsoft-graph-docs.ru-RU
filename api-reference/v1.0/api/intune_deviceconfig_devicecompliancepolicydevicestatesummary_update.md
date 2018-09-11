# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="ac799-101">Обновление объекта deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="ac799-101">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="ac799-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ac799-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac799-103">Обновление свойств объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="ac799-103">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ac799-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ac799-104">Prerequisites</span></span>
<span data-ttu-id="ac799-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ac799-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ac799-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac799-107">Permission type</span></span>|<span data-ttu-id="ac799-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac799-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac799-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac799-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ac799-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac799-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ac799-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac799-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac799-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac799-112">Not supported.</span></span>|
|<span data-ttu-id="ac799-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac799-113">Application</span></span>|<span data-ttu-id="ac799-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac799-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac799-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac799-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="ac799-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac799-116">Request headers</span></span>
|<span data-ttu-id="ac799-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ac799-117">Header</span></span>|<span data-ttu-id="ac799-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ac799-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac799-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac799-119">Authorization</span></span>|<span data-ttu-id="ac799-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="ac799-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac799-121">Принять</span><span class="sxs-lookup"><span data-stu-id="ac799-121">Accept</span></span>|<span data-ttu-id="ac799-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ac799-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac799-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac799-123">Request body</span></span>
<span data-ttu-id="ac799-124">В тексте запроса добавьте представление объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac799-124">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="ac799-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="ac799-125">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="ac799-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac799-126">Property</span></span>|<span data-ttu-id="ac799-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ac799-127">Type</span></span>|<span data-ttu-id="ac799-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ac799-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac799-129">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="ac799-129">inGracePeriodCount</span></span>|<span data-ttu-id="ac799-130">Int32</span><span class="sxs-lookup"><span data-stu-id="ac799-130">Int32</span></span>|<span data-ttu-id="ac799-131">Количество устройств, для которых действует льготный период.</span><span class="sxs-lookup"><span data-stu-id="ac799-131">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="ac799-132">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="ac799-132">configManagerCount</span></span>|<span data-ttu-id="ac799-133">Int32</span><span class="sxs-lookup"><span data-stu-id="ac799-133">Int32</span></span>|<span data-ttu-id="ac799-134">Количество устройств, для которых System Center Configuration Manager управляет соответствием требованиям.</span><span class="sxs-lookup"><span data-stu-id="ac799-134">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="ac799-135">id</span><span class="sxs-lookup"><span data-stu-id="ac799-135">id</span></span>|<span data-ttu-id="ac799-136">Строка</span><span class="sxs-lookup"><span data-stu-id="ac799-136">String</span></span>|<span data-ttu-id="ac799-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ac799-137">Key of the entity.</span></span>|
|<span data-ttu-id="ac799-138">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ac799-138">unknownDeviceCount</span></span>|<span data-ttu-id="ac799-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ac799-139">Int32</span></span>|<span data-ttu-id="ac799-140">Количество неизвестных устройств.</span><span class="sxs-lookup"><span data-stu-id="ac799-140">Number of unknown devices</span></span>|
|<span data-ttu-id="ac799-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ac799-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="ac799-142">Int32</span><span class="sxs-lookup"><span data-stu-id="ac799-142">Int32</span></span>|<span data-ttu-id="ac799-143">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="ac799-143">Number of not applicable devices</span></span>|
|<span data-ttu-id="ac799-144">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ac799-144">compliantDeviceCount</span></span>|<span data-ttu-id="ac799-145">Int32</span><span class="sxs-lookup"><span data-stu-id="ac799-145">Int32</span></span>|<span data-ttu-id="ac799-146">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="ac799-146">Number of compliant devices</span></span>|
|<span data-ttu-id="ac799-147">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ac799-147">remediatedDeviceCount</span></span>|<span data-ttu-id="ac799-148">Int32</span><span class="sxs-lookup"><span data-stu-id="ac799-148">Int32</span></span>|<span data-ttu-id="ac799-149">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="ac799-149">Number of remediated devices</span></span>|
|<span data-ttu-id="ac799-150">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ac799-150">nonCompliantDeviceCount</span></span>|<span data-ttu-id="ac799-151">Int32</span><span class="sxs-lookup"><span data-stu-id="ac799-151">Int32</span></span>|<span data-ttu-id="ac799-152">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="ac799-152">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="ac799-153">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ac799-153">errorDeviceCount</span></span>|<span data-ttu-id="ac799-154">Int32</span><span class="sxs-lookup"><span data-stu-id="ac799-154">Int32</span></span>|<span data-ttu-id="ac799-155">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="ac799-155">Number of error devices</span></span>|
|<span data-ttu-id="ac799-156">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ac799-156">conflictDeviceCount</span></span>|<span data-ttu-id="ac799-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ac799-157">Int32</span></span>|<span data-ttu-id="ac799-158">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="ac799-158">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="ac799-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac799-159">Response</span></span>
<span data-ttu-id="ac799-160">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ac799-160">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac799-161">Пример</span><span class="sxs-lookup"><span data-stu-id="ac799-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="ac799-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac799-162">Request</span></span>
<span data-ttu-id="ac799-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac799-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicyDeviceStateSummary
Content-type: application/json
Content-length: 270

{
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="ac799-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="ac799-164">Response</span></span>
<span data-ttu-id="ac799-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ac799-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```








