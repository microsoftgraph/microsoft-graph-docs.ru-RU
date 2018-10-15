# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="12d93-101">Создание объекта mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="12d93-101">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="12d93-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="12d93-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12d93-103">Создание объекта [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="12d93-103">Create a new [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="12d93-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="12d93-104">Prerequisites</span></span>
<span data-ttu-id="12d93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="12d93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="12d93-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12d93-107">Permission type</span></span>|<span data-ttu-id="12d93-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12d93-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12d93-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12d93-109">Delegated (work or school account)</span></span>|<span data-ttu-id="12d93-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12d93-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="12d93-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12d93-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12d93-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12d93-112">Not supported.</span></span>|
|<span data-ttu-id="12d93-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12d93-113">Application</span></span>|<span data-ttu-id="12d93-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12d93-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12d93-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12d93-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="12d93-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12d93-116">Request headers</span></span>
|<span data-ttu-id="12d93-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12d93-117">Header</span></span>|<span data-ttu-id="12d93-118">Значение</span><span class="sxs-lookup"><span data-stu-id="12d93-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12d93-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12d93-119">Authorization</span></span>|<span data-ttu-id="12d93-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="12d93-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12d93-121">Принять</span><span class="sxs-lookup"><span data-stu-id="12d93-121">Accept</span></span>|<span data-ttu-id="12d93-122">приложение/json</span><span class="sxs-lookup"><span data-stu-id="12d93-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12d93-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12d93-123">Request body</span></span>
<span data-ttu-id="12d93-124">В тексте запроса добавьте представление объекта mobileThreatDefenseConnector в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12d93-124">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="12d93-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="12d93-125">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="12d93-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="12d93-126">Property</span></span>|<span data-ttu-id="12d93-127">Тип</span><span class="sxs-lookup"><span data-stu-id="12d93-127">Type</span></span>|<span data-ttu-id="12d93-128">Описание</span><span class="sxs-lookup"><span data-stu-id="12d93-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12d93-129">ИД</span><span class="sxs-lookup"><span data-stu-id="12d93-129">id</span></span>|<span data-ttu-id="12d93-130">string</span><span class="sxs-lookup"><span data-stu-id="12d93-130">String</span></span>|<span data-ttu-id="12d93-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="12d93-131">Not yet documented</span></span>|
|<span data-ttu-id="12d93-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="12d93-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="12d93-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12d93-133">DateTimeOffset</span></span>|<span data-ttu-id="12d93-134">Дата и время последнего подтверждения соединения, полученные от партнера по синхронизации данных</span><span class="sxs-lookup"><span data-stu-id="12d93-134">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="12d93-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="12d93-135">partnerState</span></span>|[<span data-ttu-id="12d93-136">mobileThreatPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="12d93-136">mobileThreatPartnerTenantState</span></span>](../resources/intune_onboarding_mobilethreatpartnertenantstate.md)|<span data-ttu-id="12d93-p102">Состояние партнера по синхронизации данных для этой учетной записи. Возможные значения: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="12d93-p102">Data Sync Partner state for this account Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="12d93-139">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="12d93-139">androidEnabled</span></span>|<span data-ttu-id="12d93-140">Логическое</span><span class="sxs-lookup"><span data-stu-id="12d93-140">Boolean</span></span>|<span data-ttu-id="12d93-141">Для ОС Android следует указать, необходимо ли использовать данные партнера по синхронизации данных в ходе оценки соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="12d93-141">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="12d93-142">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="12d93-142">iosEnabled</span></span>|<span data-ttu-id="12d93-143">Логическое</span><span class="sxs-lookup"><span data-stu-id="12d93-143">Boolean</span></span>|<span data-ttu-id="12d93-144">Для ОС IOS следует указать, использовать ли данные партнера по синхронизации данных в ходе оценок соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="12d93-144">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="12d93-145">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="12d93-145">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="12d93-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="12d93-146">Boolean</span></span>|<span data-ttu-id="12d93-147">Для ОС Android следует указать, получать ли Intune данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="12d93-147">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="12d93-148">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="12d93-148">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="12d93-149">Логическое</span><span class="sxs-lookup"><span data-stu-id="12d93-149">Boolean</span></span>|<span data-ttu-id="12d93-150">Для ОС IOS следует указать, получать ли Intune данные от партнера по синхронизации данных, прежде чем отметить устройство как соответствующее требованиям</span><span class="sxs-lookup"><span data-stu-id="12d93-150">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="12d93-151">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="12d93-151">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="12d93-152">Логическое</span><span class="sxs-lookup"><span data-stu-id="12d93-152">Boolean</span></span>|<span data-ttu-id="12d93-153">Получение или задание настроек, следует ли на включенных платформах блокировать устройства, которые не соответствуют минимальным требованиям партнера по синхронизации данных к версии</span><span class="sxs-lookup"><span data-stu-id="12d93-153">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="12d93-154">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="12d93-154">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="12d93-155">Int32</span><span class="sxs-lookup"><span data-stu-id="12d93-155">Int32</span></span>|<span data-ttu-id="12d93-156">Получает или задает количество дней устойчивости к отсутствию отклика для клиента при этой интеграции партнера.</span><span class="sxs-lookup"><span data-stu-id="12d93-156">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="12d93-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="12d93-157">Response</span></span>
<span data-ttu-id="12d93-158">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="12d93-158">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12d93-159">Пример</span><span class="sxs-lookup"><span data-stu-id="12d93-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="12d93-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="12d93-160">Request</span></span>
<span data-ttu-id="12d93-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12d93-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
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

### <a name="response"></a><span data-ttu-id="12d93-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="12d93-162">Response</span></span>
<span data-ttu-id="12d93-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12d93-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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








