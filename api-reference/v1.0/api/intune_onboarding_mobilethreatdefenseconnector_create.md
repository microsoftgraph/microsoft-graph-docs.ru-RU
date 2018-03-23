# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="af163-101">Создание объекта mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="af163-101">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="af163-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="af163-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af163-103">Создание объекта [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).</span><span class="sxs-lookup"><span data-stu-id="af163-103">Create a new [plannerBucket](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af163-104">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="af163-104">Prerequisites</span></span>
<span data-ttu-id="af163-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="af163-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="af163-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af163-107">Permission type</span></span>|<span data-ttu-id="af163-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af163-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af163-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af163-109">Delegated (work or school account)</span></span>|<span data-ttu-id="af163-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af163-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="af163-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af163-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af163-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af163-112">Not supported.</span></span>|
|<span data-ttu-id="af163-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af163-113">Application</span></span>|<span data-ttu-id="af163-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af163-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af163-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af163-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="af163-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af163-116">Request headers</span></span>
|<span data-ttu-id="af163-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af163-117">Header</span></span>|<span data-ttu-id="af163-118">Значение</span><span class="sxs-lookup"><span data-stu-id="af163-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af163-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="af163-119">Authorization</span></span>|<span data-ttu-id="af163-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af163-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="af163-121">Accept</span><span class="sxs-lookup"><span data-stu-id="af163-121">Accept</span></span>|<span data-ttu-id="af163-122">application/json</span><span class="sxs-lookup"><span data-stu-id="af163-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af163-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af163-123">Request body</span></span>
<span data-ttu-id="af163-124">В тексте запроса добавьте представление объекта mobileThreatDefenseConnector в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af163-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="af163-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileThreatDefenseConnector.</span><span class="sxs-lookup"><span data-stu-id="af163-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="af163-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="af163-126">Property</span></span>|<span data-ttu-id="af163-127">Тип</span><span class="sxs-lookup"><span data-stu-id="af163-127">Type</span></span>|<span data-ttu-id="af163-128">Описание</span><span class="sxs-lookup"><span data-stu-id="af163-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af163-129">id</span><span class="sxs-lookup"><span data-stu-id="af163-129">id</span></span>|<span data-ttu-id="af163-130">String</span><span class="sxs-lookup"><span data-stu-id="af163-130">String</span></span>|<span data-ttu-id="af163-131">Н/Д</span><span class="sxs-lookup"><span data-stu-id="af163-131">Not yet documented</span></span>|
|<span data-ttu-id="af163-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="af163-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="af163-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af163-133">DateTimeOffset</span></span>|<span data-ttu-id="af163-134">Метка времени последнего полученного пакета пульса после того, как администратор включил параметр "Подключиться к MTP".</span><span class="sxs-lookup"><span data-stu-id="af163-134">Timestamp of last heartbeat after admin enabled option Connect to MTP</span></span>|
|<span data-ttu-id="af163-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="af163-135">partnerState</span></span>|<span data-ttu-id="af163-136">String</span><span class="sxs-lookup"><span data-stu-id="af163-136">String</span></span>|<span data-ttu-id="af163-137">Состояние партнера этого клиента. Возможные значения: `unavailable`, `available`, `enabled`, `unresponsive`.</span><span class="sxs-lookup"><span data-stu-id="af163-137">Partner state of this tenant Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="af163-138">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="af163-138">androidEnabled</span></span>|<span data-ttu-id="af163-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="af163-139">Boolean</span></span>|<span data-ttu-id="af163-140">Включение или отключение Android.</span><span class="sxs-lookup"><span data-stu-id="af163-140">Android Toggle On or Off</span></span>|
|<span data-ttu-id="af163-141">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="af163-141">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="af163-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="af163-142">Boolean</span></span>|<span data-ttu-id="af163-143">Для Android. Позволяет администратору настроить получение обязательных данных от партнера по синхронизации, прежде чем подтвердить соответствие требованиям.</span><span class="sxs-lookup"><span data-stu-id="af163-143">For Android, Allows admin to config must receive data from the data sync partner prior to being considered compliant</span></span>|
|<span data-ttu-id="af163-144">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="af163-144">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="af163-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="af163-145">Boolean</span></span>|<span data-ttu-id="af163-146">Для IOS. Позволяет администратору настроить получение обязательных данных от партнера по синхронизации, прежде чем подтвердить соответствие требованиям.</span><span class="sxs-lookup"><span data-stu-id="af163-146">For IOS, Allows admin to config must receive data from the data sync partner prior to being considered compliant</span></span>|
|<span data-ttu-id="af163-147">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="af163-147">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="af163-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="af163-148">Boolean</span></span>|<span data-ttu-id="af163-149">Позволяет администратору блокировать на включенных платформах устройства, несоответствующие минимальным требованиям для версии.</span><span class="sxs-lookup"><span data-stu-id="af163-149">Allows admin to block devices on the enabled platforms that do not meet minimum version requirements</span></span>|
|<span data-ttu-id="af163-150">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="af163-150">iosEnabled</span></span>|<span data-ttu-id="af163-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="af163-151">Boolean</span></span>|<span data-ttu-id="af163-152">Включение и отключение IOS.</span><span class="sxs-lookup"><span data-stu-id="af163-152">IOS Toggle On or Off</span></span>|
|<span data-ttu-id="af163-153">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="af163-153">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="af163-154">Int32</span><span class="sxs-lookup"><span data-stu-id="af163-154">Int32</span></span>|<span data-ttu-id="af163-155">Получает или задает количество дней устойчивости к отсутствию отклика для клиента при этой интеграции партнера.</span><span class="sxs-lookup"><span data-stu-id="af163-155">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="af163-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="af163-156">Response</span></span>
<span data-ttu-id="af163-157">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="af163-157">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af163-158">Пример</span><span class="sxs-lookup"><span data-stu-id="af163-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="af163-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="af163-159">Request</span></span>
<span data-ttu-id="af163-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af163-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a><span data-ttu-id="af163-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="af163-161">Response</span></span>
<span data-ttu-id="af163-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="af163-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```



