---
title: Создание deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Создание объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: df1f1c4ddae90e05c7268276379598dbdd0e4481
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43369277"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="cd8f1-103">Создание deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd8f1-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

<span data-ttu-id="cd8f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd8f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd8f1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd8f1-106">Создание объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cd8f1-106">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd8f1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cd8f1-107">Prerequisites</span></span>
<span data-ttu-id="cd8f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd8f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd8f1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd8f1-110">Permission type</span></span>|<span data-ttu-id="cd8f1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd8f1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd8f1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd8f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd8f1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd8f1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cd8f1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd8f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd8f1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-115">Not supported.</span></span>|
|<span data-ttu-id="cd8f1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd8f1-116">Application</span></span>|<span data-ttu-id="cd8f1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd8f1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd8f1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cd8f1-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cd8f1-119">Request headers</span></span>
|<span data-ttu-id="cd8f1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd8f1-120">Header</span></span>|<span data-ttu-id="cd8f1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cd8f1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd8f1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd8f1-122">Authorization</span></span>|<span data-ttu-id="cd8f1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd8f1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cd8f1-124">Accept</span></span>|<span data-ttu-id="cd8f1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd8f1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd8f1-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cd8f1-126">Request body</span></span>
<span data-ttu-id="cd8f1-127">В теле запроса добавьте представление объекта deviceEnrollmentWindowsHelloForBusinessConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-127">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="cd8f1-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-128">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="cd8f1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd8f1-129">Property</span></span>|<span data-ttu-id="cd8f1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cd8f1-130">Type</span></span>|<span data-ttu-id="cd8f1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cd8f1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd8f1-132">id</span><span class="sxs-lookup"><span data-stu-id="cd8f1-132">id</span></span>|<span data-ttu-id="cd8f1-133">String</span><span class="sxs-lookup"><span data-stu-id="cd8f1-133">String</span></span>|<span data-ttu-id="cd8f1-134">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd8f1-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cd8f1-135">displayName</span><span class="sxs-lookup"><span data-stu-id="cd8f1-135">displayName</span></span>|<span data-ttu-id="cd8f1-136">Строка</span><span class="sxs-lookup"><span data-stu-id="cd8f1-136">String</span></span>|<span data-ttu-id="cd8f1-137">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd8f1-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cd8f1-138">description</span><span class="sxs-lookup"><span data-stu-id="cd8f1-138">description</span></span>|<span data-ttu-id="cd8f1-139">String</span><span class="sxs-lookup"><span data-stu-id="cd8f1-139">String</span></span>|<span data-ttu-id="cd8f1-140">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd8f1-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cd8f1-141">priority</span><span class="sxs-lookup"><span data-stu-id="cd8f1-141">priority</span></span>|<span data-ttu-id="cd8f1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="cd8f1-142">Int32</span></span>|<span data-ttu-id="cd8f1-143">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd8f1-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cd8f1-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd8f1-144">createdDateTime</span></span>|<span data-ttu-id="cd8f1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd8f1-145">DateTimeOffset</span></span>|<span data-ttu-id="cd8f1-146">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd8f1-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cd8f1-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cd8f1-147">lastModifiedDateTime</span></span>|<span data-ttu-id="cd8f1-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd8f1-148">DateTimeOffset</span></span>|<span data-ttu-id="cd8f1-149">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cd8f1-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cd8f1-150">version</span><span class="sxs-lookup"><span data-stu-id="cd8f1-150">version</span></span>|<span data-ttu-id="cd8f1-151">Int32</span><span class="sxs-lookup"><span data-stu-id="cd8f1-151">Int32</span></span>|<span data-ttu-id="cd8f1-152">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cd8f1-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="cd8f1-153">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="cd8f1-153">pinMinimumLength</span></span>|<span data-ttu-id="cd8f1-154">Int32</span><span class="sxs-lookup"><span data-stu-id="cd8f1-154">Int32</span></span>|<span data-ttu-id="cd8f1-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-155">Not yet documented</span></span>|
|<span data-ttu-id="cd8f1-156">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="cd8f1-156">pinMaximumLength</span></span>|<span data-ttu-id="cd8f1-157">Int32</span><span class="sxs-lookup"><span data-stu-id="cd8f1-157">Int32</span></span>|<span data-ttu-id="cd8f1-158">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-158">Not yet documented</span></span>|
|<span data-ttu-id="cd8f1-159">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="cd8f1-159">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="cd8f1-160">виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="cd8f1-160">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="cd8f1-161">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-161">Not yet documented.</span></span> <span data-ttu-id="cd8f1-162">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-162">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="cd8f1-163">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="cd8f1-163">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="cd8f1-164">виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="cd8f1-164">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="cd8f1-165">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-165">Not yet documented.</span></span> <span data-ttu-id="cd8f1-166">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-166">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="cd8f1-167">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="cd8f1-167">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="cd8f1-168">виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="cd8f1-168">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="cd8f1-169">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-169">Not yet documented.</span></span> <span data-ttu-id="cd8f1-170">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-170">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="cd8f1-171">state</span><span class="sxs-lookup"><span data-stu-id="cd8f1-171">state</span></span>|[<span data-ttu-id="cd8f1-172">Включение</span><span class="sxs-lookup"><span data-stu-id="cd8f1-172">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="cd8f1-173">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-173">Not yet documented.</span></span> <span data-ttu-id="cd8f1-174">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-174">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="cd8f1-175">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="cd8f1-175">securityDeviceRequired</span></span>|<span data-ttu-id="cd8f1-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd8f1-176">Boolean</span></span>|<span data-ttu-id="cd8f1-177">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cd8f1-177">Not yet documented</span></span>|
|<span data-ttu-id="cd8f1-178">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="cd8f1-178">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="cd8f1-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd8f1-179">Boolean</span></span>|<span data-ttu-id="cd8f1-180">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cd8f1-180">Not yet documented</span></span>|
|<span data-ttu-id="cd8f1-181">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="cd8f1-181">remotePassportEnabled</span></span>|<span data-ttu-id="cd8f1-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd8f1-182">Boolean</span></span>|<span data-ttu-id="cd8f1-183">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cd8f1-183">Not yet documented</span></span>|
|<span data-ttu-id="cd8f1-184">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="cd8f1-184">pinPreviousBlockCount</span></span>|<span data-ttu-id="cd8f1-185">Int32</span><span class="sxs-lookup"><span data-stu-id="cd8f1-185">Int32</span></span>|<span data-ttu-id="cd8f1-186">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-186">Not yet documented</span></span>|
|<span data-ttu-id="cd8f1-187">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="cd8f1-187">pinExpirationInDays</span></span>|<span data-ttu-id="cd8f1-188">Int32</span><span class="sxs-lookup"><span data-stu-id="cd8f1-188">Int32</span></span>|<span data-ttu-id="cd8f1-189">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-189">Not yet documented</span></span>|
|<span data-ttu-id="cd8f1-190">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="cd8f1-190">enhancedBiometricsState</span></span>|[<span data-ttu-id="cd8f1-191">Включение</span><span class="sxs-lookup"><span data-stu-id="cd8f1-191">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="cd8f1-192">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-192">Not yet documented.</span></span> <span data-ttu-id="cd8f1-193">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="cd8f1-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd8f1-194">Response</span></span>
<span data-ttu-id="cd8f1-195">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-195">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd8f1-196">Пример</span><span class="sxs-lookup"><span data-stu-id="cd8f1-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd8f1-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd8f1-197">Request</span></span>
<span data-ttu-id="cd8f1-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="cd8f1-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd8f1-199">Response</span></span>
<span data-ttu-id="cd8f1-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd8f1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






