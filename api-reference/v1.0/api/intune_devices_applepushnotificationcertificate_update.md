# <a name="update-applepushnotificationcertificate"></a><span data-ttu-id="c45cd-101">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="c45cd-101">Update applePushNotificationCertificate</span></span>

> <span data-ttu-id="c45cd-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c45cd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c45cd-103">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="c45cd-103">Update the properties of a [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c45cd-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c45cd-104">Prerequisites</span></span>
<span data-ttu-id="c45cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c45cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c45cd-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c45cd-107">Permission type</span></span>|<span data-ttu-id="c45cd-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c45cd-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c45cd-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c45cd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c45cd-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c45cd-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c45cd-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c45cd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c45cd-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c45cd-112">Not supported.</span></span>|
|<span data-ttu-id="c45cd-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c45cd-113">Application</span></span>|<span data-ttu-id="c45cd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c45cd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c45cd-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c45cd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/applePushNotificationCertificate
```

## <a name="request-headers"></a><span data-ttu-id="c45cd-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c45cd-116">Request headers</span></span>
|<span data-ttu-id="c45cd-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c45cd-117">Header</span></span>|<span data-ttu-id="c45cd-118">Значение</span><span class="sxs-lookup"><span data-stu-id="c45cd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c45cd-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c45cd-119">Authorization</span></span>|<span data-ttu-id="c45cd-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="c45cd-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c45cd-121">Принять</span><span class="sxs-lookup"><span data-stu-id="c45cd-121">Accept</span></span>|<span data-ttu-id="c45cd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c45cd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c45cd-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c45cd-123">Request body</span></span>
<span data-ttu-id="c45cd-124">В теле запроса добавьте представление объекта [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c45cd-124">In the request body, supply a JSON representation for the [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>

<span data-ttu-id="c45cd-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="c45cd-125">The following table shows the properties that are required when you create the [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).</span></span>

|<span data-ttu-id="c45cd-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="c45cd-126">Property</span></span>|<span data-ttu-id="c45cd-127">Тип</span><span class="sxs-lookup"><span data-stu-id="c45cd-127">Type</span></span>|<span data-ttu-id="c45cd-128">Описание</span><span class="sxs-lookup"><span data-stu-id="c45cd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c45cd-129">id</span><span class="sxs-lookup"><span data-stu-id="c45cd-129">id</span></span>|<span data-ttu-id="c45cd-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="c45cd-130">String</span></span>|<span data-ttu-id="c45cd-131">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="c45cd-131">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="c45cd-132">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="c45cd-132">appleIdentifier</span></span>|<span data-ttu-id="c45cd-133">String (строка)</span><span class="sxs-lookup"><span data-stu-id="c45cd-133">String</span></span>|<span data-ttu-id="c45cd-134">Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="c45cd-134">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="c45cd-135">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="c45cd-135">topicIdentifier</span></span>|<span data-ttu-id="c45cd-136">String (строка)</span><span class="sxs-lookup"><span data-stu-id="c45cd-136">String</span></span>|<span data-ttu-id="c45cd-137">Идентификатор темы.</span><span class="sxs-lookup"><span data-stu-id="c45cd-137">Topic Id.</span></span>|
|<span data-ttu-id="c45cd-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c45cd-138">lastModifiedDateTime</span></span>|<span data-ttu-id="c45cd-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c45cd-139">DateTimeOffset</span></span>|<span data-ttu-id="c45cd-140">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="c45cd-140">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="c45cd-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c45cd-141">expirationDateTime</span></span>|<span data-ttu-id="c45cd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c45cd-142">DateTimeOffset</span></span>|<span data-ttu-id="c45cd-143">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="c45cd-143">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="c45cd-144">certificate</span><span class="sxs-lookup"><span data-stu-id="c45cd-144">certificate</span></span>|<span data-ttu-id="c45cd-145">String (строка)</span><span class="sxs-lookup"><span data-stu-id="c45cd-145">String</span></span>|<span data-ttu-id="c45cd-146">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c45cd-146">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c45cd-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="c45cd-147">Response</span></span>
<span data-ttu-id="c45cd-148">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c45cd-148">If successful, this method returns a `200 OK` response code and an updated [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c45cd-149">Пример</span><span class="sxs-lookup"><span data-stu-id="c45cd-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="c45cd-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="c45cd-150">Request</span></span>
<span data-ttu-id="c45cd-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c45cd-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/applePushNotificationCertificate
Content-type: application/json
Content-length: 264

{
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```

### <a name="response"></a><span data-ttu-id="c45cd-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="c45cd-152">Response</span></span>
<span data-ttu-id="c45cd-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c45cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 384

{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "c4c8f047-f047-c4c8-47f0-c8c447f0c8c4",
  "appleIdentifier": "Apple Identifier value",
  "topicIdentifier": "Topic Identifier value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "certificate": "Certificate value"
}
```








