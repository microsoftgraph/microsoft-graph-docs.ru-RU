# <a name="update-devicemanagementpartner"></a><span data-ttu-id="5605e-101">Обновление объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="5605e-101">Update deviceManagementPartner</span></span>

> <span data-ttu-id="5605e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5605e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5605e-103">Обновление свойств объекта [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="5605e-103">Update the properties of a [calendar](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5605e-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5605e-104">Prerequisites</span></span>
<span data-ttu-id="5605e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="5605e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5605e-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5605e-107">Permission type</span></span>|<span data-ttu-id="5605e-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5605e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5605e-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5605e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5605e-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5605e-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5605e-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5605e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5605e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5605e-112">Not supported.</span></span>|
|<span data-ttu-id="5605e-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5605e-113">Application</span></span>|<span data-ttu-id="5605e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5605e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5605e-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5605e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="5605e-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5605e-116">Request headers</span></span>
|<span data-ttu-id="5605e-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5605e-117">Header</span></span>|<span data-ttu-id="5605e-118">Значение</span><span class="sxs-lookup"><span data-stu-id="5605e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5605e-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5605e-119">Authorization</span></span>|<span data-ttu-id="5605e-120">&lt;Токен&gt; носителя. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5605e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5605e-121">Принять</span><span class="sxs-lookup"><span data-stu-id="5605e-121">Accept</span></span>|<span data-ttu-id="5605e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5605e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5605e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5605e-123">Request body</span></span>
<span data-ttu-id="5605e-124">В теле запроса добавьте представление объекта [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5605e-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="5605e-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="5605e-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="5605e-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="5605e-126">Property</span></span>|<span data-ttu-id="5605e-127">Тип</span><span class="sxs-lookup"><span data-stu-id="5605e-127">Type</span></span>|<span data-ttu-id="5605e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="5605e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5605e-129">id</span><span class="sxs-lookup"><span data-stu-id="5605e-129">id</span></span>|<span data-ttu-id="5605e-130">String</span><span class="sxs-lookup"><span data-stu-id="5605e-130">String</span></span>|<span data-ttu-id="5605e-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5605e-131">Not yet documented</span></span>|
|<span data-ttu-id="5605e-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="5605e-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="5605e-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5605e-133">DateTimeOffset</span></span>|<span data-ttu-id="5605e-134">Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".</span><span class="sxs-lookup"><span data-stu-id="5605e-134">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="5605e-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="5605e-135">partnerState</span></span>|<span data-ttu-id="5605e-136">String</span><span class="sxs-lookup"><span data-stu-id="5605e-136">String</span></span>|<span data-ttu-id="5605e-137">Состояние партнера этого клиента. Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="5605e-137">Partner state of this tenant Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="5605e-138">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="5605e-138">partnerAppType</span></span>|<span data-ttu-id="5605e-139">String</span><span class="sxs-lookup"><span data-stu-id="5605e-139">String</span></span>|<span data-ttu-id="5605e-140">Тип приложения партнера. Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.</span><span class="sxs-lookup"><span data-stu-id="5605e-140">Partner App type Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="5605e-141">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="5605e-141">singleTenantAppId</span></span>|<span data-ttu-id="5605e-142">String</span><span class="sxs-lookup"><span data-stu-id="5605e-142">String</span></span>|<span data-ttu-id="5605e-143">Идентификатор одноклиентского приложения партнера</span><span class="sxs-lookup"><span data-stu-id="5605e-143">Partner Single tenant App id</span></span>|
|<span data-ttu-id="5605e-144">displayName</span><span class="sxs-lookup"><span data-stu-id="5605e-144">displayName</span></span>|<span data-ttu-id="5605e-145">String</span><span class="sxs-lookup"><span data-stu-id="5605e-145">String</span></span>|<span data-ttu-id="5605e-146">Отображаемое имя партнера</span><span class="sxs-lookup"><span data-stu-id="5605e-146">Partner display name</span></span>|
|<span data-ttu-id="5605e-147">isConfigured</span><span class="sxs-lookup"><span data-stu-id="5605e-147">isConfigured</span></span>|<span data-ttu-id="5605e-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="5605e-148">Boolean</span></span>|<span data-ttu-id="5605e-149">Указывает, настроен ли партнер по управлению устройствами</span><span class="sxs-lookup"><span data-stu-id="5605e-149">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="5605e-150">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="5605e-150">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="5605e-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5605e-151">DateTimeOffset</span></span>|<span data-ttu-id="5605e-152">Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства</span><span class="sxs-lookup"><span data-stu-id="5605e-152">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="5605e-153">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="5605e-153">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="5605e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5605e-154">DateTimeOffset</span></span>|<span data-ttu-id="5605e-155">Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям</span><span class="sxs-lookup"><span data-stu-id="5605e-155">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="5605e-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="5605e-156">Response</span></span>
<span data-ttu-id="5605e-157">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5605e-157">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5605e-158">Пример</span><span class="sxs-lookup"><span data-stu-id="5605e-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="5605e-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="5605e-159">Request</span></span>
<span data-ttu-id="5605e-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5605e-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 440

{
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

### <a name="response"></a><span data-ttu-id="5605e-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="5605e-161">Response</span></span>
<span data-ttu-id="5605e-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5605e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



