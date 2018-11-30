---
title: Обновление deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Обновление свойств объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
ms.openlocfilehash: f91067a57dc4da7dc7d4850f72fbe267f364c6e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028474"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="5bd7e-103">Обновление deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="5bd7e-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="5bd7e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5bd7e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5bd7e-105">Обновление свойств объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5bd7e-105">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5bd7e-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5bd7e-106">Prerequisites</span></span>
<span data-ttu-id="5bd7e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5bd7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bd7e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5bd7e-109">Permission type</span></span>|<span data-ttu-id="5bd7e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5bd7e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bd7e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5bd7e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5bd7e-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bd7e-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5bd7e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5bd7e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bd7e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bd7e-114">Not supported.</span></span>|
|<span data-ttu-id="5bd7e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5bd7e-115">Application</span></span>|<span data-ttu-id="5bd7e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bd7e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bd7e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bd7e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5bd7e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5bd7e-118">Request headers</span></span>
|<span data-ttu-id="5bd7e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5bd7e-119">Header</span></span>|<span data-ttu-id="5bd7e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5bd7e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bd7e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bd7e-121">Authorization</span></span>|<span data-ttu-id="5bd7e-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5bd7e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bd7e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5bd7e-123">Accept</span></span>|<span data-ttu-id="5bd7e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5bd7e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bd7e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5bd7e-125">Request body</span></span>
<span data-ttu-id="5bd7e-126">В теле запроса добавьте представление объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5bd7e-126">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="5bd7e-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5bd7e-127">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="5bd7e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="5bd7e-128">Property</span></span>|<span data-ttu-id="5bd7e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="5bd7e-129">Type</span></span>|<span data-ttu-id="5bd7e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5bd7e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bd7e-131">id</span><span class="sxs-lookup"><span data-stu-id="5bd7e-131">id</span></span>|<span data-ttu-id="5bd7e-132">String</span><span class="sxs-lookup"><span data-stu-id="5bd7e-132">String</span></span>|<span data-ttu-id="5bd7e-133">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5bd7e-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5bd7e-134">displayName</span><span class="sxs-lookup"><span data-stu-id="5bd7e-134">displayName</span></span>|<span data-ttu-id="5bd7e-135">String</span><span class="sxs-lookup"><span data-stu-id="5bd7e-135">String</span></span>|<span data-ttu-id="5bd7e-136">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5bd7e-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5bd7e-137">описание</span><span class="sxs-lookup"><span data-stu-id="5bd7e-137">description</span></span>|<span data-ttu-id="5bd7e-138">String</span><span class="sxs-lookup"><span data-stu-id="5bd7e-138">String</span></span>|<span data-ttu-id="5bd7e-139">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5bd7e-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5bd7e-140">priority</span><span class="sxs-lookup"><span data-stu-id="5bd7e-140">priority</span></span>|<span data-ttu-id="5bd7e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="5bd7e-141">Int32</span></span>|<span data-ttu-id="5bd7e-142">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5bd7e-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5bd7e-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5bd7e-143">createdDateTime</span></span>|<span data-ttu-id="5bd7e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bd7e-144">DateTimeOffset</span></span>|<span data-ttu-id="5bd7e-145">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5bd7e-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5bd7e-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5bd7e-146">lastModifiedDateTime</span></span>|<span data-ttu-id="5bd7e-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bd7e-147">DateTimeOffset</span></span>|<span data-ttu-id="5bd7e-148">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5bd7e-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5bd7e-149">version</span><span class="sxs-lookup"><span data-stu-id="5bd7e-149">version</span></span>|<span data-ttu-id="5bd7e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5bd7e-150">Int32</span></span>|<span data-ttu-id="5bd7e-151">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5bd7e-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="5bd7e-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5bd7e-152">pinMinimumLength</span></span>|<span data-ttu-id="5bd7e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5bd7e-153">Int32</span></span>|<span data-ttu-id="5bd7e-154">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5bd7e-154">Not yet documented</span></span>|
|<span data-ttu-id="5bd7e-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="5bd7e-155">pinMaximumLength</span></span>|<span data-ttu-id="5bd7e-156">Int32</span><span class="sxs-lookup"><span data-stu-id="5bd7e-156">Int32</span></span>|<span data-ttu-id="5bd7e-157">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5bd7e-157">Not yet documented</span></span>|
|<span data-ttu-id="5bd7e-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="5bd7e-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="5bd7e-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="5bd7e-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="5bd7e-160">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="5bd7e-160">Not yet documented.</span></span> <span data-ttu-id="5bd7e-161">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="5bd7e-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="5bd7e-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="5bd7e-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="5bd7e-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="5bd7e-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="5bd7e-164">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="5bd7e-164">Not yet documented.</span></span> <span data-ttu-id="5bd7e-165">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="5bd7e-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="5bd7e-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="5bd7e-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="5bd7e-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="5bd7e-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="5bd7e-168">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="5bd7e-168">Not yet documented.</span></span> <span data-ttu-id="5bd7e-169">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="5bd7e-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="5bd7e-170">state</span><span class="sxs-lookup"><span data-stu-id="5bd7e-170">state</span></span>|[<span data-ttu-id="5bd7e-171">Включение</span><span class="sxs-lookup"><span data-stu-id="5bd7e-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="5bd7e-172">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="5bd7e-172">Not yet documented.</span></span> <span data-ttu-id="5bd7e-173">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="5bd7e-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="5bd7e-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="5bd7e-174">securityDeviceRequired</span></span>|<span data-ttu-id="5bd7e-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bd7e-175">Boolean</span></span>|<span data-ttu-id="5bd7e-176">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5bd7e-176">Not yet documented</span></span>|
|<span data-ttu-id="5bd7e-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="5bd7e-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="5bd7e-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bd7e-178">Boolean</span></span>|<span data-ttu-id="5bd7e-179">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5bd7e-179">Not yet documented</span></span>|
|<span data-ttu-id="5bd7e-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="5bd7e-180">remotePassportEnabled</span></span>|<span data-ttu-id="5bd7e-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="5bd7e-181">Boolean</span></span>|<span data-ttu-id="5bd7e-182">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5bd7e-182">Not yet documented</span></span>|
|<span data-ttu-id="5bd7e-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="5bd7e-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="5bd7e-184">Int32</span><span class="sxs-lookup"><span data-stu-id="5bd7e-184">Int32</span></span>|<span data-ttu-id="5bd7e-185">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5bd7e-185">Not yet documented</span></span>|
|<span data-ttu-id="5bd7e-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="5bd7e-186">pinExpirationInDays</span></span>|<span data-ttu-id="5bd7e-187">Int32</span><span class="sxs-lookup"><span data-stu-id="5bd7e-187">Int32</span></span>|<span data-ttu-id="5bd7e-188">Н/Д</span><span class="sxs-lookup"><span data-stu-id="5bd7e-188">Not yet documented</span></span>|
|<span data-ttu-id="5bd7e-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="5bd7e-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="5bd7e-190">Включение</span><span class="sxs-lookup"><span data-stu-id="5bd7e-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="5bd7e-191">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="5bd7e-191">Not yet documented.</span></span> <span data-ttu-id="5bd7e-192">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="5bd7e-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="5bd7e-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bd7e-193">Response</span></span>
<span data-ttu-id="5bd7e-194">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5bd7e-194">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bd7e-195">Пример</span><span class="sxs-lookup"><span data-stu-id="5bd7e-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="5bd7e-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bd7e-196">Request</span></span>
<span data-ttu-id="5bd7e-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5bd7e-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 629

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="5bd7e-198">Ответ</span><span class="sxs-lookup"><span data-stu-id="5bd7e-198">Response</span></span>
<span data-ttu-id="5bd7e-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5bd7e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 801

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```



