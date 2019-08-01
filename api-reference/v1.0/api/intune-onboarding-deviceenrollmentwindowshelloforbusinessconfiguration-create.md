---
title: Создание deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Создание объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 291b9817ab7f1d0487088fbd9aef56fdc01a7f9e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017919"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="9539c-103">Создание deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="9539c-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="9539c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9539c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9539c-105">Создание объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9539c-105">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9539c-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9539c-106">Prerequisites</span></span>
<span data-ttu-id="9539c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9539c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9539c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9539c-109">Permission type</span></span>|<span data-ttu-id="9539c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9539c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9539c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9539c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9539c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9539c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9539c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9539c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9539c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9539c-114">Not supported.</span></span>|
|<span data-ttu-id="9539c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9539c-115">Application</span></span>|<span data-ttu-id="9539c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9539c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9539c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9539c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9539c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9539c-118">Request headers</span></span>
|<span data-ttu-id="9539c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9539c-119">Header</span></span>|<span data-ttu-id="9539c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9539c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9539c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9539c-121">Authorization</span></span>|<span data-ttu-id="9539c-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9539c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9539c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9539c-123">Accept</span></span>|<span data-ttu-id="9539c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9539c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9539c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9539c-125">Request body</span></span>
<span data-ttu-id="9539c-126">В теле запроса добавьте представление объекта deviceEnrollmentWindowsHelloForBusinessConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9539c-126">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="9539c-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9539c-127">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="9539c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9539c-128">Property</span></span>|<span data-ttu-id="9539c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9539c-129">Type</span></span>|<span data-ttu-id="9539c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9539c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9539c-131">id</span><span class="sxs-lookup"><span data-stu-id="9539c-131">id</span></span>|<span data-ttu-id="9539c-132">String</span><span class="sxs-lookup"><span data-stu-id="9539c-132">String</span></span>|<span data-ttu-id="9539c-133">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9539c-133">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9539c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="9539c-134">displayName</span></span>|<span data-ttu-id="9539c-135">Строка</span><span class="sxs-lookup"><span data-stu-id="9539c-135">String</span></span>|<span data-ttu-id="9539c-136">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9539c-136">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9539c-137">description</span><span class="sxs-lookup"><span data-stu-id="9539c-137">description</span></span>|<span data-ttu-id="9539c-138">String</span><span class="sxs-lookup"><span data-stu-id="9539c-138">String</span></span>|<span data-ttu-id="9539c-139">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9539c-139">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9539c-140">priority</span><span class="sxs-lookup"><span data-stu-id="9539c-140">priority</span></span>|<span data-ttu-id="9539c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="9539c-141">Int32</span></span>|<span data-ttu-id="9539c-142">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9539c-142">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9539c-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9539c-143">createdDateTime</span></span>|<span data-ttu-id="9539c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9539c-144">DateTimeOffset</span></span>|<span data-ttu-id="9539c-145">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9539c-145">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9539c-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9539c-146">lastModifiedDateTime</span></span>|<span data-ttu-id="9539c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9539c-147">DateTimeOffset</span></span>|<span data-ttu-id="9539c-148">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9539c-148">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9539c-149">version</span><span class="sxs-lookup"><span data-stu-id="9539c-149">version</span></span>|<span data-ttu-id="9539c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="9539c-150">Int32</span></span>|<span data-ttu-id="9539c-151">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9539c-151">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="9539c-152">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9539c-152">pinMinimumLength</span></span>|<span data-ttu-id="9539c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="9539c-153">Int32</span></span>|<span data-ttu-id="9539c-154">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9539c-154">Not yet documented</span></span>|
|<span data-ttu-id="9539c-155">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="9539c-155">pinMaximumLength</span></span>|<span data-ttu-id="9539c-156">Int32</span><span class="sxs-lookup"><span data-stu-id="9539c-156">Int32</span></span>|<span data-ttu-id="9539c-157">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9539c-157">Not yet documented</span></span>|
|<span data-ttu-id="9539c-158">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="9539c-158">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="9539c-159">Виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="9539c-159">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="9539c-160">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9539c-160">Not yet documented.</span></span> <span data-ttu-id="9539c-161">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="9539c-161">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="9539c-162">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="9539c-162">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="9539c-163">Виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="9539c-163">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="9539c-164">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9539c-164">Not yet documented.</span></span> <span data-ttu-id="9539c-165">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="9539c-165">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="9539c-166">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="9539c-166">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="9539c-167">Виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="9539c-167">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="9539c-168">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9539c-168">Not yet documented.</span></span> <span data-ttu-id="9539c-169">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="9539c-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="9539c-170">состояние</span><span class="sxs-lookup"><span data-stu-id="9539c-170">state</span></span>|[<span data-ttu-id="9539c-171">Включение</span><span class="sxs-lookup"><span data-stu-id="9539c-171">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="9539c-172">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9539c-172">Not yet documented.</span></span> <span data-ttu-id="9539c-173">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9539c-173">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9539c-174">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="9539c-174">securityDeviceRequired</span></span>|<span data-ttu-id="9539c-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="9539c-175">Boolean</span></span>|<span data-ttu-id="9539c-176">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9539c-176">Not yet documented</span></span>|
|<span data-ttu-id="9539c-177">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="9539c-177">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="9539c-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="9539c-178">Boolean</span></span>|<span data-ttu-id="9539c-179">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9539c-179">Not yet documented</span></span>|
|<span data-ttu-id="9539c-180">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="9539c-180">remotePassportEnabled</span></span>|<span data-ttu-id="9539c-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="9539c-181">Boolean</span></span>|<span data-ttu-id="9539c-182">Н/Д</span><span class="sxs-lookup"><span data-stu-id="9539c-182">Not yet documented</span></span>|
|<span data-ttu-id="9539c-183">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="9539c-183">pinPreviousBlockCount</span></span>|<span data-ttu-id="9539c-184">Int32</span><span class="sxs-lookup"><span data-stu-id="9539c-184">Int32</span></span>|<span data-ttu-id="9539c-185">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9539c-185">Not yet documented</span></span>|
|<span data-ttu-id="9539c-186">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="9539c-186">pinExpirationInDays</span></span>|<span data-ttu-id="9539c-187">Int32</span><span class="sxs-lookup"><span data-stu-id="9539c-187">Int32</span></span>|<span data-ttu-id="9539c-188">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9539c-188">Not yet documented</span></span>|
|<span data-ttu-id="9539c-189">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="9539c-189">enhancedBiometricsState</span></span>|[<span data-ttu-id="9539c-190">Включение</span><span class="sxs-lookup"><span data-stu-id="9539c-190">enablement</span></span>](../resources/intune-onboarding-enablement.md)|<span data-ttu-id="9539c-191">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9539c-191">Not yet documented.</span></span> <span data-ttu-id="9539c-192">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9539c-192">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="9539c-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="9539c-193">Response</span></span>
<span data-ttu-id="9539c-194">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9539c-194">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9539c-195">Пример</span><span class="sxs-lookup"><span data-stu-id="9539c-195">Example</span></span>

### <a name="request"></a><span data-ttu-id="9539c-196">Запрос</span><span class="sxs-lookup"><span data-stu-id="9539c-196">Request</span></span>
<span data-ttu-id="9539c-197">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9539c-197">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9539c-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="9539c-198">Response</span></span>
<span data-ttu-id="9539c-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9539c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



