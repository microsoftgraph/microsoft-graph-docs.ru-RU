# <a name="create-devicemanagementpartner"></a><span data-ttu-id="5e955-101">Создание объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="5e955-101">Create deviceManagementPartner</span></span>

> <span data-ttu-id="5e955-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5e955-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e955-103">Создание объекта [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="5e955-103">Create a new [plannerBucket](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5e955-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5e955-104">Prerequisites</span></span>
<span data-ttu-id="5e955-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5e955-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5e955-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e955-107">Permission type</span></span>|<span data-ttu-id="5e955-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e955-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e955-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e955-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5e955-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e955-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5e955-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e955-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e955-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e955-112">Not supported.</span></span>|
|<span data-ttu-id="5e955-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e955-113">Application</span></span>|<span data-ttu-id="5e955-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e955-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e955-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e955-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="5e955-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e955-116">Request headers</span></span>
|<span data-ttu-id="5e955-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e955-117">Header</span></span>|<span data-ttu-id="5e955-118">Значение</span><span class="sxs-lookup"><span data-stu-id="5e955-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e955-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e955-119">Authorization</span></span>|<span data-ttu-id="5e955-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e955-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5e955-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5e955-121">Accept</span></span>|<span data-ttu-id="5e955-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5e955-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e955-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5e955-123">Request body</span></span>
<span data-ttu-id="5e955-124">В теле запроса добавьте представление объекта deviceManagementPartner в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e955-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="5e955-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceManagementPartner.</span><span class="sxs-lookup"><span data-stu-id="5e955-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="5e955-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e955-126">Property</span></span>|<span data-ttu-id="5e955-127">Тип</span><span class="sxs-lookup"><span data-stu-id="5e955-127">Type</span></span>|<span data-ttu-id="5e955-128">Описание</span><span class="sxs-lookup"><span data-stu-id="5e955-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e955-129">id</span><span class="sxs-lookup"><span data-stu-id="5e955-129">id</span></span>|<span data-ttu-id="5e955-130">String</span><span class="sxs-lookup"><span data-stu-id="5e955-130">String</span></span>|<span data-ttu-id="5e955-131">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="5e955-131">Not yet documented</span></span>|
|<span data-ttu-id="5e955-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="5e955-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="5e955-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e955-133">DateTimeOffset</span></span>|<span data-ttu-id="5e955-134">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="5e955-134">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="5e955-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="5e955-135">partnerState</span></span>|<span data-ttu-id="5e955-136">String</span><span class="sxs-lookup"><span data-stu-id="5e955-136">String</span></span>|<span data-ttu-id="5e955-137">Состояние партнера этого клиента. Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="5e955-137">Partner state of this tenant Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="5e955-138">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="5e955-138">partnerAppType</span></span>|<span data-ttu-id="5e955-139">String</span><span class="sxs-lookup"><span data-stu-id="5e955-139">String</span></span>|<span data-ttu-id="5e955-140">Тип приложения партнера. Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="5e955-140">Partner App type Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="5e955-141">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="5e955-141">singleTenantAppId</span></span>|<span data-ttu-id="5e955-142">String</span><span class="sxs-lookup"><span data-stu-id="5e955-142">String</span></span>|<span data-ttu-id="5e955-143">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="5e955-143">Partner Single tenant App id</span></span>|
|<span data-ttu-id="5e955-144">displayName</span><span class="sxs-lookup"><span data-stu-id="5e955-144">displayName</span></span>|<span data-ttu-id="5e955-145">String</span><span class="sxs-lookup"><span data-stu-id="5e955-145">String</span></span>|<span data-ttu-id="5e955-146">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="5e955-146">Partner display name</span></span>|
|<span data-ttu-id="5e955-147">isConfigured</span><span class="sxs-lookup"><span data-stu-id="5e955-147">isConfigured</span></span>|<span data-ttu-id="5e955-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e955-148">Boolean</span></span>|<span data-ttu-id="5e955-149">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="5e955-149">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="5e955-150">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e955-150">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="5e955-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e955-151">DateTimeOffset</span></span>|<span data-ttu-id="5e955-152">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства.</span><span class="sxs-lookup"><span data-stu-id="5e955-152">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="5e955-153">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="5e955-153">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="5e955-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e955-154">DateTimeOffset</span></span>|<span data-ttu-id="5e955-155">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям.</span><span class="sxs-lookup"><span data-stu-id="5e955-155">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="5e955-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e955-156">Response</span></span>
<span data-ttu-id="5e955-157">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5e955-157">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_onboarding_devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e955-158">Пример</span><span class="sxs-lookup"><span data-stu-id="5e955-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="5e955-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e955-159">Request</span></span>
<span data-ttu-id="5e955-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e955-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5e955-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e955-161">Response</span></span>
<span data-ttu-id="5e955-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5e955-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



