# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="671a9-101">Создание объекта deviceEnrollmentLimitConfiguration</span><span class="sxs-lookup"><span data-stu-id="671a9-101">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="671a9-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="671a9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="671a9-103">Создание объекта [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="671a9-103">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="671a9-104">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="671a9-104">Prerequisites</span></span>
<span data-ttu-id="671a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="671a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="671a9-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="671a9-107">Permission type</span></span>|<span data-ttu-id="671a9-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="671a9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="671a9-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="671a9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="671a9-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="671a9-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="671a9-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="671a9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="671a9-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="671a9-112">Not supported.</span></span>|
|<span data-ttu-id="671a9-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="671a9-113">Application</span></span>|<span data-ttu-id="671a9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="671a9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="671a9-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="671a9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="671a9-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="671a9-116">Request headers</span></span>
|<span data-ttu-id="671a9-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="671a9-117">Header</span></span>|<span data-ttu-id="671a9-118">Значение</span><span class="sxs-lookup"><span data-stu-id="671a9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="671a9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="671a9-119">Authorization</span></span>|<span data-ttu-id="671a9-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="671a9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="671a9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="671a9-121">Accept</span></span>|<span data-ttu-id="671a9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="671a9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="671a9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="671a9-123">Request body</span></span>
<span data-ttu-id="671a9-124">В тексте запроса добавьте представление объекта deviceEnrollmentLimitConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="671a9-124">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="671a9-125">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceEnrollmentLimitConfiguration.</span><span class="sxs-lookup"><span data-stu-id="671a9-125">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="671a9-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="671a9-126">Property</span></span>|<span data-ttu-id="671a9-127">Тип</span><span class="sxs-lookup"><span data-stu-id="671a9-127">Type</span></span>|<span data-ttu-id="671a9-128">Описание</span><span class="sxs-lookup"><span data-stu-id="671a9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="671a9-129">id</span><span class="sxs-lookup"><span data-stu-id="671a9-129">id</span></span>|<span data-ttu-id="671a9-130">String</span><span class="sxs-lookup"><span data-stu-id="671a9-130">String</span></span>|<span data-ttu-id="671a9-131">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="671a9-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="671a9-132">displayName</span><span class="sxs-lookup"><span data-stu-id="671a9-132">displayName</span></span>|<span data-ttu-id="671a9-133">String</span><span class="sxs-lookup"><span data-stu-id="671a9-133">String</span></span>|<span data-ttu-id="671a9-134">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="671a9-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="671a9-135">description</span><span class="sxs-lookup"><span data-stu-id="671a9-135">description</span></span>|<span data-ttu-id="671a9-136">String</span><span class="sxs-lookup"><span data-stu-id="671a9-136">String</span></span>|<span data-ttu-id="671a9-137">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="671a9-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="671a9-138">priority</span><span class="sxs-lookup"><span data-stu-id="671a9-138">priority</span></span>|<span data-ttu-id="671a9-139">Int32</span><span class="sxs-lookup"><span data-stu-id="671a9-139">Int32</span></span>|<span data-ttu-id="671a9-140">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="671a9-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="671a9-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="671a9-141">createdDateTime</span></span>|<span data-ttu-id="671a9-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="671a9-142">DateTimeOffset</span></span>|<span data-ttu-id="671a9-143">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="671a9-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="671a9-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="671a9-144">lastModifiedDateTime</span></span>|<span data-ttu-id="671a9-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="671a9-145">DateTimeOffset</span></span>|<span data-ttu-id="671a9-146">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="671a9-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="671a9-147">version</span><span class="sxs-lookup"><span data-stu-id="671a9-147">version</span></span>|<span data-ttu-id="671a9-148">Int32</span><span class="sxs-lookup"><span data-stu-id="671a9-148">Int32</span></span>|<span data-ttu-id="671a9-149">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="671a9-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="671a9-150">limit</span><span class="sxs-lookup"><span data-stu-id="671a9-150">limit</span></span>|<span data-ttu-id="671a9-151">Int32</span><span class="sxs-lookup"><span data-stu-id="671a9-151">Int32</span></span>|<span data-ttu-id="671a9-152">Н/Д</span><span class="sxs-lookup"><span data-stu-id="671a9-152">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="671a9-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="671a9-153">Response</span></span>
<span data-ttu-id="671a9-154">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="671a9-154">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="671a9-155">Пример</span><span class="sxs-lookup"><span data-stu-id="671a9-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="671a9-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="671a9-156">Request</span></span>
<span data-ttu-id="671a9-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="671a9-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 205

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="671a9-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="671a9-158">Response</span></span>
<span data-ttu-id="671a9-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="671a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



