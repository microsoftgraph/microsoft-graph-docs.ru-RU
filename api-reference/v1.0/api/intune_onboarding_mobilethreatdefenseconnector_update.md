# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="b4136-101">Обновление mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="b4136-101">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="b4136-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b4136-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4136-103">Обновление свойств объекта [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="b4136-103">Update the properties of a [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4136-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b4136-104">Prerequisites</span></span>
<span data-ttu-id="b4136-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b4136-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b4136-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4136-107">Permission type</span></span>|<span data-ttu-id="b4136-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4136-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4136-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4136-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b4136-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4136-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b4136-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4136-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4136-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4136-112">Not supported.</span></span>|
|<span data-ttu-id="b4136-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4136-113">Application</span></span>|<span data-ttu-id="b4136-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4136-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4136-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4136-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="b4136-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b4136-116">Request headers</span></span>
|<span data-ttu-id="b4136-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4136-117">Header</span></span>|<span data-ttu-id="b4136-118">Значение</span><span class="sxs-lookup"><span data-stu-id="b4136-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4136-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4136-119">Authorization</span></span>|<span data-ttu-id="b4136-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4136-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4136-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b4136-121">Accept</span></span>|<span data-ttu-id="b4136-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b4136-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4136-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b4136-123">Request body</span></span>
<span data-ttu-id="b4136-124">В теле запроса добавьте представление объекта [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4136-124">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="b4136-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="b4136-125">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="b4136-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4136-126">Property</span></span>|<span data-ttu-id="b4136-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b4136-127">Type</span></span>|<span data-ttu-id="b4136-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b4136-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4136-129">id</span><span class="sxs-lookup"><span data-stu-id="b4136-129">id</span></span>|<span data-ttu-id="b4136-130">String</span><span class="sxs-lookup"><span data-stu-id="b4136-130">String</span></span>|<span data-ttu-id="b4136-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="b4136-131">Not yet documented</span></span>|
|<span data-ttu-id="b4136-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="b4136-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="b4136-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4136-133">DateTimeOffset</span></span>|<span data-ttu-id="b4136-134">Дата и время последнего подтверждения соединения, полученные от партнера по синхронизации данных</span><span class="sxs-lookup"><span data-stu-id="b4136-134">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="b4136-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="b4136-135">partnerState</span></span>|<span data-ttu-id="b4136-136">String</span><span class="sxs-lookup"><span data-stu-id="b4136-136">String</span></span>|<span data-ttu-id="b4136-137">Возможные значения состояния партнера по синхронизации данных для этой учетной записи: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="b4136-137">Data Sync Partner state for this account Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="b4136-138">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="b4136-138">androidEnabled</span></span>|<span data-ttu-id="b4136-139">Логическое</span><span class="sxs-lookup"><span data-stu-id="b4136-139">Boolean</span></span>|<span data-ttu-id="b4136-140">Для ОС Android следует указать в настройках, необходимо ли использовать данные партнера по синхронизации данных в ходе оценки соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="b4136-140">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="b4136-141">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="b4136-141">iosEnabled</span></span>|<span data-ttu-id="b4136-142">Логическое</span><span class="sxs-lookup"><span data-stu-id="b4136-142">Boolean</span></span>|<span data-ttu-id="b4136-143">Для ОС IOS следует получить или задать настройки, необходимо ли использовать данные партнера по синхронизации данных в ходе оценок соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="b4136-143">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="b4136-144">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="b4136-144">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="b4136-145">Логическое</span><span class="sxs-lookup"><span data-stu-id="b4136-145">Boolean</span></span>|<span data-ttu-id="b4136-146">Для ОС Android следует указать, необходимо ли Intune получать данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="b4136-146">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="b4136-147">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="b4136-147">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="b4136-148">Логическое</span><span class="sxs-lookup"><span data-stu-id="b4136-148">Boolean</span></span>|<span data-ttu-id="b4136-149">Для ОС IOS следует указать, необходимо ли Intune получать данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="b4136-149">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="b4136-150">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="b4136-150">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="b4136-151">Логическое</span><span class="sxs-lookup"><span data-stu-id="b4136-151">Boolean</span></span>|<span data-ttu-id="b4136-152">Получение или задание настроек, следует ли блокировать устройства на включенных платформах, которые не соответствуют минимальным требованиям к версии партнера по синхронизации данных</span><span class="sxs-lookup"><span data-stu-id="b4136-152">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="b4136-153">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="b4136-153">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="b4136-154">Int32</span><span class="sxs-lookup"><span data-stu-id="b4136-154">Int32</span></span>|<span data-ttu-id="b4136-155">Получает или задает количество дней устойчивости к отсутствию отклика для клиента при этой интеграции партнера.</span><span class="sxs-lookup"><span data-stu-id="b4136-155">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="b4136-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4136-156">Response</span></span>
<span data-ttu-id="b4136-157">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b4136-157">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4136-158">Пример</span><span class="sxs-lookup"><span data-stu-id="b4136-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4136-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4136-159">Request</span></span>
<span data-ttu-id="b4136-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4136-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 347

{
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a><span data-ttu-id="b4136-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4136-161">Response</span></span>
<span data-ttu-id="b4136-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b4136-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 463

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```



