---
title: Обновление deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Обновление свойств объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e8032ab753b3dc70450dd556dc6aaab5005c311
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512589"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="c20e5-103">Обновление deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="c20e5-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

<span data-ttu-id="c20e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c20e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c20e5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c20e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c20e5-106">Обновление свойств объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c20e5-106">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c20e5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c20e5-107">Prerequisites</span></span>
<span data-ttu-id="c20e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c20e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c20e5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c20e5-110">Permission type</span></span>|<span data-ttu-id="c20e5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c20e5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c20e5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c20e5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c20e5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c20e5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c20e5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c20e5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c20e5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c20e5-115">Not supported.</span></span>|
|<span data-ttu-id="c20e5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c20e5-116">Application</span></span>|<span data-ttu-id="c20e5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c20e5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c20e5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c20e5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c20e5-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c20e5-119">Request headers</span></span>
|<span data-ttu-id="c20e5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c20e5-120">Header</span></span>|<span data-ttu-id="c20e5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c20e5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c20e5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c20e5-122">Authorization</span></span>|<span data-ttu-id="c20e5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c20e5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c20e5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c20e5-124">Accept</span></span>|<span data-ttu-id="c20e5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c20e5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c20e5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c20e5-126">Request body</span></span>
<span data-ttu-id="c20e5-127">В теле запроса добавьте представление объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c20e5-127">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="c20e5-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c20e5-128">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="c20e5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c20e5-129">Property</span></span>|<span data-ttu-id="c20e5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c20e5-130">Type</span></span>|<span data-ttu-id="c20e5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c20e5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c20e5-132">id</span><span class="sxs-lookup"><span data-stu-id="c20e5-132">id</span></span>|<span data-ttu-id="c20e5-133">String</span><span class="sxs-lookup"><span data-stu-id="c20e5-133">String</span></span>|<span data-ttu-id="c20e5-134">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c20e5-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c20e5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c20e5-135">displayName</span></span>|<span data-ttu-id="c20e5-136">Строка</span><span class="sxs-lookup"><span data-stu-id="c20e5-136">String</span></span>|<span data-ttu-id="c20e5-137">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c20e5-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c20e5-138">description</span><span class="sxs-lookup"><span data-stu-id="c20e5-138">description</span></span>|<span data-ttu-id="c20e5-139">String</span><span class="sxs-lookup"><span data-stu-id="c20e5-139">String</span></span>|<span data-ttu-id="c20e5-140">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c20e5-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c20e5-141">priority</span><span class="sxs-lookup"><span data-stu-id="c20e5-141">priority</span></span>|<span data-ttu-id="c20e5-142">Int32</span><span class="sxs-lookup"><span data-stu-id="c20e5-142">Int32</span></span>|<span data-ttu-id="c20e5-143">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c20e5-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c20e5-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c20e5-144">createdDateTime</span></span>|<span data-ttu-id="c20e5-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c20e5-145">DateTimeOffset</span></span>|<span data-ttu-id="c20e5-146">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c20e5-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c20e5-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c20e5-147">lastModifiedDateTime</span></span>|<span data-ttu-id="c20e5-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c20e5-148">DateTimeOffset</span></span>|<span data-ttu-id="c20e5-149">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c20e5-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c20e5-150">version</span><span class="sxs-lookup"><span data-stu-id="c20e5-150">version</span></span>|<span data-ttu-id="c20e5-151">Int32</span><span class="sxs-lookup"><span data-stu-id="c20e5-151">Int32</span></span>|<span data-ttu-id="c20e5-152">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c20e5-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="c20e5-153">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c20e5-153">pinMinimumLength</span></span>|<span data-ttu-id="c20e5-154">Int32</span><span class="sxs-lookup"><span data-stu-id="c20e5-154">Int32</span></span>|<span data-ttu-id="c20e5-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c20e5-155">Not yet documented</span></span>|
|<span data-ttu-id="c20e5-156">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="c20e5-156">pinMaximumLength</span></span>|<span data-ttu-id="c20e5-157">Int32</span><span class="sxs-lookup"><span data-stu-id="c20e5-157">Int32</span></span>|<span data-ttu-id="c20e5-158">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c20e5-158">Not yet documented</span></span>|
|<span data-ttu-id="c20e5-159">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="c20e5-159">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="c20e5-160">виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="c20e5-160">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="c20e5-161">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c20e5-161">Not yet documented.</span></span> <span data-ttu-id="c20e5-162">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="c20e5-162">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="c20e5-163">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="c20e5-163">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="c20e5-164">виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="c20e5-164">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="c20e5-165">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c20e5-165">Not yet documented.</span></span> <span data-ttu-id="c20e5-166">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="c20e5-166">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="c20e5-167">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="c20e5-167">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="c20e5-168">виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="c20e5-168">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="c20e5-169">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c20e5-169">Not yet documented.</span></span> <span data-ttu-id="c20e5-170">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="c20e5-170">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="c20e5-171">state</span><span class="sxs-lookup"><span data-stu-id="c20e5-171">state</span></span>|[<span data-ttu-id="c20e5-172">Включение</span><span class="sxs-lookup"><span data-stu-id="c20e5-172">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="c20e5-173">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c20e5-173">Not yet documented.</span></span> <span data-ttu-id="c20e5-174">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="c20e5-174">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="c20e5-175">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="c20e5-175">securityDeviceRequired</span></span>|<span data-ttu-id="c20e5-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="c20e5-176">Boolean</span></span>|<span data-ttu-id="c20e5-177">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c20e5-177">Not yet documented</span></span>|
|<span data-ttu-id="c20e5-178">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="c20e5-178">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="c20e5-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="c20e5-179">Boolean</span></span>|<span data-ttu-id="c20e5-180">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c20e5-180">Not yet documented</span></span>|
|<span data-ttu-id="c20e5-181">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="c20e5-181">remotePassportEnabled</span></span>|<span data-ttu-id="c20e5-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="c20e5-182">Boolean</span></span>|<span data-ttu-id="c20e5-183">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c20e5-183">Not yet documented</span></span>|
|<span data-ttu-id="c20e5-184">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="c20e5-184">pinPreviousBlockCount</span></span>|<span data-ttu-id="c20e5-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c20e5-185">Int32</span></span>|<span data-ttu-id="c20e5-186">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c20e5-186">Not yet documented</span></span>|
|<span data-ttu-id="c20e5-187">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="c20e5-187">pinExpirationInDays</span></span>|<span data-ttu-id="c20e5-188">Int32</span><span class="sxs-lookup"><span data-stu-id="c20e5-188">Int32</span></span>|<span data-ttu-id="c20e5-189">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c20e5-189">Not yet documented</span></span>|
|<span data-ttu-id="c20e5-190">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="c20e5-190">enhancedBiometricsState</span></span>|[<span data-ttu-id="c20e5-191">Включение</span><span class="sxs-lookup"><span data-stu-id="c20e5-191">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="c20e5-192">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="c20e5-192">Not yet documented.</span></span> <span data-ttu-id="c20e5-193">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="c20e5-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="c20e5-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="c20e5-194">Response</span></span>
<span data-ttu-id="c20e5-195">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c20e5-195">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c20e5-196">Пример</span><span class="sxs-lookup"><span data-stu-id="c20e5-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="c20e5-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="c20e5-197">Request</span></span>
<span data-ttu-id="c20e5-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c20e5-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c20e5-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="c20e5-199">Response</span></span>
<span data-ttu-id="c20e5-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c20e5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




