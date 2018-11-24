# <a name="create-deviceenrollmentplatformrestrictionsconfiguration"></a><span data-ttu-id="ac310-101">Создание объекта deviceEnrollmentPlatformRestrictionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="ac310-101">Create deviceEnrollmentPlatformRestrictionsConfiguration</span></span>

> <span data-ttu-id="ac310-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ac310-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac310-103">Создание объекта [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac310-103">Create a new [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ac310-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ac310-104">Prerequisites</span></span>
<span data-ttu-id="ac310-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ac310-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ac310-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac310-107">Permission type</span></span>|<span data-ttu-id="ac310-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac310-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac310-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac310-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ac310-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac310-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ac310-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac310-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac310-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac310-112">Not supported.</span></span>|
|<span data-ttu-id="ac310-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac310-113">Application</span></span>|<span data-ttu-id="ac310-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac310-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac310-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac310-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ac310-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac310-116">Request headers</span></span>
|<span data-ttu-id="ac310-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ac310-117">Header</span></span>|<span data-ttu-id="ac310-118">Значение</span><span class="sxs-lookup"><span data-stu-id="ac310-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac310-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac310-119">Authorization</span></span>|<span data-ttu-id="ac310-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac310-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac310-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ac310-121">Accept</span></span>|<span data-ttu-id="ac310-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ac310-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac310-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ac310-123">Request body</span></span>
<span data-ttu-id="ac310-124">В теле запроса добавьте представление объекта deviceEnrollmentPlatformRestrictionsConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac310-124">In the request body, supply a JSON representation for the deviceEnrollmentPlatformRestrictionsConfiguration object.</span></span>

<span data-ttu-id="ac310-125">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceEnrollmentPlatformRestrictionsConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ac310-125">The following table shows the properties that are required when you create the deviceEnrollmentPlatformRestrictionsConfiguration.</span></span>

|<span data-ttu-id="ac310-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac310-126">Property</span></span>|<span data-ttu-id="ac310-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ac310-127">Type</span></span>|<span data-ttu-id="ac310-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ac310-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac310-129">id</span><span class="sxs-lookup"><span data-stu-id="ac310-129">id</span></span>|<span data-ttu-id="ac310-130">String</span><span class="sxs-lookup"><span data-stu-id="ac310-130">String</span></span>|<span data-ttu-id="ac310-131">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac310-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ac310-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ac310-132">displayName</span></span>|<span data-ttu-id="ac310-133">String</span><span class="sxs-lookup"><span data-stu-id="ac310-133">String</span></span>|<span data-ttu-id="ac310-134">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac310-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ac310-135">description</span><span class="sxs-lookup"><span data-stu-id="ac310-135">description</span></span>|<span data-ttu-id="ac310-136">String</span><span class="sxs-lookup"><span data-stu-id="ac310-136">String</span></span>|<span data-ttu-id="ac310-137">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac310-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ac310-138">priority</span><span class="sxs-lookup"><span data-stu-id="ac310-138">priority</span></span>|<span data-ttu-id="ac310-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ac310-139">Int32</span></span>|<span data-ttu-id="ac310-140">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac310-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ac310-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac310-141">createdDateTime</span></span>|<span data-ttu-id="ac310-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac310-142">DateTimeOffset</span></span>|<span data-ttu-id="ac310-143">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac310-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ac310-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac310-144">lastModifiedDateTime</span></span>|<span data-ttu-id="ac310-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac310-145">DateTimeOffset</span></span>|<span data-ttu-id="ac310-146">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac310-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ac310-147">version</span><span class="sxs-lookup"><span data-stu-id="ac310-147">version</span></span>|<span data-ttu-id="ac310-148">Int32</span><span class="sxs-lookup"><span data-stu-id="ac310-148">Int32</span></span>|<span data-ttu-id="ac310-149">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ac310-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ac310-150">iosRestriction</span><span class="sxs-lookup"><span data-stu-id="ac310-150">iosRestriction</span></span>|[<span data-ttu-id="ac310-151">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ac310-151">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ac310-152">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ac310-152">Not yet documented</span></span>|
|<span data-ttu-id="ac310-153">windowsRestriction</span><span class="sxs-lookup"><span data-stu-id="ac310-153">windowsRestriction</span></span>|[<span data-ttu-id="ac310-154">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ac310-154">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ac310-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ac310-155">Not yet documented</span></span>|
|<span data-ttu-id="ac310-156">windowsMobileRestriction</span><span class="sxs-lookup"><span data-stu-id="ac310-156">windowsMobileRestriction</span></span>|[<span data-ttu-id="ac310-157">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ac310-157">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ac310-158">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ac310-158">Not yet documented</span></span>|
|<span data-ttu-id="ac310-159">androidRestriction</span><span class="sxs-lookup"><span data-stu-id="ac310-159">androidRestriction</span></span>|[<span data-ttu-id="ac310-160">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ac310-160">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ac310-161">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ac310-161">Not yet documented</span></span>|
|<span data-ttu-id="ac310-162">macOSRestriction</span><span class="sxs-lookup"><span data-stu-id="ac310-162">macOSRestriction</span></span>|[<span data-ttu-id="ac310-163">deviceEnrollmentPlatformRestriction</span><span class="sxs-lookup"><span data-stu-id="ac310-163">deviceEnrollmentPlatformRestriction</span></span>](../resources/intune_onboarding_deviceenrollmentplatformrestriction.md)|<span data-ttu-id="ac310-164">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ac310-164">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ac310-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac310-165">Response</span></span>
<span data-ttu-id="ac310-166">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ac310-166">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac310-167">Пример</span><span class="sxs-lookup"><span data-stu-id="ac310-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="ac310-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac310-168">Request</span></span>
<span data-ttu-id="ac310-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac310-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 1650

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
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

### <a name="response"></a><span data-ttu-id="ac310-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="ac310-170">Response</span></span>
<span data-ttu-id="ac310-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ac310-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



