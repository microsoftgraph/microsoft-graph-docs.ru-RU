# <a name="create-devicemanagementpartner"></a><span data-ttu-id="ab8f7-101">Создание объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="ab8f7-101">Create deviceManagementPartner</span></span>

> <span data-ttu-id="ab8f7-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ab8f7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab8f7-103">Создание объекта [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="ab8f7-103">Create a new [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab8f7-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ab8f7-104">Prerequisites</span></span>
<span data-ttu-id="ab8f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ab8f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ab8f7-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab8f7-107">Permission type</span></span>|<span data-ttu-id="ab8f7-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab8f7-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab8f7-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab8f7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ab8f7-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab8f7-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ab8f7-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab8f7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab8f7-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab8f7-112">Not supported.</span></span>|
|<span data-ttu-id="ab8f7-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab8f7-113">Application</span></span>|<span data-ttu-id="ab8f7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab8f7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab8f7-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab8f7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="ab8f7-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab8f7-116">Request headers</span></span>
|<span data-ttu-id="ab8f7-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab8f7-117">Header</span></span>|<span data-ttu-id="ab8f7-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ab8f7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab8f7-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ab8f7-119">Authorization</span></span>|<span data-ttu-id="ab8f7-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="ab8f7-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab8f7-121">Принять</span><span class="sxs-lookup"><span data-stu-id="ab8f7-121">Accept</span></span>|<span data-ttu-id="ab8f7-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="ab8f7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab8f7-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ab8f7-123">Request body</span></span>
<span data-ttu-id="ab8f7-124">В теле запроса добавьте представление объекта deviceManagementPartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab8f7-124">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="ab8f7-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="ab8f7-125">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="ab8f7-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab8f7-126">Property</span></span>|<span data-ttu-id="ab8f7-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ab8f7-127">Type</span></span>|<span data-ttu-id="ab8f7-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ab8f7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab8f7-129">ИД</span><span class="sxs-lookup"><span data-stu-id="ab8f7-129">id</span></span>|<span data-ttu-id="ab8f7-130">Строка</span><span class="sxs-lookup"><span data-stu-id="ab8f7-130">String</span></span>|<span data-ttu-id="ab8f7-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ab8f7-131">Not yet documented</span></span>|
|<span data-ttu-id="ab8f7-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="ab8f7-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="ab8f7-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab8f7-133">DateTimeOffset</span></span>|<span data-ttu-id="ab8f7-134">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="ab8f7-134">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="ab8f7-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="ab8f7-135">partnerState</span></span>|[<span data-ttu-id="ab8f7-136">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="ab8f7-136">deviceManagementPartnerTenantState</span></span>](../resources/intune_onboarding_devicemanagementpartnertenantstate.md)|<span data-ttu-id="ab8f7-137">Состояние партнера этого клиента.</span><span class="sxs-lookup"><span data-stu-id="ab8f7-137">Partner state of this tenant Possible values are: , , , , , .</span></span> <span data-ttu-id="ab8f7-138">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="ab8f7-138">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="ab8f7-139">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="ab8f7-139">partnerAppType</span></span>|[<span data-ttu-id="ab8f7-140">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="ab8f7-140">deviceManagementPartnerAppType</span></span>](../resources/intune_onboarding_devicemanagementpartnerapptype.md)|<span data-ttu-id="ab8f7-141">Тип партнерского приложения.</span><span class="sxs-lookup"><span data-stu-id="ab8f7-141">Partner App Type.</span></span> <span data-ttu-id="ab8f7-142">Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="ab8f7-142">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="ab8f7-143">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="ab8f7-143">singleTenantAppId</span></span>|<span data-ttu-id="ab8f7-144">Строка</span><span class="sxs-lookup"><span data-stu-id="ab8f7-144">String</span></span>|<span data-ttu-id="ab8f7-145">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="ab8f7-145">Partner Single tenant App id</span></span>|
|<span data-ttu-id="ab8f7-146">displayName</span><span class="sxs-lookup"><span data-stu-id="ab8f7-146">displayName</span></span>|<span data-ttu-id="ab8f7-147">Строка</span><span class="sxs-lookup"><span data-stu-id="ab8f7-147">String</span></span>|<span data-ttu-id="ab8f7-148">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="ab8f7-148">Partner display name</span></span>|
|<span data-ttu-id="ab8f7-149">isConfigured</span><span class="sxs-lookup"><span data-stu-id="ab8f7-149">isConfigured</span></span>|<span data-ttu-id="ab8f7-150">Логический</span><span class="sxs-lookup"><span data-stu-id="ab8f7-150">Boolean</span></span>|<span data-ttu-id="ab8f7-151">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="ab8f7-151">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="ab8f7-152">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab8f7-152">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="ab8f7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab8f7-153">DateTimeOffset</span></span>|<span data-ttu-id="ab8f7-154">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства.</span><span class="sxs-lookup"><span data-stu-id="ab8f7-154">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="ab8f7-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="ab8f7-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="ab8f7-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab8f7-156">DateTimeOffset</span></span>|<span data-ttu-id="ab8f7-157">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям.</span><span class="sxs-lookup"><span data-stu-id="ab8f7-157">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="ab8f7-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab8f7-158">Response</span></span>
<span data-ttu-id="ab8f7-159">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ab8f7-159">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab8f7-160">Пример</span><span class="sxs-lookup"><span data-stu-id="ab8f7-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab8f7-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab8f7-161">Request</span></span>
<span data-ttu-id="ab8f7-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab8f7-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners
Content-type: application/json
Content-length: 502

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```

### <a name="response"></a><span data-ttu-id="ab8f7-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab8f7-163">Response</span></span>
<span data-ttu-id="ab8f7-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab8f7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 551

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```








