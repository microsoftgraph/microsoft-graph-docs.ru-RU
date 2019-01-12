---
title: Обновление deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Обновление свойств объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b5e5cd09ba2e3246eccb4a0984cf2086209be3da
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913585"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="a4aba-103">Обновление deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="a4aba-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="a4aba-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a4aba-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4aba-105">Обновление свойств объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4aba-105">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a4aba-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a4aba-106">Prerequisites</span></span>
<span data-ttu-id="a4aba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4aba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4aba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4aba-109">Permission type</span></span>|<span data-ttu-id="a4aba-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4aba-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4aba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4aba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a4aba-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4aba-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a4aba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4aba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4aba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4aba-114">Not supported.</span></span>|
|<span data-ttu-id="a4aba-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4aba-115">Application</span></span>|<span data-ttu-id="a4aba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4aba-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4aba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4aba-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a4aba-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4aba-118">Request headers</span></span>
|<span data-ttu-id="a4aba-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4aba-119">Header</span></span>|<span data-ttu-id="a4aba-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a4aba-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4aba-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4aba-121">Authorization</span></span>|<span data-ttu-id="a4aba-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a4aba-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4aba-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a4aba-123">Accept</span></span>|<span data-ttu-id="a4aba-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a4aba-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4aba-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a4aba-125">Request body</span></span>
<span data-ttu-id="a4aba-126">В теле запроса добавьте представление объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4aba-126">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="a4aba-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4aba-127">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="a4aba-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4aba-128">Property</span></span>|<span data-ttu-id="a4aba-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a4aba-129">Type</span></span>|<span data-ttu-id="a4aba-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a4aba-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4aba-131">id</span><span class="sxs-lookup"><span data-stu-id="a4aba-131">id</span></span>|<span data-ttu-id="a4aba-132">String</span><span class="sxs-lookup"><span data-stu-id="a4aba-132">String</span></span>|<span data-ttu-id="a4aba-133">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4aba-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a4aba-134">displayName</span><span class="sxs-lookup"><span data-stu-id="a4aba-134">displayName</span></span>|<span data-ttu-id="a4aba-135">String</span><span class="sxs-lookup"><span data-stu-id="a4aba-135">String</span></span>|<span data-ttu-id="a4aba-136">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4aba-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a4aba-137">описание</span><span class="sxs-lookup"><span data-stu-id="a4aba-137">description</span></span>|<span data-ttu-id="a4aba-138">String</span><span class="sxs-lookup"><span data-stu-id="a4aba-138">String</span></span>|<span data-ttu-id="a4aba-139">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4aba-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a4aba-140">priority</span><span class="sxs-lookup"><span data-stu-id="a4aba-140">priority</span></span>|<span data-ttu-id="a4aba-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a4aba-141">Int32</span></span>|<span data-ttu-id="a4aba-142">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4aba-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a4aba-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4aba-143">createdDateTime</span></span>|<span data-ttu-id="a4aba-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4aba-144">DateTimeOffset</span></span>|<span data-ttu-id="a4aba-145">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4aba-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a4aba-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4aba-146">lastModifiedDateTime</span></span>|<span data-ttu-id="a4aba-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4aba-147">DateTimeOffset</span></span>|<span data-ttu-id="a4aba-148">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a4aba-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a4aba-149">version</span><span class="sxs-lookup"><span data-stu-id="a4aba-149">version</span></span>|<span data-ttu-id="a4aba-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a4aba-150">Int32</span></span>|<span data-ttu-id="a4aba-151">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a4aba-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a4aba-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a4aba-152">pinMinimumLength</span></span>|<span data-ttu-id="a4aba-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a4aba-153">Int32</span></span>|<span data-ttu-id="a4aba-154">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a4aba-154">Not yet documented</span></span>|
|<span data-ttu-id="a4aba-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="a4aba-155">pinMaximumLength</span></span>|<span data-ttu-id="a4aba-156">Int32</span><span class="sxs-lookup"><span data-stu-id="a4aba-156">Int32</span></span>|<span data-ttu-id="a4aba-157">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a4aba-157">Not yet documented</span></span>|
|<span data-ttu-id="a4aba-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a4aba-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="a4aba-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="a4aba-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="a4aba-160">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="a4aba-160">Not yet documented.</span></span> <span data-ttu-id="a4aba-161">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="a4aba-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="a4aba-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a4aba-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="a4aba-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="a4aba-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="a4aba-164">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="a4aba-164">Not yet documented.</span></span> <span data-ttu-id="a4aba-165">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="a4aba-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="a4aba-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a4aba-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="a4aba-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="a4aba-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="a4aba-168">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="a4aba-168">Not yet documented.</span></span> <span data-ttu-id="a4aba-169">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="a4aba-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="a4aba-170">state</span><span class="sxs-lookup"><span data-stu-id="a4aba-170">state</span></span>|[<span data-ttu-id="a4aba-171">Включение</span><span class="sxs-lookup"><span data-stu-id="a4aba-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="a4aba-172">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="a4aba-172">Not yet documented.</span></span> <span data-ttu-id="a4aba-173">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="a4aba-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a4aba-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="a4aba-174">securityDeviceRequired</span></span>|<span data-ttu-id="a4aba-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4aba-175">Boolean</span></span>|<span data-ttu-id="a4aba-176">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a4aba-176">Not yet documented</span></span>|
|<span data-ttu-id="a4aba-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="a4aba-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="a4aba-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4aba-178">Boolean</span></span>|<span data-ttu-id="a4aba-179">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a4aba-179">Not yet documented</span></span>|
|<span data-ttu-id="a4aba-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="a4aba-180">remotePassportEnabled</span></span>|<span data-ttu-id="a4aba-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4aba-181">Boolean</span></span>|<span data-ttu-id="a4aba-182">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a4aba-182">Not yet documented</span></span>|
|<span data-ttu-id="a4aba-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="a4aba-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="a4aba-184">Int32</span><span class="sxs-lookup"><span data-stu-id="a4aba-184">Int32</span></span>|<span data-ttu-id="a4aba-185">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a4aba-185">Not yet documented</span></span>|
|<span data-ttu-id="a4aba-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="a4aba-186">pinExpirationInDays</span></span>|<span data-ttu-id="a4aba-187">Int32</span><span class="sxs-lookup"><span data-stu-id="a4aba-187">Int32</span></span>|<span data-ttu-id="a4aba-188">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a4aba-188">Not yet documented</span></span>|
|<span data-ttu-id="a4aba-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="a4aba-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="a4aba-190">Включение</span><span class="sxs-lookup"><span data-stu-id="a4aba-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="a4aba-191">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="a4aba-191">Not yet documented.</span></span> <span data-ttu-id="a4aba-192">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="a4aba-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="a4aba-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4aba-193">Response</span></span>
<span data-ttu-id="a4aba-194">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a4aba-194">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4aba-195">Пример</span><span class="sxs-lookup"><span data-stu-id="a4aba-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="a4aba-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4aba-196">Request</span></span>
<span data-ttu-id="a4aba-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4aba-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a4aba-198">Ответ</span><span class="sxs-lookup"><span data-stu-id="a4aba-198">Response</span></span>
<span data-ttu-id="a4aba-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a4aba-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



