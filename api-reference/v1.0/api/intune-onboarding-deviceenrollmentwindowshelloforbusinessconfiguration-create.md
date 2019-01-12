---
title: Создание deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Создание объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f86fd9fc1a8028ab983dce46998046b1515c761
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983081"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="2b14f-103">Создание deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b14f-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="2b14f-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2b14f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b14f-105">Создание объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b14f-105">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2b14f-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2b14f-106">Prerequisites</span></span>
<span data-ttu-id="2b14f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b14f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b14f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b14f-109">Permission type</span></span>|<span data-ttu-id="2b14f-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b14f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b14f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b14f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2b14f-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b14f-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2b14f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b14f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b14f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b14f-114">Not supported.</span></span>|
|<span data-ttu-id="2b14f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b14f-115">Application</span></span>|<span data-ttu-id="2b14f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b14f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b14f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b14f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2b14f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b14f-118">Request headers</span></span>
|<span data-ttu-id="2b14f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b14f-119">Header</span></span>|<span data-ttu-id="2b14f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2b14f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b14f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b14f-121">Authorization</span></span>|<span data-ttu-id="2b14f-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2b14f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b14f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2b14f-123">Accept</span></span>|<span data-ttu-id="2b14f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2b14f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b14f-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2b14f-125">Request body</span></span>
<span data-ttu-id="2b14f-126">В теле запроса добавьте представление объекта deviceEnrollmentWindowsHelloForBusinessConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b14f-126">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="2b14f-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2b14f-127">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="2b14f-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b14f-128">Property</span></span>|<span data-ttu-id="2b14f-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2b14f-129">Type</span></span>|<span data-ttu-id="2b14f-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2b14f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b14f-131">id</span><span class="sxs-lookup"><span data-stu-id="2b14f-131">id</span></span>|<span data-ttu-id="2b14f-132">String</span><span class="sxs-lookup"><span data-stu-id="2b14f-132">String</span></span>|<span data-ttu-id="2b14f-133">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b14f-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2b14f-134">displayName</span><span class="sxs-lookup"><span data-stu-id="2b14f-134">displayName</span></span>|<span data-ttu-id="2b14f-135">String</span><span class="sxs-lookup"><span data-stu-id="2b14f-135">String</span></span>|<span data-ttu-id="2b14f-136">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b14f-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2b14f-137">описание</span><span class="sxs-lookup"><span data-stu-id="2b14f-137">description</span></span>|<span data-ttu-id="2b14f-138">String</span><span class="sxs-lookup"><span data-stu-id="2b14f-138">String</span></span>|<span data-ttu-id="2b14f-139">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b14f-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2b14f-140">priority</span><span class="sxs-lookup"><span data-stu-id="2b14f-140">priority</span></span>|<span data-ttu-id="2b14f-141">Int32</span><span class="sxs-lookup"><span data-stu-id="2b14f-141">Int32</span></span>|<span data-ttu-id="2b14f-142">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b14f-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2b14f-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b14f-143">createdDateTime</span></span>|<span data-ttu-id="2b14f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b14f-144">DateTimeOffset</span></span>|<span data-ttu-id="2b14f-145">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b14f-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2b14f-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b14f-146">lastModifiedDateTime</span></span>|<span data-ttu-id="2b14f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b14f-147">DateTimeOffset</span></span>|<span data-ttu-id="2b14f-148">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b14f-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2b14f-149">version</span><span class="sxs-lookup"><span data-stu-id="2b14f-149">version</span></span>|<span data-ttu-id="2b14f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="2b14f-150">Int32</span></span>|<span data-ttu-id="2b14f-151">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b14f-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="2b14f-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2b14f-152">pinMinimumLength</span></span>|<span data-ttu-id="2b14f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="2b14f-153">Int32</span></span>|<span data-ttu-id="2b14f-154">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2b14f-154">Not yet documented</span></span>|
|<span data-ttu-id="2b14f-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="2b14f-155">pinMaximumLength</span></span>|<span data-ttu-id="2b14f-156">Int32</span><span class="sxs-lookup"><span data-stu-id="2b14f-156">Int32</span></span>|<span data-ttu-id="2b14f-157">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2b14f-157">Not yet documented</span></span>|
|<span data-ttu-id="2b14f-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="2b14f-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="2b14f-159">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="2b14f-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="2b14f-160">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="2b14f-160">Not yet documented.</span></span> <span data-ttu-id="2b14f-161">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="2b14f-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="2b14f-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="2b14f-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="2b14f-163">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="2b14f-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="2b14f-164">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="2b14f-164">Not yet documented.</span></span> <span data-ttu-id="2b14f-165">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="2b14f-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="2b14f-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="2b14f-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="2b14f-167">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="2b14f-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="2b14f-168">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="2b14f-168">Not yet documented.</span></span> <span data-ttu-id="2b14f-169">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="2b14f-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="2b14f-170">состояние</span><span class="sxs-lookup"><span data-stu-id="2b14f-170">state</span></span>|[<span data-ttu-id="2b14f-171">Включение</span><span class="sxs-lookup"><span data-stu-id="2b14f-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="2b14f-172">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="2b14f-172">Not yet documented.</span></span> <span data-ttu-id="2b14f-173">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="2b14f-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="2b14f-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="2b14f-174">securityDeviceRequired</span></span>|<span data-ttu-id="2b14f-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b14f-175">Boolean</span></span>|<span data-ttu-id="2b14f-176">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2b14f-176">Not yet documented</span></span>|
|<span data-ttu-id="2b14f-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="2b14f-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="2b14f-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b14f-178">Boolean</span></span>|<span data-ttu-id="2b14f-179">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2b14f-179">Not yet documented</span></span>|
|<span data-ttu-id="2b14f-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="2b14f-180">remotePassportEnabled</span></span>|<span data-ttu-id="2b14f-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b14f-181">Boolean</span></span>|<span data-ttu-id="2b14f-182">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2b14f-182">Not yet documented</span></span>|
|<span data-ttu-id="2b14f-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="2b14f-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="2b14f-184">Int32</span><span class="sxs-lookup"><span data-stu-id="2b14f-184">Int32</span></span>|<span data-ttu-id="2b14f-185">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2b14f-185">Not yet documented</span></span>|
|<span data-ttu-id="2b14f-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="2b14f-186">pinExpirationInDays</span></span>|<span data-ttu-id="2b14f-187">Int32</span><span class="sxs-lookup"><span data-stu-id="2b14f-187">Int32</span></span>|<span data-ttu-id="2b14f-188">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2b14f-188">Not yet documented</span></span>|
|<span data-ttu-id="2b14f-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="2b14f-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="2b14f-190">Включение</span><span class="sxs-lookup"><span data-stu-id="2b14f-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="2b14f-191">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="2b14f-191">Not yet documented.</span></span> <span data-ttu-id="2b14f-192">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="2b14f-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="2b14f-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b14f-193">Response</span></span>
<span data-ttu-id="2b14f-194">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2b14f-194">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b14f-195">Пример</span><span class="sxs-lookup"><span data-stu-id="2b14f-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="2b14f-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b14f-196">Request</span></span>
<span data-ttu-id="2b14f-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b14f-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2b14f-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b14f-198">Response</span></span>
<span data-ttu-id="2b14f-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2b14f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



