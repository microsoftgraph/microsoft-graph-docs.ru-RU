# <a name="update-vpptoken"></a><span data-ttu-id="b96da-101">Обновить VPP токен</span><span class="sxs-lookup"><span data-stu-id="b96da-101">Update vppToken</span></span>

> <span data-ttu-id="b96da-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b96da-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b96da-103">Обновление свойств объекта [VPP токен](../resources/intune_onboarding_vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="b96da-103">Update the properties of a [vppToken](../resources/intune_onboarding_vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b96da-104">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="b96da-104">Prerequisites</span></span>
<span data-ttu-id="b96da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b96da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b96da-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b96da-107">Permission type</span></span>|<span data-ttu-id="b96da-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b96da-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b96da-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b96da-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b96da-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b96da-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b96da-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b96da-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b96da-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b96da-112">Not supported.</span></span>|
|<span data-ttu-id="b96da-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b96da-113">Application</span></span>|<span data-ttu-id="b96da-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b96da-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b96da-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b96da-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="b96da-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b96da-116">Request headers</span></span>
|<span data-ttu-id="b96da-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b96da-117">Header</span></span>|<span data-ttu-id="b96da-118">Значение</span><span class="sxs-lookup"><span data-stu-id="b96da-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b96da-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b96da-119">Authorization</span></span>|<span data-ttu-id="b96da-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="b96da-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b96da-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b96da-121">Accept</span></span>|<span data-ttu-id="b96da-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b96da-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b96da-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b96da-123">Request body</span></span>
<span data-ttu-id="b96da-124">В тексте запроса добавьте представление объекта [VPP токен](../resources/intune_onboarding_vpptoken.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b96da-124">In the request body, supply a JSON representation for the [vppToken](../resources/intune_onboarding_vpptoken.md) object.</span></span>

<span data-ttu-id="b96da-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [VPP токен](../resources/intune_onboarding_vpptoken.md).</span><span class="sxs-lookup"><span data-stu-id="b96da-125">The following table shows the properties that are required when you create the [vppToken](../resources/intune_onboarding_vpptoken.md).</span></span>

|<span data-ttu-id="b96da-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="b96da-126">Property</span></span>|<span data-ttu-id="b96da-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b96da-127">Type</span></span>|<span data-ttu-id="b96da-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b96da-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b96da-129">id</span><span class="sxs-lookup"><span data-stu-id="b96da-129">id</span></span>|<span data-ttu-id="b96da-130">Строка</span><span class="sxs-lookup"><span data-stu-id="b96da-130">String</span></span>|<span data-ttu-id="b96da-131">Автоматически генерируется при создании appleVolumePurchaseProgramToken.</span><span class="sxs-lookup"><span data-stu-id="b96da-131">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="b96da-132">Это ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b96da-132">It is the Key of the entity.</span></span>|
|<span data-ttu-id="b96da-133">organizationName</span><span class="sxs-lookup"><span data-stu-id="b96da-133">organizationName</span></span>|<span data-ttu-id="b96da-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b96da-134">String</span></span>|<span data-ttu-id="b96da-135">Организация, связанная с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="b96da-135">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="b96da-136">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="b96da-136">vppTokenAccountType</span></span>|[<span data-ttu-id="b96da-137">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="b96da-137">vppTokenAccountType</span></span>](../resources/intune_shared_vpptokenaccounttype.md)|<span data-ttu-id="b96da-138">Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="b96da-138">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="b96da-139">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="b96da-139">The possible values are:</span></span> <span data-ttu-id="b96da-140">Возможные значения: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="b96da-140">The possible values are:</span></span>|
|<span data-ttu-id="b96da-141">appleId</span><span class="sxs-lookup"><span data-stu-id="b96da-141">appleId</span></span>|<span data-ttu-id="b96da-142">Строка</span><span class="sxs-lookup"><span data-stu-id="b96da-142">String</span></span>|<span data-ttu-id="b96da-143">Идентификатор Apple ID, связанный с заданным маркером Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="b96da-143">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b96da-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b96da-144">expirationDateTime</span></span>|<span data-ttu-id="b96da-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b96da-145">DateTimeOffset</span></span>|<span data-ttu-id="b96da-146">Дата и время завершения срока действия маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="b96da-146">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b96da-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b96da-147">lastSyncDateTime</span></span>|<span data-ttu-id="b96da-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b96da-148">DateTimeOffset</span></span>|<span data-ttu-id="b96da-149">Последнее выполнение синхронизации приложения при помощи службы Apple Volume Purchase Program с использованием токена Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="b96da-149">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b96da-150">токен</span><span class="sxs-lookup"><span data-stu-id="b96da-150">token</span></span>|<span data-ttu-id="b96da-151">Строка</span><span class="sxs-lookup"><span data-stu-id="b96da-151">String</span></span>|<span data-ttu-id="b96da-152">Строка токена Apple Volume Purchase Program; загрузка выполнена из Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="b96da-152">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="b96da-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b96da-153">lastModifiedDateTime</span></span>|<span data-ttu-id="b96da-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b96da-154">DateTimeOffset</span></span>|<span data-ttu-id="b96da-155">Дата и время последнего изменения, связанного с токеном Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="b96da-155">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b96da-156">state</span><span class="sxs-lookup"><span data-stu-id="b96da-156">state</span></span>|[<span data-ttu-id="b96da-157">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="b96da-157">vppTokenState</span></span>](../resources/intune_onboarding_vpptokenstate.md)|<span data-ttu-id="b96da-158">Текущее состояние маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="b96da-158">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="b96da-159">Возможные значения: `unknown`, `valid`, `expired`, `invalid`.</span><span class="sxs-lookup"><span data-stu-id="b96da-159">The possible values are `unknown`, `valid`, `expired`, `invalid`, , , , , , , , or .</span></span> <span data-ttu-id="b96da-160">Возможные значения: `unknown`, `valid`, `expired`, `invalid`.</span><span class="sxs-lookup"><span data-stu-id="b96da-160">The possible values are `unknown`, `valid`, `expired`, `invalid`, , , , , , , , or .</span></span>|
|<span data-ttu-id="b96da-161">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="b96da-161">lastSyncStatus</span></span>|[<span data-ttu-id="b96da-162">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="b96da-162">vppTokenSyncStatus</span></span>](../resources/intune_onboarding_vpptokensyncstatus.md)|<span data-ttu-id="b96da-163">Текущее состояние последней синхронизации приложения, инициированной с помощью маркера Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="b96da-163">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="b96da-164">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="b96da-164">The possible values are `none`, `inProgress`, `completed`, `failed`, , , , , , , , or .</span></span> <span data-ttu-id="b96da-165">Возможные значения: `none`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="b96da-165">The possible values are `none`, `inProgress`, `completed`, `failed`, , , , , , , , or .</span></span>|
|<span data-ttu-id="b96da-166">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="b96da-166">automaticallyUpdateApps</span></span>|<span data-ttu-id="b96da-167">Логическое</span><span class="sxs-lookup"><span data-stu-id="b96da-167">Boolean</span></span>|<span data-ttu-id="b96da-168">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="b96da-168">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="b96da-169">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="b96da-169">countryOrRegion</span></span>|<span data-ttu-id="b96da-170">Строка</span><span class="sxs-lookup"><span data-stu-id="b96da-170">String</span></span>|<span data-ttu-id="b96da-171">Автоматически обновятся все приложения, не только для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="b96da-171">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="b96da-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="b96da-172">Response</span></span>
<span data-ttu-id="b96da-173">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [VPP токен](../resources/intune_onboarding_vpptoken.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b96da-173">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune_onboarding_vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b96da-174">Пример</span><span class="sxs-lookup"><span data-stu-id="b96da-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="b96da-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="b96da-175">Request</span></span>
<span data-ttu-id="b96da-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b96da-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b96da-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="b96da-177">Response</span></span>
<span data-ttu-id="b96da-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b96da-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



