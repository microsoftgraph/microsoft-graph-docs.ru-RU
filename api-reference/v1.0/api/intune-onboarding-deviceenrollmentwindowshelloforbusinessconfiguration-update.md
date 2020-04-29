---
title: Обновление deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Обновление свойств объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bcabc2772fa2b60d6f7563f9288b436f68037f74
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450051"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="eb0d0-103">Обновление deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="eb0d0-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

<span data-ttu-id="eb0d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb0d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb0d0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb0d0-106">Обновление свойств объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb0d0-106">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb0d0-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eb0d0-107">Prerequisites</span></span>
<span data-ttu-id="eb0d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb0d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb0d0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb0d0-110">Permission type</span></span>|<span data-ttu-id="eb0d0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb0d0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb0d0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb0d0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb0d0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb0d0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="eb0d0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb0d0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb0d0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-115">Not supported.</span></span>|
|<span data-ttu-id="eb0d0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb0d0-116">Application</span></span>|<span data-ttu-id="eb0d0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb0d0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb0d0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="eb0d0-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eb0d0-119">Request headers</span></span>
|<span data-ttu-id="eb0d0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eb0d0-120">Header</span></span>|<span data-ttu-id="eb0d0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="eb0d0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb0d0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb0d0-122">Authorization</span></span>|<span data-ttu-id="eb0d0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb0d0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="eb0d0-124">Accept</span></span>|<span data-ttu-id="eb0d0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb0d0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb0d0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eb0d0-126">Request body</span></span>
<span data-ttu-id="eb0d0-127">В теле запроса добавьте представление объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-127">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="eb0d0-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb0d0-128">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="eb0d0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb0d0-129">Property</span></span>|<span data-ttu-id="eb0d0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="eb0d0-130">Type</span></span>|<span data-ttu-id="eb0d0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="eb0d0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb0d0-132">id</span><span class="sxs-lookup"><span data-stu-id="eb0d0-132">id</span></span>|<span data-ttu-id="eb0d0-133">String</span><span class="sxs-lookup"><span data-stu-id="eb0d0-133">String</span></span>|<span data-ttu-id="eb0d0-134">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb0d0-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="eb0d0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="eb0d0-135">displayName</span></span>|<span data-ttu-id="eb0d0-136">Строка</span><span class="sxs-lookup"><span data-stu-id="eb0d0-136">String</span></span>|<span data-ttu-id="eb0d0-137">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb0d0-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="eb0d0-138">description</span><span class="sxs-lookup"><span data-stu-id="eb0d0-138">description</span></span>|<span data-ttu-id="eb0d0-139">String</span><span class="sxs-lookup"><span data-stu-id="eb0d0-139">String</span></span>|<span data-ttu-id="eb0d0-140">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb0d0-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="eb0d0-141">priority</span><span class="sxs-lookup"><span data-stu-id="eb0d0-141">priority</span></span>|<span data-ttu-id="eb0d0-142">Int32</span><span class="sxs-lookup"><span data-stu-id="eb0d0-142">Int32</span></span>|<span data-ttu-id="eb0d0-143">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb0d0-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="eb0d0-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb0d0-144">createdDateTime</span></span>|<span data-ttu-id="eb0d0-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb0d0-145">DateTimeOffset</span></span>|<span data-ttu-id="eb0d0-146">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb0d0-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="eb0d0-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb0d0-147">lastModifiedDateTime</span></span>|<span data-ttu-id="eb0d0-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb0d0-148">DateTimeOffset</span></span>|<span data-ttu-id="eb0d0-149">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb0d0-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="eb0d0-150">version</span><span class="sxs-lookup"><span data-stu-id="eb0d0-150">version</span></span>|<span data-ttu-id="eb0d0-151">Int32</span><span class="sxs-lookup"><span data-stu-id="eb0d0-151">Int32</span></span>|<span data-ttu-id="eb0d0-152">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb0d0-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="eb0d0-153">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="eb0d0-153">pinMinimumLength</span></span>|<span data-ttu-id="eb0d0-154">Int32</span><span class="sxs-lookup"><span data-stu-id="eb0d0-154">Int32</span></span>|<span data-ttu-id="eb0d0-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-155">Not yet documented</span></span>|
|<span data-ttu-id="eb0d0-156">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="eb0d0-156">pinMaximumLength</span></span>|<span data-ttu-id="eb0d0-157">Int32</span><span class="sxs-lookup"><span data-stu-id="eb0d0-157">Int32</span></span>|<span data-ttu-id="eb0d0-158">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-158">Not yet documented</span></span>|
|<span data-ttu-id="eb0d0-159">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="eb0d0-159">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="eb0d0-160">виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="eb0d0-160">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="eb0d0-161">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-161">Not yet documented.</span></span> <span data-ttu-id="eb0d0-162">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-162">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="eb0d0-163">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="eb0d0-163">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="eb0d0-164">виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="eb0d0-164">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="eb0d0-165">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-165">Not yet documented.</span></span> <span data-ttu-id="eb0d0-166">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-166">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="eb0d0-167">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="eb0d0-167">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="eb0d0-168">виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="eb0d0-168">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="eb0d0-169">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-169">Not yet documented.</span></span> <span data-ttu-id="eb0d0-170">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-170">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="eb0d0-171">state</span><span class="sxs-lookup"><span data-stu-id="eb0d0-171">state</span></span>|[<span data-ttu-id="eb0d0-172">Включение</span><span class="sxs-lookup"><span data-stu-id="eb0d0-172">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="eb0d0-173">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-173">Not yet documented.</span></span> <span data-ttu-id="eb0d0-174">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-174">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="eb0d0-175">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="eb0d0-175">securityDeviceRequired</span></span>|<span data-ttu-id="eb0d0-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb0d0-176">Boolean</span></span>|<span data-ttu-id="eb0d0-177">Н/Д</span><span class="sxs-lookup"><span data-stu-id="eb0d0-177">Not yet documented</span></span>|
|<span data-ttu-id="eb0d0-178">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="eb0d0-178">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="eb0d0-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb0d0-179">Boolean</span></span>|<span data-ttu-id="eb0d0-180">Н/Д</span><span class="sxs-lookup"><span data-stu-id="eb0d0-180">Not yet documented</span></span>|
|<span data-ttu-id="eb0d0-181">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="eb0d0-181">remotePassportEnabled</span></span>|<span data-ttu-id="eb0d0-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb0d0-182">Boolean</span></span>|<span data-ttu-id="eb0d0-183">Н/Д</span><span class="sxs-lookup"><span data-stu-id="eb0d0-183">Not yet documented</span></span>|
|<span data-ttu-id="eb0d0-184">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="eb0d0-184">pinPreviousBlockCount</span></span>|<span data-ttu-id="eb0d0-185">Int32</span><span class="sxs-lookup"><span data-stu-id="eb0d0-185">Int32</span></span>|<span data-ttu-id="eb0d0-186">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-186">Not yet documented</span></span>|
|<span data-ttu-id="eb0d0-187">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="eb0d0-187">pinExpirationInDays</span></span>|<span data-ttu-id="eb0d0-188">Int32</span><span class="sxs-lookup"><span data-stu-id="eb0d0-188">Int32</span></span>|<span data-ttu-id="eb0d0-189">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-189">Not yet documented</span></span>|
|<span data-ttu-id="eb0d0-190">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="eb0d0-190">enhancedBiometricsState</span></span>|[<span data-ttu-id="eb0d0-191">Включение</span><span class="sxs-lookup"><span data-stu-id="eb0d0-191">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="eb0d0-192">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-192">Not yet documented.</span></span> <span data-ttu-id="eb0d0-193">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="eb0d0-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb0d0-194">Response</span></span>
<span data-ttu-id="eb0d0-195">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-195">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb0d0-196">Пример</span><span class="sxs-lookup"><span data-stu-id="eb0d0-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb0d0-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb0d0-197">Request</span></span>
<span data-ttu-id="eb0d0-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eb0d0-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb0d0-199">Response</span></span>
<span data-ttu-id="eb0d0-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eb0d0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






