# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="737ba-101">Обновить softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="737ba-101">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="737ba-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="737ba-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="737ba-103">Обновление свойств объекта [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="737ba-103">Update the properties of a [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="737ba-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="737ba-104">Prerequisites</span></span>
<span data-ttu-id="737ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="737ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="737ba-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="737ba-107">Permission type</span></span>|<span data-ttu-id="737ba-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="737ba-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="737ba-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="737ba-109">Delegated (work or school account)</span></span>|<span data-ttu-id="737ba-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="737ba-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="737ba-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="737ba-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="737ba-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="737ba-112">Not supported.</span></span>|
|<span data-ttu-id="737ba-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="737ba-113">Application</span></span>|<span data-ttu-id="737ba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="737ba-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="737ba-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="737ba-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="737ba-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="737ba-116">Request headers</span></span>
|<span data-ttu-id="737ba-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="737ba-117">Header</span></span>|<span data-ttu-id="737ba-118">Значение</span><span class="sxs-lookup"><span data-stu-id="737ba-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="737ba-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="737ba-119">Authorization</span></span>|<span data-ttu-id="737ba-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="737ba-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="737ba-121">Принять</span><span class="sxs-lookup"><span data-stu-id="737ba-121">Accept</span></span>|<span data-ttu-id="737ba-122">application/json</span><span class="sxs-lookup"><span data-stu-id="737ba-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="737ba-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="737ba-123">Request body</span></span>
<span data-ttu-id="737ba-124">В теле запроса добавьте представление объекта [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="737ba-124">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="737ba-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md).</span><span class="sxs-lookup"><span data-stu-id="737ba-125">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="737ba-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="737ba-126">Property</span></span>|<span data-ttu-id="737ba-127">Тип</span><span class="sxs-lookup"><span data-stu-id="737ba-127">Type</span></span>|<span data-ttu-id="737ba-128">Описание</span><span class="sxs-lookup"><span data-stu-id="737ba-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="737ba-129">id</span><span class="sxs-lookup"><span data-stu-id="737ba-129">id</span></span>|<span data-ttu-id="737ba-130">Строка</span><span class="sxs-lookup"><span data-stu-id="737ba-130">String</span></span>|<span data-ttu-id="737ba-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="737ba-131">Key of the entity.</span></span>|
|<span data-ttu-id="737ba-132">displayName</span><span class="sxs-lookup"><span data-stu-id="737ba-132">displayName</span></span>|<span data-ttu-id="737ba-133">String</span><span class="sxs-lookup"><span data-stu-id="737ba-133">String</span></span>|<span data-ttu-id="737ba-134">Имя политики.</span><span class="sxs-lookup"><span data-stu-id="737ba-134">The name of the policy.</span></span>|
|<span data-ttu-id="737ba-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="737ba-135">compliantDeviceCount</span></span>|<span data-ttu-id="737ba-136">Int32</span><span class="sxs-lookup"><span data-stu-id="737ba-136">Int32</span></span>|<span data-ttu-id="737ba-137">Количество устройств, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="737ba-137">Number of compliant devices.</span></span>|
|<span data-ttu-id="737ba-138">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="737ba-138">nonCompliantDeviceCount</span></span>|<span data-ttu-id="737ba-139">Int32</span><span class="sxs-lookup"><span data-stu-id="737ba-139">Int32</span></span>|<span data-ttu-id="737ba-140">Количество устройств, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="737ba-140">Number of non compliant devices.</span></span>|
|<span data-ttu-id="737ba-141">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="737ba-141">remediatedDeviceCount</span></span>|<span data-ttu-id="737ba-142">Int32</span><span class="sxs-lookup"><span data-stu-id="737ba-142">Int32</span></span>|<span data-ttu-id="737ba-143">Количество исправленных устройств.</span><span class="sxs-lookup"><span data-stu-id="737ba-143">Number of remediated devices.</span></span>|
|<span data-ttu-id="737ba-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="737ba-144">errorDeviceCount</span></span>|<span data-ttu-id="737ba-145">Int32</span><span class="sxs-lookup"><span data-stu-id="737ba-145">Int32</span></span>|<span data-ttu-id="737ba-146">Количество устройств с ошибками.</span><span class="sxs-lookup"><span data-stu-id="737ba-146">Number of devices had error.</span></span>|
|<span data-ttu-id="737ba-147">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="737ba-147">unknownDeviceCount</span></span>|<span data-ttu-id="737ba-148">Int32</span><span class="sxs-lookup"><span data-stu-id="737ba-148">Int32</span></span>|<span data-ttu-id="737ba-149">Количество неизвестных устройств</span><span class="sxs-lookup"><span data-stu-id="737ba-149">Number of unknown devices.</span></span>|
|<span data-ttu-id="737ba-150">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="737ba-150">conflictDeviceCount</span></span>|<span data-ttu-id="737ba-151">Int32</span><span class="sxs-lookup"><span data-stu-id="737ba-151">Int32</span></span>|<span data-ttu-id="737ba-152">Количество конфликтующих устройств.</span><span class="sxs-lookup"><span data-stu-id="737ba-152">Number of conflict devices.</span></span>|
|<span data-ttu-id="737ba-153">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="737ba-153">notApplicableDeviceCount</span></span>|<span data-ttu-id="737ba-154">Int32</span><span class="sxs-lookup"><span data-stu-id="737ba-154">Int32</span></span>|<span data-ttu-id="737ba-155">Количество неприменимых устройств.</span><span class="sxs-lookup"><span data-stu-id="737ba-155">Number of not applicable devices.</span></span>|
|<span data-ttu-id="737ba-156">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="737ba-156">compliantUserCount</span></span>|<span data-ttu-id="737ba-157">Int32</span><span class="sxs-lookup"><span data-stu-id="737ba-157">Int32</span></span>|<span data-ttu-id="737ba-158">Количество пользователей, соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="737ba-158">Number of compliant users.</span></span>|
|<span data-ttu-id="737ba-159">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="737ba-159">nonCompliantUserCount</span></span>|<span data-ttu-id="737ba-160">Int32</span><span class="sxs-lookup"><span data-stu-id="737ba-160">Int32</span></span>|<span data-ttu-id="737ba-161">Количество пользователей, не соответствующих требованиям.</span><span class="sxs-lookup"><span data-stu-id="737ba-161">Number of non compliant users.</span></span>|
|<span data-ttu-id="737ba-162">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="737ba-162">remediatedUserCount</span></span>|<span data-ttu-id="737ba-163">Int32</span><span class="sxs-lookup"><span data-stu-id="737ba-163">Int32</span></span>|<span data-ttu-id="737ba-164">Количество исправленных пользователей.</span><span class="sxs-lookup"><span data-stu-id="737ba-164">Number of remediated users.</span></span>|
|<span data-ttu-id="737ba-165">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="737ba-165">errorUserCount</span></span>|<span data-ttu-id="737ba-166">Int32</span><span class="sxs-lookup"><span data-stu-id="737ba-166">Int32</span></span>|<span data-ttu-id="737ba-167">Количество пользователей с ошибками.</span><span class="sxs-lookup"><span data-stu-id="737ba-167">Number of users had error.</span></span>|
|<span data-ttu-id="737ba-168">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="737ba-168">unknownUserCount</span></span>|<span data-ttu-id="737ba-169">Int32</span><span class="sxs-lookup"><span data-stu-id="737ba-169">Int32</span></span>|<span data-ttu-id="737ba-170">Количество неизвестных пользователей.</span><span class="sxs-lookup"><span data-stu-id="737ba-170">Number of unknown users.</span></span>|
|<span data-ttu-id="737ba-171">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="737ba-171">conflictUserCount</span></span>|<span data-ttu-id="737ba-172">Int32</span><span class="sxs-lookup"><span data-stu-id="737ba-172">Int32</span></span>|<span data-ttu-id="737ba-173">Количество конфликтующих пользователей.</span><span class="sxs-lookup"><span data-stu-id="737ba-173">Number of conflict users.</span></span>|
|<span data-ttu-id="737ba-174">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="737ba-174">notApplicableUserCount</span></span>|<span data-ttu-id="737ba-175">Int32</span><span class="sxs-lookup"><span data-stu-id="737ba-175">Int32</span></span>|<span data-ttu-id="737ba-176">Количество неприменимых пользователей.</span><span class="sxs-lookup"><span data-stu-id="737ba-176">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="737ba-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="737ba-177">Response</span></span>
<span data-ttu-id="737ba-178">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="737ba-178">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="737ba-179">Пример</span><span class="sxs-lookup"><span data-stu-id="737ba-179">Example</span></span>
### <a name="request"></a><span data-ttu-id="737ba-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="737ba-180">Request</span></span>
<span data-ttu-id="737ba-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="737ba-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
Content-type: application/json
Content-length: 452

{
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```

### <a name="response"></a><span data-ttu-id="737ba-182">Ответ</span><span class="sxs-lookup"><span data-stu-id="737ba-182">Response</span></span>
<span data-ttu-id="737ba-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="737ba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```








