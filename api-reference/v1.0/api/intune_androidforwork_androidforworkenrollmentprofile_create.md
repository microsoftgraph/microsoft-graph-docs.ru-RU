# <a name="create-androidforworkenrollmentprofile"></a><span data-ttu-id="1cd4a-101">Create androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="1cd4a-101">Create androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="1cd4a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1cd4a-103">Создание объекта [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="1cd4a-103">Create a new [plannerBucket](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1cd4a-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1cd4a-104">Prerequisites</span></span>
<span data-ttu-id="1cd4a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1cd4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1cd4a-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cd4a-107">Permission type</span></span>|<span data-ttu-id="1cd4a-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cd4a-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cd4a-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cd4a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1cd4a-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cd4a-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1cd4a-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cd4a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cd4a-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-112">Not supported.</span></span>|
|<span data-ttu-id="1cd4a-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1cd4a-113">Application</span></span>|<span data-ttu-id="1cd4a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cd4a-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cd4a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="1cd4a-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1cd4a-116">Request headers</span></span>
|<span data-ttu-id="1cd4a-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1cd4a-117">Header</span></span>|<span data-ttu-id="1cd4a-118">Значение</span><span class="sxs-lookup"><span data-stu-id="1cd4a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cd4a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cd4a-119">Authorization</span></span>|<span data-ttu-id="1cd4a-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1cd4a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1cd4a-121">Accept</span></span>|<span data-ttu-id="1cd4a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1cd4a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cd4a-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1cd4a-123">Request body</span></span>
<span data-ttu-id="1cd4a-124">В тексте запроса добавьте представление объекта androidForWorkEnrollmentProfile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="1cd4a-125">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта androidForWorkEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="1cd4a-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cd4a-126">Property</span></span>|<span data-ttu-id="1cd4a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="1cd4a-127">Type</span></span>|<span data-ttu-id="1cd4a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="1cd4a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cd4a-129">accountId</span><span class="sxs-lookup"><span data-stu-id="1cd4a-129">accountId</span></span>|<span data-ttu-id="1cd4a-130">String</span><span class="sxs-lookup"><span data-stu-id="1cd4a-130">String</span></span>|<span data-ttu-id="1cd4a-131">GUID клиента, которому принадлежит профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-131">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="1cd4a-132">id</span><span class="sxs-lookup"><span data-stu-id="1cd4a-132">id</span></span>|<span data-ttu-id="1cd4a-133">String</span><span class="sxs-lookup"><span data-stu-id="1cd4a-133">String</span></span>|<span data-ttu-id="1cd4a-134">Уникальный GUID профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-134">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="1cd4a-135">name</span><span class="sxs-lookup"><span data-stu-id="1cd4a-135">name</span></span>|<span data-ttu-id="1cd4a-136">String</span><span class="sxs-lookup"><span data-stu-id="1cd4a-136">String</span></span>|<span data-ttu-id="1cd4a-137">(Нерекомендуемое) Отображаемое имя для профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-137">(Deprecated) Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="1cd4a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="1cd4a-138">displayName</span></span>|<span data-ttu-id="1cd4a-139">String</span><span class="sxs-lookup"><span data-stu-id="1cd4a-139">String</span></span>|<span data-ttu-id="1cd4a-140">Отображаемое имя профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="1cd4a-141">description</span><span class="sxs-lookup"><span data-stu-id="1cd4a-141">description</span></span>|<span data-ttu-id="1cd4a-142">String</span><span class="sxs-lookup"><span data-stu-id="1cd4a-142">String</span></span>|<span data-ttu-id="1cd4a-143">Описание профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="1cd4a-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1cd4a-144">createdDateTime</span></span>|<span data-ttu-id="1cd4a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cd4a-145">DateTimeOffset</span></span>|<span data-ttu-id="1cd4a-146">Дата и время создания профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="1cd4a-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1cd4a-147">modifiedDateTime</span></span>|<span data-ttu-id="1cd4a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cd4a-148">DateTimeOffset</span></span>|<span data-ttu-id="1cd4a-149">(Нерекомендуемое) Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-149">(Deprecated) Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="1cd4a-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1cd4a-150">lastModifiedDateTime</span></span>|<span data-ttu-id="1cd4a-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cd4a-151">DateTimeOffset</span></span>|<span data-ttu-id="1cd4a-152">Дата и время последнего изменения профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-152">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="1cd4a-153">tokenValue</span><span class="sxs-lookup"><span data-stu-id="1cd4a-153">tokenValue</span></span>|<span data-ttu-id="1cd4a-154">String</span><span class="sxs-lookup"><span data-stu-id="1cd4a-154">String</span></span>|<span data-ttu-id="1cd4a-155">Значение последнего созданного маркера для этого профиля регистрации.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-155">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="1cd4a-156">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1cd4a-156">tokenExpirationDateTime</span></span>|<span data-ttu-id="1cd4a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cd4a-157">DateTimeOffset</span></span>|<span data-ttu-id="1cd4a-158">Дата и время, когда истекает срок действия последнего созданного маркера.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-158">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="1cd4a-159">totalEnrollmentCount</span><span class="sxs-lookup"><span data-stu-id="1cd4a-159">totalEnrollmentCount</span></span>|<span data-ttu-id="1cd4a-160">Int32</span><span class="sxs-lookup"><span data-stu-id="1cd4a-160">Int32</span></span>|<span data-ttu-id="1cd4a-161">(Нерекомендуемое) Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-161">(Deprecated) Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="1cd4a-162">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1cd4a-162">enrolledDeviceCount</span></span>|<span data-ttu-id="1cd4a-163">Int32</span><span class="sxs-lookup"><span data-stu-id="1cd4a-163">Int32</span></span>|<span data-ttu-id="1cd4a-164">Общее количество устройств с Android, зарегистрированных через этот профиль регистрации.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-164">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="1cd4a-165">qrCode</span><span class="sxs-lookup"><span data-stu-id="1cd4a-165">qrCode</span></span>|<span data-ttu-id="1cd4a-166">String</span><span class="sxs-lookup"><span data-stu-id="1cd4a-166">String</span></span>|<span data-ttu-id="1cd4a-167">(Нерекомендуемое) Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-167">(Deprecated) String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="1cd4a-168">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="1cd4a-168">qrCodeContent</span></span>|<span data-ttu-id="1cd4a-169">String</span><span class="sxs-lookup"><span data-stu-id="1cd4a-169">String</span></span>|<span data-ttu-id="1cd4a-170">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-170">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="1cd4a-171">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="1cd4a-171">qrCodeImage</span></span>|[<span data-ttu-id="1cd4a-172">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1cd4a-172">mimeContent</span></span>](../resources/intune_androidforwork_mimecontent.md)|<span data-ttu-id="1cd4a-173">Строка, используемая для создания QR-кода маркера.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-173">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="1cd4a-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cd4a-174">Response</span></span>
<span data-ttu-id="1cd4a-175">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-175">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cd4a-176">Пример</span><span class="sxs-lookup"><span data-stu-id="1cd4a-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="1cd4a-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cd4a-177">Request</span></span>
<span data-ttu-id="1cd4a-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkEnrollmentProfiles
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
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

### <a name="response"></a><span data-ttu-id="1cd4a-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cd4a-179">Response</span></span>
<span data-ttu-id="1cd4a-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1cd4a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



