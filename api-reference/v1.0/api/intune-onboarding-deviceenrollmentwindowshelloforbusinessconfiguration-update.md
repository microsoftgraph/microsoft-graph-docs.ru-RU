---
title: Обновление deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Обновление свойств объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3225f7fe36f5ec8a66df8424a06d8569b7c92efd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968639"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="7c0e5-103">Обновление deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c0e5-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="7c0e5-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c0e5-105">Обновление свойств объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c0e5-105">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c0e5-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7c0e5-106">Prerequisites</span></span>
<span data-ttu-id="7c0e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c0e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c0e5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c0e5-109">Permission type</span></span>|<span data-ttu-id="7c0e5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c0e5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c0e5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c0e5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7c0e5-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c0e5-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7c0e5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c0e5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c0e5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-114">Not supported.</span></span>|
|<span data-ttu-id="7c0e5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c0e5-115">Application</span></span>|<span data-ttu-id="7c0e5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c0e5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c0e5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7c0e5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c0e5-118">Request headers</span></span>
|<span data-ttu-id="7c0e5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c0e5-119">Header</span></span>|<span data-ttu-id="7c0e5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7c0e5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c0e5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c0e5-121">Authorization</span></span>|<span data-ttu-id="7c0e5-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c0e5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7c0e5-123">Accept</span></span>|<span data-ttu-id="7c0e5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7c0e5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c0e5-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c0e5-125">Request body</span></span>
<span data-ttu-id="7c0e5-126">В теле запроса добавьте представление объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-126">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="7c0e5-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c0e5-127">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="7c0e5-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c0e5-128">Property</span></span>|<span data-ttu-id="7c0e5-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7c0e5-129">Type</span></span>|<span data-ttu-id="7c0e5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7c0e5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c0e5-131">id</span><span class="sxs-lookup"><span data-stu-id="7c0e5-131">id</span></span>|<span data-ttu-id="7c0e5-132">Строка</span><span class="sxs-lookup"><span data-stu-id="7c0e5-132">String</span></span>|<span data-ttu-id="7c0e5-133">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c0e5-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c0e5-134">displayName</span><span class="sxs-lookup"><span data-stu-id="7c0e5-134">displayName</span></span>|<span data-ttu-id="7c0e5-135">String</span><span class="sxs-lookup"><span data-stu-id="7c0e5-135">String</span></span>|<span data-ttu-id="7c0e5-136">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c0e5-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c0e5-137">description</span><span class="sxs-lookup"><span data-stu-id="7c0e5-137">description</span></span>|<span data-ttu-id="7c0e5-138">String</span><span class="sxs-lookup"><span data-stu-id="7c0e5-138">String</span></span>|<span data-ttu-id="7c0e5-139">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c0e5-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c0e5-140">priority</span><span class="sxs-lookup"><span data-stu-id="7c0e5-140">priority</span></span>|<span data-ttu-id="7c0e5-141">Int32</span><span class="sxs-lookup"><span data-stu-id="7c0e5-141">Int32</span></span>|<span data-ttu-id="7c0e5-142">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c0e5-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c0e5-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c0e5-143">createdDateTime</span></span>|<span data-ttu-id="7c0e5-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c0e5-144">DateTimeOffset</span></span>|<span data-ttu-id="7c0e5-145">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c0e5-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c0e5-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c0e5-146">lastModifiedDateTime</span></span>|<span data-ttu-id="7c0e5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c0e5-147">DateTimeOffset</span></span>|<span data-ttu-id="7c0e5-148">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c0e5-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c0e5-149">version</span><span class="sxs-lookup"><span data-stu-id="7c0e5-149">version</span></span>|<span data-ttu-id="7c0e5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7c0e5-150">Int32</span></span>|<span data-ttu-id="7c0e5-151">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c0e5-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="7c0e5-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7c0e5-152">pinMinimumLength</span></span>|<span data-ttu-id="7c0e5-153">Int32</span><span class="sxs-lookup"><span data-stu-id="7c0e5-153">Int32</span></span>|<span data-ttu-id="7c0e5-154">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-154">Not yet documented</span></span>|
|<span data-ttu-id="7c0e5-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="7c0e5-155">pinMaximumLength</span></span>|<span data-ttu-id="7c0e5-156">Int32</span><span class="sxs-lookup"><span data-stu-id="7c0e5-156">Int32</span></span>|<span data-ttu-id="7c0e5-157">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-157">Not yet documented</span></span>|
|<span data-ttu-id="7c0e5-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="7c0e5-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="7c0e5-159">Виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="7c0e5-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="7c0e5-160">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-160">Not yet documented.</span></span> <span data-ttu-id="7c0e5-161">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="7c0e5-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="7c0e5-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="7c0e5-163">Виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="7c0e5-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="7c0e5-164">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-164">Not yet documented.</span></span> <span data-ttu-id="7c0e5-165">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="7c0e5-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="7c0e5-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="7c0e5-167">Виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="7c0e5-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="7c0e5-168">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-168">Not yet documented.</span></span> <span data-ttu-id="7c0e5-169">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="7c0e5-170">state</span><span class="sxs-lookup"><span data-stu-id="7c0e5-170">state</span></span>|[<span data-ttu-id="7c0e5-171">Включение</span><span class="sxs-lookup"><span data-stu-id="7c0e5-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="7c0e5-172">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-172">Not yet documented.</span></span> <span data-ttu-id="7c0e5-173">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="7c0e5-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="7c0e5-174">securityDeviceRequired</span></span>|<span data-ttu-id="7c0e5-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c0e5-175">Boolean</span></span>|<span data-ttu-id="7c0e5-176">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7c0e5-176">Not yet documented</span></span>|
|<span data-ttu-id="7c0e5-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="7c0e5-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="7c0e5-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c0e5-178">Boolean</span></span>|<span data-ttu-id="7c0e5-179">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7c0e5-179">Not yet documented</span></span>|
|<span data-ttu-id="7c0e5-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="7c0e5-180">remotePassportEnabled</span></span>|<span data-ttu-id="7c0e5-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c0e5-181">Boolean</span></span>|<span data-ttu-id="7c0e5-182">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7c0e5-182">Not yet documented</span></span>|
|<span data-ttu-id="7c0e5-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="7c0e5-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="7c0e5-184">Int32</span><span class="sxs-lookup"><span data-stu-id="7c0e5-184">Int32</span></span>|<span data-ttu-id="7c0e5-185">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-185">Not yet documented</span></span>|
|<span data-ttu-id="7c0e5-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="7c0e5-186">pinExpirationInDays</span></span>|<span data-ttu-id="7c0e5-187">Int32</span><span class="sxs-lookup"><span data-stu-id="7c0e5-187">Int32</span></span>|<span data-ttu-id="7c0e5-188">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-188">Not yet documented</span></span>|
|<span data-ttu-id="7c0e5-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="7c0e5-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="7c0e5-190">Включение</span><span class="sxs-lookup"><span data-stu-id="7c0e5-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="7c0e5-191">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-191">Not yet documented.</span></span> <span data-ttu-id="7c0e5-192">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="7c0e5-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c0e5-193">Response</span></span>
<span data-ttu-id="7c0e5-194">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-194">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c0e5-195">Пример</span><span class="sxs-lookup"><span data-stu-id="7c0e5-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c0e5-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c0e5-196">Request</span></span>
<span data-ttu-id="7c0e5-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7c0e5-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c0e5-198">Response</span></span>
<span data-ttu-id="7c0e5-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c0e5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



