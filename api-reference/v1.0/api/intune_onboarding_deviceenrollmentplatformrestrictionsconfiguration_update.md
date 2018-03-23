# <a name="update-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="d6960-101">Обновление объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="d6960-101">Update deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="d6960-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d6960-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6960-103">Обновление свойств объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6960-103">Update the properties of a [calendar](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d6960-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d6960-104">Prerequisites</span></span>
<span data-ttu-id="d6960-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d6960-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d6960-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6960-107">Permission type</span></span>|<span data-ttu-id="d6960-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6960-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6960-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6960-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d6960-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6960-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d6960-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6960-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6960-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6960-112">Not supported.</span></span>|
|<span data-ttu-id="d6960-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6960-113">Application</span></span>|<span data-ttu-id="d6960-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6960-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6960-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6960-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d6960-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6960-116">Request headers</span></span>
|<span data-ttu-id="d6960-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6960-117">Header</span></span>|<span data-ttu-id="d6960-118">Значение</span><span class="sxs-lookup"><span data-stu-id="d6960-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6960-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6960-119">Authorization</span></span>|<span data-ttu-id="d6960-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6960-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d6960-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d6960-121">Accept</span></span>|<span data-ttu-id="d6960-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d6960-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6960-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d6960-123">Request body</span></span>
<span data-ttu-id="d6960-124">В теле запроса добавьте представление объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6960-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>

<span data-ttu-id="d6960-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6960-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="d6960-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6960-126">Property</span></span>|<span data-ttu-id="d6960-127">Тип</span><span class="sxs-lookup"><span data-stu-id="d6960-127">Type</span></span>|<span data-ttu-id="d6960-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d6960-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6960-129">id</span><span class="sxs-lookup"><span data-stu-id="d6960-129">id</span></span>|<span data-ttu-id="d6960-130">String</span><span class="sxs-lookup"><span data-stu-id="d6960-130">String</span></span>|<span data-ttu-id="d6960-131">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6960-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d6960-132">displayName</span><span class="sxs-lookup"><span data-stu-id="d6960-132">displayName</span></span>|<span data-ttu-id="d6960-133">String</span><span class="sxs-lookup"><span data-stu-id="d6960-133">String</span></span>|<span data-ttu-id="d6960-134">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6960-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d6960-135">description</span><span class="sxs-lookup"><span data-stu-id="d6960-135">description</span></span>|<span data-ttu-id="d6960-136">String</span><span class="sxs-lookup"><span data-stu-id="d6960-136">String</span></span>|<span data-ttu-id="d6960-137">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6960-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d6960-138">priority</span><span class="sxs-lookup"><span data-stu-id="d6960-138">priority</span></span>|<span data-ttu-id="d6960-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d6960-139">Int32</span></span>|<span data-ttu-id="d6960-140">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6960-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d6960-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6960-141">createdDateTime</span></span>|<span data-ttu-id="d6960-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6960-142">DateTimeOffset</span></span>|<span data-ttu-id="d6960-143">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6960-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d6960-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6960-144">lastModifiedDateTime</span></span>|<span data-ttu-id="d6960-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6960-145">DateTimeOffset</span></span>|<span data-ttu-id="d6960-146">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6960-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d6960-147">version</span><span class="sxs-lookup"><span data-stu-id="d6960-147">version</span></span>|<span data-ttu-id="d6960-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d6960-148">Int32</span></span>|<span data-ttu-id="d6960-149">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d6960-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="d6960-150">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="d6960-150">iosRestriction</span></span>|[<span data-ttu-id="d6960-151">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d6960-151">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d6960-152">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d6960-152">Not yet documented</span></span>|
|<span data-ttu-id="d6960-153">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="d6960-153">windowsRestriction</span></span>|[<span data-ttu-id="d6960-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d6960-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d6960-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d6960-155">Not yet documented</span></span>|
|<span data-ttu-id="d6960-156">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="d6960-156">windowsMobileRestriction</span></span>|[<span data-ttu-id="d6960-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d6960-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d6960-158">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d6960-158">Not yet documented</span></span>|
|<span data-ttu-id="d6960-159">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="d6960-159">androidRestriction</span></span>|[<span data-ttu-id="d6960-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d6960-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d6960-161">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d6960-161">Not yet documented</span></span>|
|<span data-ttu-id="d6960-162">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="d6960-162">macOSRestriction</span></span>|[<span data-ttu-id="d6960-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="d6960-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="d6960-164">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d6960-164">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d6960-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6960-165">Response</span></span>
<span data-ttu-id="d6960-166">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d6960-166">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6960-167">Пример</span><span class="sxs-lookup"><span data-stu-id="d6960-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="d6960-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6960-168">Request</span></span>
<span data-ttu-id="d6960-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6960-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 1626

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```

### <a name="response"></a><span data-ttu-id="d6960-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="d6960-170">Response</span></span>
<span data-ttu-id="d6960-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d6960-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1822

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "iosRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "windowsMobileRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "androidRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  },
  "macOSRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value"
  }
}
```



