---
title: Обновление deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Обновление свойств объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
ms.openlocfilehash: 44624aaf7f073d67f8623bdaee8266c80596a90d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076058"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="fbd30-103">Обновление deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="fbd30-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="fbd30-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fbd30-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbd30-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbd30-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbd30-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fbd30-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbd30-107">Обновление свойств объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd30-107">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fbd30-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fbd30-108">Prerequisites</span></span>
<span data-ttu-id="fbd30-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbd30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbd30-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbd30-111">Permission type</span></span>|<span data-ttu-id="fbd30-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbd30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbd30-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbd30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbd30-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbd30-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fbd30-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbd30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbd30-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbd30-116">Not supported.</span></span>|
|<span data-ttu-id="fbd30-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbd30-117">Application</span></span>|<span data-ttu-id="fbd30-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbd30-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbd30-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbd30-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fbd30-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fbd30-120">Request headers</span></span>
|<span data-ttu-id="fbd30-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fbd30-121">Header</span></span>|<span data-ttu-id="fbd30-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fbd30-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbd30-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbd30-123">Authorization</span></span>|<span data-ttu-id="fbd30-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fbd30-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbd30-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fbd30-125">Accept</span></span>|<span data-ttu-id="fbd30-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbd30-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbd30-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fbd30-127">Request body</span></span>
<span data-ttu-id="fbd30-128">В теле запроса добавьте представление объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbd30-128">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="fbd30-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd30-129">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="fbd30-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbd30-130">Property</span></span>|<span data-ttu-id="fbd30-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fbd30-131">Type</span></span>|<span data-ttu-id="fbd30-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fbd30-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbd30-133">id</span><span class="sxs-lookup"><span data-stu-id="fbd30-133">id</span></span>|<span data-ttu-id="fbd30-134">String</span><span class="sxs-lookup"><span data-stu-id="fbd30-134">String</span></span>|<span data-ttu-id="fbd30-135">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd30-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fbd30-136">displayName</span><span class="sxs-lookup"><span data-stu-id="fbd30-136">displayName</span></span>|<span data-ttu-id="fbd30-137">String</span><span class="sxs-lookup"><span data-stu-id="fbd30-137">String</span></span>|<span data-ttu-id="fbd30-138">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd30-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fbd30-139">описание</span><span class="sxs-lookup"><span data-stu-id="fbd30-139">description</span></span>|<span data-ttu-id="fbd30-140">String</span><span class="sxs-lookup"><span data-stu-id="fbd30-140">String</span></span>|<span data-ttu-id="fbd30-141">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd30-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fbd30-142">priority</span><span class="sxs-lookup"><span data-stu-id="fbd30-142">priority</span></span>|<span data-ttu-id="fbd30-143">Int32</span><span class="sxs-lookup"><span data-stu-id="fbd30-143">Int32</span></span>|<span data-ttu-id="fbd30-144">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd30-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fbd30-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fbd30-145">createdDateTime</span></span>|<span data-ttu-id="fbd30-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbd30-146">DateTimeOffset</span></span>|<span data-ttu-id="fbd30-147">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd30-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fbd30-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbd30-148">lastModifiedDateTime</span></span>|<span data-ttu-id="fbd30-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbd30-149">DateTimeOffset</span></span>|<span data-ttu-id="fbd30-150">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbd30-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fbd30-151">version</span><span class="sxs-lookup"><span data-stu-id="fbd30-151">version</span></span>|<span data-ttu-id="fbd30-152">Int32</span><span class="sxs-lookup"><span data-stu-id="fbd30-152">Int32</span></span>|<span data-ttu-id="fbd30-153">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fbd30-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="fbd30-154">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="fbd30-154">pinMinimumLength</span></span>|<span data-ttu-id="fbd30-155">Int32</span><span class="sxs-lookup"><span data-stu-id="fbd30-155">Int32</span></span>|<span data-ttu-id="fbd30-156">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fbd30-156">Not yet documented</span></span>|
|<span data-ttu-id="fbd30-157">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="fbd30-157">pinMaximumLength</span></span>|<span data-ttu-id="fbd30-158">Int32</span><span class="sxs-lookup"><span data-stu-id="fbd30-158">Int32</span></span>|<span data-ttu-id="fbd30-159">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fbd30-159">Not yet documented</span></span>|
|<span data-ttu-id="fbd30-160">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="fbd30-160">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="fbd30-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="fbd30-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="fbd30-162">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="fbd30-162">Not yet documented.</span></span> <span data-ttu-id="fbd30-163">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="fbd30-163">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="fbd30-164">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="fbd30-164">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="fbd30-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="fbd30-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="fbd30-166">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="fbd30-166">Not yet documented.</span></span> <span data-ttu-id="fbd30-167">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="fbd30-167">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="fbd30-168">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="fbd30-168">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="fbd30-169">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="fbd30-169">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="fbd30-170">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="fbd30-170">Not yet documented.</span></span> <span data-ttu-id="fbd30-171">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="fbd30-171">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="fbd30-172">state</span><span class="sxs-lookup"><span data-stu-id="fbd30-172">state</span></span>|[<span data-ttu-id="fbd30-173">Включение</span><span class="sxs-lookup"><span data-stu-id="fbd30-173">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="fbd30-174">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="fbd30-174">Not yet documented.</span></span> <span data-ttu-id="fbd30-175">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="fbd30-175">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="fbd30-176">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="fbd30-176">securityDeviceRequired</span></span>|<span data-ttu-id="fbd30-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbd30-177">Boolean</span></span>|<span data-ttu-id="fbd30-178">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fbd30-178">Not yet documented</span></span>|
|<span data-ttu-id="fbd30-179">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="fbd30-179">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="fbd30-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbd30-180">Boolean</span></span>|<span data-ttu-id="fbd30-181">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fbd30-181">Not yet documented</span></span>|
|<span data-ttu-id="fbd30-182">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="fbd30-182">remotePassportEnabled</span></span>|<span data-ttu-id="fbd30-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbd30-183">Boolean</span></span>|<span data-ttu-id="fbd30-184">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fbd30-184">Not yet documented</span></span>|
|<span data-ttu-id="fbd30-185">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="fbd30-185">pinPreviousBlockCount</span></span>|<span data-ttu-id="fbd30-186">Int32</span><span class="sxs-lookup"><span data-stu-id="fbd30-186">Int32</span></span>|<span data-ttu-id="fbd30-187">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fbd30-187">Not yet documented</span></span>|
|<span data-ttu-id="fbd30-188">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="fbd30-188">pinExpirationInDays</span></span>|<span data-ttu-id="fbd30-189">Int32</span><span class="sxs-lookup"><span data-stu-id="fbd30-189">Int32</span></span>|<span data-ttu-id="fbd30-190">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fbd30-190">Not yet documented</span></span>|
|<span data-ttu-id="fbd30-191">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="fbd30-191">enhancedBiometricsState</span></span>|[<span data-ttu-id="fbd30-192">Включение</span><span class="sxs-lookup"><span data-stu-id="fbd30-192">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="fbd30-193">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="fbd30-193">Not yet documented.</span></span> <span data-ttu-id="fbd30-194">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="fbd30-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="fbd30-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbd30-195">Response</span></span>
<span data-ttu-id="fbd30-196">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fbd30-196">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbd30-197">Пример</span><span class="sxs-lookup"><span data-stu-id="fbd30-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="fbd30-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbd30-198">Request</span></span>
<span data-ttu-id="fbd30-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbd30-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 602

{
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
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

### <a name="response"></a><span data-ttu-id="fbd30-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="fbd30-200">Response</span></span>
<span data-ttu-id="fbd30-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="fbd30-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





