# <a name="update-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="d0f36-101">Обновление объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0f36-101">Update deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="d0f36-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d0f36-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0f36-103">Обновление свойств объекта [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0f36-103">Update the properties of a [calendar](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d0f36-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d0f36-104">Prerequisites</span></span>
<span data-ttu-id="d0f36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d0f36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d0f36-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0f36-107">Permission type</span></span>|<span data-ttu-id="d0f36-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0f36-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0f36-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0f36-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d0f36-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0f36-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d0f36-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0f36-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0f36-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0f36-112">Not supported.</span></span>|
|<span data-ttu-id="d0f36-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0f36-113">Application</span></span>|<span data-ttu-id="d0f36-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0f36-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0f36-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0f36-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d0f36-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0f36-116">Request headers</span></span>
|<span data-ttu-id="d0f36-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0f36-117">Header</span></span>|<span data-ttu-id="d0f36-118">Значение</span><span class="sxs-lookup"><span data-stu-id="d0f36-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0f36-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0f36-119">Authorization</span></span>|<span data-ttu-id="d0f36-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0f36-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d0f36-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d0f36-121">Accept</span></span>|<span data-ttu-id="d0f36-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d0f36-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0f36-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d0f36-123">Request body</span></span>
<span data-ttu-id="d0f36-124">В теле запроса добавьте представление объекта [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0f36-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object.</span></span>

<span data-ttu-id="d0f36-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0f36-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="d0f36-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0f36-126">Property</span></span>|<span data-ttu-id="d0f36-127">Тип</span><span class="sxs-lookup"><span data-stu-id="d0f36-127">Type</span></span>|<span data-ttu-id="d0f36-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d0f36-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0f36-129">id</span><span class="sxs-lookup"><span data-stu-id="d0f36-129">id</span></span>|<span data-ttu-id="d0f36-130">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-130">String</span></span>|<span data-ttu-id="d0f36-131">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0f36-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d0f36-132">displayName</span><span class="sxs-lookup"><span data-stu-id="d0f36-132">displayName</span></span>|<span data-ttu-id="d0f36-133">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-133">String</span></span>|<span data-ttu-id="d0f36-134">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0f36-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d0f36-135">description</span><span class="sxs-lookup"><span data-stu-id="d0f36-135">description</span></span>|<span data-ttu-id="d0f36-136">String</span><span class="sxs-lookup"><span data-stu-id="d0f36-136">String</span></span>|<span data-ttu-id="d0f36-137">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0f36-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d0f36-138">priority</span><span class="sxs-lookup"><span data-stu-id="d0f36-138">priority</span></span>|<span data-ttu-id="d0f36-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d0f36-139">Int32</span></span>|<span data-ttu-id="d0f36-140">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0f36-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d0f36-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0f36-141">createdDateTime</span></span>|<span data-ttu-id="d0f36-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0f36-142">DateTimeOffset</span></span>|<span data-ttu-id="d0f36-143">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0f36-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d0f36-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0f36-144">lastModifiedDateTime</span></span>|<span data-ttu-id="d0f36-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0f36-145">DateTimeOffset</span></span>|<span data-ttu-id="d0f36-146">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0f36-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d0f36-147">version</span><span class="sxs-lookup"><span data-stu-id="d0f36-147">version</span></span>|<span data-ttu-id="d0f36-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d0f36-148">Int32</span></span>|<span data-ttu-id="d0f36-149">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0f36-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d0f36-150">limit</span><span class="sxs-lookup"><span data-stu-id="d0f36-150">Limit</span></span>|<span data-ttu-id="d0f36-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d0f36-151">Int32</span></span>|<span data-ttu-id="d0f36-152">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d0f36-152">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d0f36-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0f36-153">Response</span></span>
<span data-ttu-id="d0f36-154">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d0f36-154">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0f36-155">Пример</span><span class="sxs-lookup"><span data-stu-id="d0f36-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="d0f36-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0f36-156">Request</span></span>
<span data-ttu-id="d0f36-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0f36-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 196

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="d0f36-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0f36-158">Response</span></span>
<span data-ttu-id="d0f36-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d0f36-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 377

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```



