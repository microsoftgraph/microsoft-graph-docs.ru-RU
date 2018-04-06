# <a name="update-vpptoken"></a><span data-ttu-id="2d452-101">Обновить VPP токен</span><span class="sxs-lookup"><span data-stu-id="2d452-101">Update vppToken</span></span>

> <span data-ttu-id="2d452-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2d452-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d452-103">Обновление свойств объекта [VPP токен](../resources/intune_onboarding_vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="2d452-103">Update the properties of a [managedAppOperation](../resources/intune_onboarding_vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2d452-104">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="2d452-104">Prerequisites</span></span>
<span data-ttu-id="2d452-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2d452-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2d452-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d452-107">Permission type</span></span>|<span data-ttu-id="2d452-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d452-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d452-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d452-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2d452-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d452-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2d452-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d452-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d452-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d452-112">Not supported.</span></span>|
|<span data-ttu-id="2d452-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d452-113">Application</span></span>|<span data-ttu-id="2d452-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d452-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d452-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d452-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="2d452-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2d452-116">Request headers</span></span>
|<span data-ttu-id="2d452-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2d452-117">Header</span></span>|<span data-ttu-id="2d452-118">Значение</span><span class="sxs-lookup"><span data-stu-id="2d452-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d452-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d452-119">Authorization</span></span>|<span data-ttu-id="2d452-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d452-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d452-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2d452-121">Accept</span></span>|<span data-ttu-id="2d452-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2d452-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d452-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d452-123">Request body</span></span>
<span data-ttu-id="2d452-124">В тексте запроса добавьте представление объекта [VPP токен](../resources/intune_onboarding_vpptoken.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d452-124">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune_onboarding_vpptoken.md) object.</span></span>

<span data-ttu-id="2d452-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [VPP токен](../resources/intune_onboarding_vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="2d452-125">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune_onboarding_vpptoken.md).</span></span>

|<span data-ttu-id="2d452-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d452-126">Property</span></span>|<span data-ttu-id="2d452-127">Тип</span><span class="sxs-lookup"><span data-stu-id="2d452-127">Type</span></span>|<span data-ttu-id="2d452-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2d452-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d452-129">id</span><span class="sxs-lookup"><span data-stu-id="2d452-129">id</span></span>|<span data-ttu-id="2d452-130">Строка</span><span class="sxs-lookup"><span data-stu-id="2d452-130">String</span></span>|<span data-ttu-id="2d452-131">Создается автоматически при создании appleVolumePurchaseProgramToken.</span><span class="sxs-lookup"><span data-stu-id="2d452-131">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="2d452-132">Это ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2d452-132">It is the Key of the entity.</span></span>|
|<span data-ttu-id="2d452-133">organizationName</span><span class="sxs-lookup"><span data-stu-id="2d452-133">organizationName</span></span>|<span data-ttu-id="2d452-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2d452-134">String</span></span>|<span data-ttu-id="2d452-135">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2d452-135">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="2d452-136">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="2d452-136">vppTokenAccountType</span></span>|<span data-ttu-id="2d452-137">String</span><span class="sxs-lookup"><span data-stu-id="2d452-137">String</span></span>|<span data-ttu-id="2d452-138">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2d452-138">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="2d452-139">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="2d452-139">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="2d452-140">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="2d452-140">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="2d452-141">appleId</span><span class="sxs-lookup"><span data-stu-id="2d452-141">appleId</span></span>|<span data-ttu-id="2d452-142">Строка</span><span class="sxs-lookup"><span data-stu-id="2d452-142">String</span></span>|<span data-ttu-id="2d452-143">Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2d452-143">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="2d452-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2d452-144">expirationDateTime</span></span>|<span data-ttu-id="2d452-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d452-145">DateTimeOffset</span></span>|<span data-ttu-id="2d452-146">Дата и время завершения срока действия токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2d452-146">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="2d452-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2d452-147">lastSyncDateTime</span></span>|<span data-ttu-id="2d452-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d452-148">DateTimeOffset</span></span>|<span data-ttu-id="2d452-149">Последнее выполнение синхронизации приложения при помощи службы Apple Volume Purchase Program с использованием токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2d452-149">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="2d452-150">токен</span><span class="sxs-lookup"><span data-stu-id="2d452-150">token</span></span>|<span data-ttu-id="2d452-151">Строка</span><span class="sxs-lookup"><span data-stu-id="2d452-151">String</span></span>|<span data-ttu-id="2d452-152">Строка токена Apple Volume Purchase Program; загрузка выполнена из Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2d452-152">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="2d452-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d452-153">lastModifiedDateTime</span></span>|<span data-ttu-id="2d452-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d452-154">DateTimeOffset</span></span>|<span data-ttu-id="2d452-155">Дата и время последнего изменения, связанного с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2d452-155">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="2d452-156">состояние</span><span class="sxs-lookup"><span data-stu-id="2d452-156">state</span></span>|<span data-ttu-id="2d452-157">Строка</span><span class="sxs-lookup"><span data-stu-id="2d452-157">String</span></span>|<span data-ttu-id="2d452-158">Текущее состояние токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2d452-158">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="2d452-159">Возможные значения: `unknown`, `valid`, `expired`, `invalid`.</span><span class="sxs-lookup"><span data-stu-id="2d452-159">Possible values are: `unknown`, `valid`, `expired`, `invalid`.</span></span> <span data-ttu-id="2d452-160">Возможные значения: `unknown`, `valid`, `expired`, `invalid`.</span><span class="sxs-lookup"><span data-stu-id="2d452-160">Possible values are: `unknown`, `valid`, `expired`, `invalid`.</span></span>|
|<span data-ttu-id="2d452-161">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="2d452-161">lastSyncStatus</span></span>|<span data-ttu-id="2d452-162">Строка</span><span class="sxs-lookup"><span data-stu-id="2d452-162">String</span></span>|<span data-ttu-id="2d452-163">Текущее состояние последней синхронизации приложения, инициированной с помощью токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="2d452-163">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="2d452-164">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="2d452-164">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="2d452-165">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="2d452-165">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="2d452-166">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="2d452-166">automaticallyUpdateApps</span></span>|<span data-ttu-id="2d452-167">Логическое</span><span class="sxs-lookup"><span data-stu-id="2d452-167">Boolean</span></span>|<span data-ttu-id="2d452-168">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="2d452-168">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="2d452-169">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="2d452-169">countryOrRegion</span></span>|<span data-ttu-id="2d452-170">Строка</span><span class="sxs-lookup"><span data-stu-id="2d452-170">String</span></span>|<span data-ttu-id="2d452-171">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="2d452-171">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="2d452-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d452-172">Response</span></span>
<span data-ttu-id="2d452-173">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [VPP токен](../resources/intune_onboarding_vpptoken.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2d452-173">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune_onboarding_vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d452-174">Пример</span><span class="sxs-lookup"><span data-stu-id="2d452-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="2d452-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d452-175">Request</span></span>
<span data-ttu-id="2d452-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d452-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}
Content-type: application/json
Content-length: 478

{
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```

### <a name="response"></a><span data-ttu-id="2d452-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="2d452-177">Response</span></span>
<span data-ttu-id="2d452-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2d452-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```



