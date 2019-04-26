---
title: Создание deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Создание объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11d5377c815b4c6711937b858d9e903f6e99e659
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561644"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="be16d-103">Создание deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="be16d-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="be16d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be16d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be16d-105">Создание объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be16d-105">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be16d-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="be16d-106">Prerequisites</span></span>
<span data-ttu-id="be16d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be16d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be16d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be16d-109">Permission type</span></span>|<span data-ttu-id="be16d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be16d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be16d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be16d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="be16d-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be16d-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="be16d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be16d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be16d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be16d-114">Not supported.</span></span>|
|<span data-ttu-id="be16d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be16d-115">Application</span></span>|<span data-ttu-id="be16d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be16d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be16d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be16d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="be16d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be16d-118">Request headers</span></span>
|<span data-ttu-id="be16d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be16d-119">Header</span></span>|<span data-ttu-id="be16d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="be16d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be16d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be16d-121">Authorization</span></span>|<span data-ttu-id="be16d-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be16d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be16d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="be16d-123">Accept</span></span>|<span data-ttu-id="be16d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="be16d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be16d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be16d-125">Request body</span></span>
<span data-ttu-id="be16d-126">В теле запроса добавьте представление объекта deviceEnrollmentWindowsHelloForBusinessConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be16d-126">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="be16d-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="be16d-127">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="be16d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="be16d-128">Property</span></span>|<span data-ttu-id="be16d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="be16d-129">Type</span></span>|<span data-ttu-id="be16d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="be16d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be16d-131">id</span><span class="sxs-lookup"><span data-stu-id="be16d-131">id</span></span>|<span data-ttu-id="be16d-132">Строка</span><span class="sxs-lookup"><span data-stu-id="be16d-132">String</span></span>|<span data-ttu-id="be16d-133">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be16d-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="be16d-134">displayName</span><span class="sxs-lookup"><span data-stu-id="be16d-134">displayName</span></span>|<span data-ttu-id="be16d-135">String</span><span class="sxs-lookup"><span data-stu-id="be16d-135">String</span></span>|<span data-ttu-id="be16d-136">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be16d-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="be16d-137">description</span><span class="sxs-lookup"><span data-stu-id="be16d-137">description</span></span>|<span data-ttu-id="be16d-138">String</span><span class="sxs-lookup"><span data-stu-id="be16d-138">String</span></span>|<span data-ttu-id="be16d-139">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be16d-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="be16d-140">priority</span><span class="sxs-lookup"><span data-stu-id="be16d-140">priority</span></span>|<span data-ttu-id="be16d-141">Int32</span><span class="sxs-lookup"><span data-stu-id="be16d-141">Int32</span></span>|<span data-ttu-id="be16d-142">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be16d-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="be16d-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be16d-143">createdDateTime</span></span>|<span data-ttu-id="be16d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be16d-144">DateTimeOffset</span></span>|<span data-ttu-id="be16d-145">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be16d-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="be16d-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be16d-146">lastModifiedDateTime</span></span>|<span data-ttu-id="be16d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be16d-147">DateTimeOffset</span></span>|<span data-ttu-id="be16d-148">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be16d-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="be16d-149">version</span><span class="sxs-lookup"><span data-stu-id="be16d-149">version</span></span>|<span data-ttu-id="be16d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="be16d-150">Int32</span></span>|<span data-ttu-id="be16d-151">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be16d-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="be16d-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="be16d-152">pinMinimumLength</span></span>|<span data-ttu-id="be16d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="be16d-153">Int32</span></span>|<span data-ttu-id="be16d-154">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="be16d-154">Not yet documented</span></span>|
|<span data-ttu-id="be16d-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="be16d-155">pinMaximumLength</span></span>|<span data-ttu-id="be16d-156">Int32</span><span class="sxs-lookup"><span data-stu-id="be16d-156">Int32</span></span>|<span data-ttu-id="be16d-157">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="be16d-157">Not yet documented</span></span>|
|<span data-ttu-id="be16d-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="be16d-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="be16d-159">Виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="be16d-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="be16d-160">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="be16d-160">Not yet documented.</span></span> <span data-ttu-id="be16d-161">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="be16d-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="be16d-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="be16d-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="be16d-163">Виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="be16d-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="be16d-164">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="be16d-164">Not yet documented.</span></span> <span data-ttu-id="be16d-165">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="be16d-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="be16d-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="be16d-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="be16d-167">Виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="be16d-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="be16d-168">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="be16d-168">Not yet documented.</span></span> <span data-ttu-id="be16d-169">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="be16d-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="be16d-170">state</span><span class="sxs-lookup"><span data-stu-id="be16d-170">state</span></span>|[<span data-ttu-id="be16d-171">Включение</span><span class="sxs-lookup"><span data-stu-id="be16d-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="be16d-172">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="be16d-172">Not yet documented.</span></span> <span data-ttu-id="be16d-173">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="be16d-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="be16d-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="be16d-174">securityDeviceRequired</span></span>|<span data-ttu-id="be16d-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="be16d-175">Boolean</span></span>|<span data-ttu-id="be16d-176">Н/Д</span><span class="sxs-lookup"><span data-stu-id="be16d-176">Not yet documented</span></span>|
|<span data-ttu-id="be16d-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="be16d-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="be16d-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="be16d-178">Boolean</span></span>|<span data-ttu-id="be16d-179">Н/Д</span><span class="sxs-lookup"><span data-stu-id="be16d-179">Not yet documented</span></span>|
|<span data-ttu-id="be16d-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="be16d-180">remotePassportEnabled</span></span>|<span data-ttu-id="be16d-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="be16d-181">Boolean</span></span>|<span data-ttu-id="be16d-182">Н/Д</span><span class="sxs-lookup"><span data-stu-id="be16d-182">Not yet documented</span></span>|
|<span data-ttu-id="be16d-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="be16d-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="be16d-184">Int32</span><span class="sxs-lookup"><span data-stu-id="be16d-184">Int32</span></span>|<span data-ttu-id="be16d-185">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="be16d-185">Not yet documented</span></span>|
|<span data-ttu-id="be16d-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="be16d-186">pinExpirationInDays</span></span>|<span data-ttu-id="be16d-187">Int32</span><span class="sxs-lookup"><span data-stu-id="be16d-187">Int32</span></span>|<span data-ttu-id="be16d-188">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="be16d-188">Not yet documented</span></span>|
|<span data-ttu-id="be16d-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="be16d-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="be16d-190">Включение</span><span class="sxs-lookup"><span data-stu-id="be16d-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="be16d-191">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="be16d-191">Not yet documented.</span></span> <span data-ttu-id="be16d-192">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="be16d-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="be16d-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="be16d-193">Response</span></span>
<span data-ttu-id="be16d-194">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="be16d-194">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be16d-195">Пример</span><span class="sxs-lookup"><span data-stu-id="be16d-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="be16d-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="be16d-196">Request</span></span>
<span data-ttu-id="be16d-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be16d-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="be16d-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="be16d-198">Response</span></span>
<span data-ttu-id="be16d-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be16d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



