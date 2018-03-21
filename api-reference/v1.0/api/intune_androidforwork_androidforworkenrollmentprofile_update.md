# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="1ea7b-101">Обновление объекта androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="1ea7b-101">Update androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="1ea7b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ea7b-103">Обновление свойств объекта [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="1ea7b-103">Update the properties of a [calendar](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ea7b-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1ea7b-104">Prerequisites</span></span>
<span data-ttu-id="1ea7b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1ea7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1ea7b-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ea7b-107">Permission type</span></span>|<span data-ttu-id="1ea7b-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ea7b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ea7b-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ea7b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1ea7b-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ea7b-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1ea7b-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ea7b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ea7b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-112">Not supported.</span></span>|
|<span data-ttu-id="1ea7b-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ea7b-113">Application</span></span>|<span data-ttu-id="1ea7b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ea7b-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ea7b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="1ea7b-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ea7b-116">Request headers</span></span>
|<span data-ttu-id="1ea7b-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ea7b-117">Header</span></span>|<span data-ttu-id="1ea7b-118">Значение</span><span class="sxs-lookup"><span data-stu-id="1ea7b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ea7b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ea7b-119">Authorization</span></span>|<span data-ttu-id="1ea7b-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1ea7b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1ea7b-121">Accept</span></span>|<span data-ttu-id="1ea7b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1ea7b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ea7b-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ea7b-123">Request body</span></span>
<span data-ttu-id="1ea7b-124">В тексте запроса добавьте представление объекта [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="1ea7b-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="1ea7b-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="1ea7b-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ea7b-126">Property</span></span>|<span data-ttu-id="1ea7b-127">Тип</span><span class="sxs-lookup"><span data-stu-id="1ea7b-127">Type</span></span>|<span data-ttu-id="1ea7b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="1ea7b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ea7b-129">accountId</span><span class="sxs-lookup"><span data-stu-id="1ea7b-129">accountId</span></span>|<span data-ttu-id="1ea7b-130">String</span><span class="sxs-lookup"><span data-stu-id="1ea7b-130">String</span></span>|<span data-ttu-id="1ea7b-131">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-131">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="1ea7b-132">id</span><span class="sxs-lookup"><span data-stu-id="1ea7b-132">id</span></span>|<span data-ttu-id="1ea7b-133">String</span><span class="sxs-lookup"><span data-stu-id="1ea7b-133">String</span></span>|<span data-ttu-id="1ea7b-134">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-134">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="1ea7b-135">name</span><span class="sxs-lookup"><span data-stu-id="1ea7b-135">name</span></span>|<span data-ttu-id="1ea7b-136">String</span><span class="sxs-lookup"><span data-stu-id="1ea7b-136">String</span></span>|<span data-ttu-id="1ea7b-137">(Нерекомендуемое) Отображаемое имя для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-137">(Deprecated) Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="1ea7b-138">displayName</span><span class="sxs-lookup"><span data-stu-id="1ea7b-138">displayName</span></span>|<span data-ttu-id="1ea7b-139">String</span><span class="sxs-lookup"><span data-stu-id="1ea7b-139">String</span></span>|<span data-ttu-id="1ea7b-140">Отображаемое имя для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="1ea7b-141">description</span><span class="sxs-lookup"><span data-stu-id="1ea7b-141">description</span></span>|<span data-ttu-id="1ea7b-142">String</span><span class="sxs-lookup"><span data-stu-id="1ea7b-142">String</span></span>|<span data-ttu-id="1ea7b-143">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="1ea7b-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ea7b-144">createdDateTime</span></span>|<span data-ttu-id="1ea7b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ea7b-145">DateTimeOffset</span></span>|<span data-ttu-id="1ea7b-146">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="1ea7b-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ea7b-147">modifiedDateTime</span></span>|<span data-ttu-id="1ea7b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ea7b-148">DateTimeOffset</span></span>|<span data-ttu-id="1ea7b-149">(Нерекомендуемое) Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-149">(Deprecated) Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="1ea7b-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ea7b-150">lastModifiedDateTime</span></span>|<span data-ttu-id="1ea7b-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ea7b-151">DateTimeOffset</span></span>|<span data-ttu-id="1ea7b-152">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-152">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="1ea7b-153">tokenValue</span><span class="sxs-lookup"><span data-stu-id="1ea7b-153">tokenValue</span></span>|<span data-ttu-id="1ea7b-154">String</span><span class="sxs-lookup"><span data-stu-id="1ea7b-154">String</span></span>|<span data-ttu-id="1ea7b-155">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-155">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="1ea7b-156">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1ea7b-156">tokenExpirationDateTime</span></span>|<span data-ttu-id="1ea7b-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ea7b-157">DateTimeOffset</span></span>|<span data-ttu-id="1ea7b-158">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-158">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="1ea7b-159">totalEnrollmentCount</span><span class="sxs-lookup"><span data-stu-id="1ea7b-159">totalEnrollmentCount</span></span>|<span data-ttu-id="1ea7b-160">Int32</span><span class="sxs-lookup"><span data-stu-id="1ea7b-160">Int32</span></span>|<span data-ttu-id="1ea7b-161">(Нерекомендуемое) Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-161">(Deprecated) Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="1ea7b-162">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1ea7b-162">enrolledDeviceCount</span></span>|<span data-ttu-id="1ea7b-163">Int32</span><span class="sxs-lookup"><span data-stu-id="1ea7b-163">Int32</span></span>|<span data-ttu-id="1ea7b-164">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-164">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="1ea7b-165">qrCode</span><span class="sxs-lookup"><span data-stu-id="1ea7b-165">qrCode</span></span>|<span data-ttu-id="1ea7b-166">String</span><span class="sxs-lookup"><span data-stu-id="1ea7b-166">String</span></span>|<span data-ttu-id="1ea7b-167">(Нерекомендуемое) Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-167">(Deprecated) String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="1ea7b-168">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="1ea7b-168">qrCodeContent</span></span>|<span data-ttu-id="1ea7b-169">String</span><span class="sxs-lookup"><span data-stu-id="1ea7b-169">String</span></span>|<span data-ttu-id="1ea7b-170">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-170">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="1ea7b-171">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="1ea7b-171">qrCodeImage</span></span>|[<span data-ttu-id="1ea7b-172">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1ea7b-172">mimeContent</span></span>](../resources/intune_androidforwork_mimecontent.md)|<span data-ttu-id="1ea7b-173">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-173">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="1ea7b-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ea7b-174">Response</span></span>
<span data-ttu-id="1ea7b-175">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-175">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ea7b-176">Пример</span><span class="sxs-lookup"><span data-stu-id="1ea7b-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ea7b-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ea7b-177">Request</span></span>
<span data-ttu-id="1ea7b-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
Content-type: application/json
Content-length: 575

{
  "accountId": "Account Id value",
  "name": "Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "totalEnrollmentCount": 4,
  "enrolledDeviceCount": 3,
  "qrCode": "Qr Code value",
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a><span data-ttu-id="1ea7b-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ea7b-179">Response</span></span>
<span data-ttu-id="1ea7b-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1ea7b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 813

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "e6742553-2553-e674-5325-74e6532574e6",
  "name": "Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "totalEnrollmentCount": 4,
  "enrolledDeviceCount": 3,
  "qrCode": "Qr Code value",
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```



