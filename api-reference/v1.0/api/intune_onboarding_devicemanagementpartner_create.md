# <a name="create-devicemanagementpartner"></a><span data-ttu-id="8ad19-101">Создание объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="8ad19-101">Create deviceManagementPartner</span></span>

> <span data-ttu-id="8ad19-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8ad19-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ad19-103">Создание объекта [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="8ad19-103">Create a new [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8ad19-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8ad19-104">Prerequisites</span></span>
<span data-ttu-id="8ad19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8ad19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8ad19-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ad19-107">Permission type</span></span>|<span data-ttu-id="8ad19-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ad19-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ad19-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ad19-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8ad19-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ad19-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8ad19-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ad19-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ad19-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ad19-112">Not supported.</span></span>|
|<span data-ttu-id="8ad19-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ad19-113">Application</span></span>|<span data-ttu-id="8ad19-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ad19-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ad19-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ad19-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="8ad19-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ad19-116">Request headers</span></span>
|<span data-ttu-id="8ad19-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ad19-117">Header</span></span>|<span data-ttu-id="8ad19-118">Значение</span><span class="sxs-lookup"><span data-stu-id="8ad19-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ad19-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ad19-119">Authorization</span></span>|<span data-ttu-id="8ad19-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ad19-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ad19-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8ad19-121">Accept</span></span>|<span data-ttu-id="8ad19-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8ad19-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ad19-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ad19-123">Request body</span></span>
<span data-ttu-id="8ad19-124">В теле запроса добавьте представление объекта deviceManagementPartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ad19-124">In the request body, supply a JSON representation for the deviceManagementPartner object.</span></span>

<span data-ttu-id="8ad19-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="8ad19-125">The following table shows the properties that are required when you create the deviceManagementPartner.</span></span>

|<span data-ttu-id="8ad19-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ad19-126">Property</span></span>|<span data-ttu-id="8ad19-127">Тип</span><span class="sxs-lookup"><span data-stu-id="8ad19-127">Type</span></span>|<span data-ttu-id="8ad19-128">Описание</span><span class="sxs-lookup"><span data-stu-id="8ad19-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ad19-129">id</span><span class="sxs-lookup"><span data-stu-id="8ad19-129">id</span></span>|<span data-ttu-id="8ad19-130">String</span><span class="sxs-lookup"><span data-stu-id="8ad19-130">String</span></span>|<span data-ttu-id="8ad19-131">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="8ad19-131">Not yet documented</span></span>|
|<span data-ttu-id="8ad19-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="8ad19-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="8ad19-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ad19-133">DateTimeOffset</span></span>|<span data-ttu-id="8ad19-134">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="8ad19-134">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="8ad19-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="8ad19-135">partnerState</span></span>|[<span data-ttu-id="8ad19-136">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="8ad19-136">deviceManagementPartnerTenantState</span></span>](../resources/intune_onboarding_devicemanagementpartnertenantstate.md)|<span data-ttu-id="8ad19-137">Состояние партнера клиента.</span><span class="sxs-lookup"><span data-stu-id="8ad19-137">Partner state of this tenant.</span></span> <span data-ttu-id="8ad19-138">Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="8ad19-138">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="8ad19-139">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="8ad19-139">partnerAppType</span></span>|[<span data-ttu-id="8ad19-140">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="8ad19-140">deviceManagementPartnerAppType</span></span>](../resources/intune_onboarding_devicemanagementpartnerapptype.md)|<span data-ttu-id="8ad19-141">Партнерские типа приложения.</span><span class="sxs-lookup"><span data-stu-id="8ad19-141">Partner App type.</span></span> <span data-ttu-id="8ad19-142">Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="8ad19-142">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="8ad19-143">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="8ad19-143">singleTenantAppId</span></span>|<span data-ttu-id="8ad19-144">String</span><span class="sxs-lookup"><span data-stu-id="8ad19-144">String</span></span>|<span data-ttu-id="8ad19-145">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="8ad19-145">Partner Single tenant App id</span></span>|
|<span data-ttu-id="8ad19-146">displayName</span><span class="sxs-lookup"><span data-stu-id="8ad19-146">displayName</span></span>|<span data-ttu-id="8ad19-147">String</span><span class="sxs-lookup"><span data-stu-id="8ad19-147">String</span></span>|<span data-ttu-id="8ad19-148">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="8ad19-148">Partner display name</span></span>|
|<span data-ttu-id="8ad19-149">isConfigured</span><span class="sxs-lookup"><span data-stu-id="8ad19-149">isConfigured</span></span>|<span data-ttu-id="8ad19-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ad19-150">Boolean</span></span>|<span data-ttu-id="8ad19-151">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="8ad19-151">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="8ad19-152">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ad19-152">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="8ad19-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ad19-153">DateTimeOffset</span></span>|<span data-ttu-id="8ad19-154">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства.</span><span class="sxs-lookup"><span data-stu-id="8ad19-154">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="8ad19-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="8ad19-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="8ad19-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ad19-156">DateTimeOffset</span></span>|<span data-ttu-id="8ad19-157">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям.</span><span class="sxs-lookup"><span data-stu-id="8ad19-157">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="8ad19-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ad19-158">Response</span></span>
<span data-ttu-id="8ad19-159">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8ad19-159">If successful, this method returns a `201 Created` response code and a [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ad19-160">Пример</span><span class="sxs-lookup"><span data-stu-id="8ad19-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="8ad19-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ad19-161">Request</span></span>
<span data-ttu-id="8ad19-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ad19-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8ad19-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="8ad19-163">Response</span></span>
<span data-ttu-id="8ad19-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8ad19-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



