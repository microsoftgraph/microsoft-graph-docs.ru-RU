---
title: Создание deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Создание объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7ac406b338d70761c8b14c9100d2eca4cedcb7fd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416148"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="505a0-103">Создание deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="505a0-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="505a0-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="505a0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="505a0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="505a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="505a0-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="505a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="505a0-107">Создание объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="505a0-107">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="505a0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="505a0-108">Prerequisites</span></span>
<span data-ttu-id="505a0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="505a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="505a0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="505a0-111">Permission type</span></span>|<span data-ttu-id="505a0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="505a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="505a0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="505a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="505a0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="505a0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="505a0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="505a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="505a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="505a0-116">Not supported.</span></span>|
|<span data-ttu-id="505a0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="505a0-117">Application</span></span>|<span data-ttu-id="505a0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="505a0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="505a0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="505a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="505a0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="505a0-120">Request headers</span></span>
|<span data-ttu-id="505a0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="505a0-121">Header</span></span>|<span data-ttu-id="505a0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="505a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="505a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="505a0-123">Authorization</span></span>|<span data-ttu-id="505a0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="505a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="505a0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="505a0-125">Accept</span></span>|<span data-ttu-id="505a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="505a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="505a0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="505a0-127">Request body</span></span>
<span data-ttu-id="505a0-128">В теле запроса добавьте представление объекта deviceEnrollmentWindowsHelloForBusinessConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="505a0-128">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="505a0-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="505a0-129">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="505a0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="505a0-130">Property</span></span>|<span data-ttu-id="505a0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="505a0-131">Type</span></span>|<span data-ttu-id="505a0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="505a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="505a0-133">id</span><span class="sxs-lookup"><span data-stu-id="505a0-133">id</span></span>|<span data-ttu-id="505a0-134">String</span><span class="sxs-lookup"><span data-stu-id="505a0-134">String</span></span>|<span data-ttu-id="505a0-135">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="505a0-135">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="505a0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="505a0-136">displayName</span></span>|<span data-ttu-id="505a0-137">String</span><span class="sxs-lookup"><span data-stu-id="505a0-137">String</span></span>|<span data-ttu-id="505a0-138">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="505a0-138">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="505a0-139">description</span><span class="sxs-lookup"><span data-stu-id="505a0-139">description</span></span>|<span data-ttu-id="505a0-140">String</span><span class="sxs-lookup"><span data-stu-id="505a0-140">String</span></span>|<span data-ttu-id="505a0-141">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="505a0-141">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="505a0-142">priority</span><span class="sxs-lookup"><span data-stu-id="505a0-142">priority</span></span>|<span data-ttu-id="505a0-143">Int32</span><span class="sxs-lookup"><span data-stu-id="505a0-143">Int32</span></span>|<span data-ttu-id="505a0-144">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="505a0-144">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="505a0-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="505a0-145">createdDateTime</span></span>|<span data-ttu-id="505a0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="505a0-146">DateTimeOffset</span></span>|<span data-ttu-id="505a0-147">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="505a0-147">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="505a0-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="505a0-148">lastModifiedDateTime</span></span>|<span data-ttu-id="505a0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="505a0-149">DateTimeOffset</span></span>|<span data-ttu-id="505a0-150">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="505a0-150">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="505a0-151">version</span><span class="sxs-lookup"><span data-stu-id="505a0-151">version</span></span>|<span data-ttu-id="505a0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="505a0-152">Int32</span></span>|<span data-ttu-id="505a0-153">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="505a0-153">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="505a0-154">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="505a0-154">pinMinimumLength</span></span>|<span data-ttu-id="505a0-155">Int32</span><span class="sxs-lookup"><span data-stu-id="505a0-155">Int32</span></span>|<span data-ttu-id="505a0-156">Н/Д</span><span class="sxs-lookup"><span data-stu-id="505a0-156">Not yet documented</span></span>|
|<span data-ttu-id="505a0-157">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="505a0-157">pinMaximumLength</span></span>|<span data-ttu-id="505a0-158">Int32</span><span class="sxs-lookup"><span data-stu-id="505a0-158">Int32</span></span>|<span data-ttu-id="505a0-159">Н/Д</span><span class="sxs-lookup"><span data-stu-id="505a0-159">Not yet documented</span></span>|
|<span data-ttu-id="505a0-160">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="505a0-160">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="505a0-161">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="505a0-161">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="505a0-162">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="505a0-162">Not yet documented.</span></span> <span data-ttu-id="505a0-163">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="505a0-163">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="505a0-164">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="505a0-164">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="505a0-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="505a0-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="505a0-166">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="505a0-166">Not yet documented.</span></span> <span data-ttu-id="505a0-167">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="505a0-167">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="505a0-168">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="505a0-168">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="505a0-169">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="505a0-169">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="505a0-170">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="505a0-170">Not yet documented.</span></span> <span data-ttu-id="505a0-171">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="505a0-171">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="505a0-172">state</span><span class="sxs-lookup"><span data-stu-id="505a0-172">state</span></span>|[<span data-ttu-id="505a0-173">Включение</span><span class="sxs-lookup"><span data-stu-id="505a0-173">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="505a0-174">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="505a0-174">Not yet documented.</span></span> <span data-ttu-id="505a0-175">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="505a0-175">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="505a0-176">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="505a0-176">securityDeviceRequired</span></span>|<span data-ttu-id="505a0-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="505a0-177">Boolean</span></span>|<span data-ttu-id="505a0-178">Н/Д</span><span class="sxs-lookup"><span data-stu-id="505a0-178">Not yet documented</span></span>|
|<span data-ttu-id="505a0-179">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="505a0-179">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="505a0-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="505a0-180">Boolean</span></span>|<span data-ttu-id="505a0-181">Н/Д</span><span class="sxs-lookup"><span data-stu-id="505a0-181">Not yet documented</span></span>|
|<span data-ttu-id="505a0-182">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="505a0-182">remotePassportEnabled</span></span>|<span data-ttu-id="505a0-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="505a0-183">Boolean</span></span>|<span data-ttu-id="505a0-184">Н/Д</span><span class="sxs-lookup"><span data-stu-id="505a0-184">Not yet documented</span></span>|
|<span data-ttu-id="505a0-185">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="505a0-185">pinPreviousBlockCount</span></span>|<span data-ttu-id="505a0-186">Int32</span><span class="sxs-lookup"><span data-stu-id="505a0-186">Int32</span></span>|<span data-ttu-id="505a0-187">Н/Д</span><span class="sxs-lookup"><span data-stu-id="505a0-187">Not yet documented</span></span>|
|<span data-ttu-id="505a0-188">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="505a0-188">pinExpirationInDays</span></span>|<span data-ttu-id="505a0-189">Int32</span><span class="sxs-lookup"><span data-stu-id="505a0-189">Int32</span></span>|<span data-ttu-id="505a0-190">Н/Д</span><span class="sxs-lookup"><span data-stu-id="505a0-190">Not yet documented</span></span>|
|<span data-ttu-id="505a0-191">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="505a0-191">enhancedBiometricsState</span></span>|[<span data-ttu-id="505a0-192">Включение</span><span class="sxs-lookup"><span data-stu-id="505a0-192">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="505a0-193">Еще не документированы.</span><span class="sxs-lookup"><span data-stu-id="505a0-193">Not yet documented.</span></span> <span data-ttu-id="505a0-194">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="505a0-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="505a0-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="505a0-195">Response</span></span>
<span data-ttu-id="505a0-196">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="505a0-196">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="505a0-197">Пример</span><span class="sxs-lookup"><span data-stu-id="505a0-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="505a0-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="505a0-198">Request</span></span>
<span data-ttu-id="505a0-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="505a0-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
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

### <a name="response"></a><span data-ttu-id="505a0-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="505a0-200">Response</span></span>
<span data-ttu-id="505a0-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="505a0-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




