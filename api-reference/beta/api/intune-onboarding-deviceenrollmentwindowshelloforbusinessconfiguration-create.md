---
title: Создание deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Создание объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4db61460a7855e11f6c8fb51aa2656f25c10547e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151347"
---
# <a name="create-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="1ff98-103">Создание deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ff98-103">Create deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="1ff98-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ff98-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ff98-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ff98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ff98-106">Создание объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ff98-106">Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ff98-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1ff98-107">Prerequisites</span></span>
<span data-ttu-id="1ff98-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1ff98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1ff98-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ff98-110">Permission type</span></span>|<span data-ttu-id="1ff98-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ff98-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ff98-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ff98-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1ff98-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ff98-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1ff98-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ff98-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ff98-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ff98-115">Not supported.</span></span>|
|<span data-ttu-id="1ff98-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ff98-116">Application</span></span>|<span data-ttu-id="1ff98-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ff98-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ff98-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ff98-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1ff98-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ff98-119">Request headers</span></span>
|<span data-ttu-id="1ff98-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ff98-120">Header</span></span>|<span data-ttu-id="1ff98-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1ff98-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ff98-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1ff98-122">Authorization</span></span>|<span data-ttu-id="1ff98-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1ff98-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ff98-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1ff98-124">Accept</span></span>|<span data-ttu-id="1ff98-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1ff98-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ff98-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1ff98-126">Request body</span></span>
<span data-ttu-id="1ff98-127">В теле запроса добавьте представление объекта deviceEnrollmentWindowsHelloForBusinessConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ff98-127">In the request body, supply a JSON representation for the deviceEnrollmentWindowsHelloForBusinessConfiguration object.</span></span>

<span data-ttu-id="1ff98-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1ff98-128">The following table shows the properties that are required when you create the deviceEnrollmentWindowsHelloForBusinessConfiguration.</span></span>

|<span data-ttu-id="1ff98-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ff98-129">Property</span></span>|<span data-ttu-id="1ff98-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1ff98-130">Type</span></span>|<span data-ttu-id="1ff98-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1ff98-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ff98-132">id</span><span class="sxs-lookup"><span data-stu-id="1ff98-132">id</span></span>|<span data-ttu-id="1ff98-133">String</span><span class="sxs-lookup"><span data-stu-id="1ff98-133">String</span></span>|<span data-ttu-id="1ff98-134">Идентификатор конфигурации страницы состояния регистрации, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ff98-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1ff98-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1ff98-135">displayName</span></span>|<span data-ttu-id="1ff98-136">String</span><span class="sxs-lookup"><span data-stu-id="1ff98-136">String</span></span>|<span data-ttu-id="1ff98-137">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ff98-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1ff98-138">description</span><span class="sxs-lookup"><span data-stu-id="1ff98-138">description</span></span>|<span data-ttu-id="1ff98-139">String</span><span class="sxs-lookup"><span data-stu-id="1ff98-139">String</span></span>|<span data-ttu-id="1ff98-140">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ff98-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1ff98-141">priority</span><span class="sxs-lookup"><span data-stu-id="1ff98-141">priority</span></span>|<span data-ttu-id="1ff98-142">Int32</span><span class="sxs-lookup"><span data-stu-id="1ff98-142">Int32</span></span>|<span data-ttu-id="1ff98-143">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ff98-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1ff98-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ff98-144">createdDateTime</span></span>|<span data-ttu-id="1ff98-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ff98-145">DateTimeOffset</span></span>|<span data-ttu-id="1ff98-146">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ff98-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1ff98-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ff98-147">lastModifiedDateTime</span></span>|<span data-ttu-id="1ff98-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ff98-148">DateTimeOffset</span></span>|<span data-ttu-id="1ff98-149">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ff98-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1ff98-150">version</span><span class="sxs-lookup"><span data-stu-id="1ff98-150">version</span></span>|<span data-ttu-id="1ff98-151">Int32</span><span class="sxs-lookup"><span data-stu-id="1ff98-151">Int32</span></span>|<span data-ttu-id="1ff98-152">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ff98-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="1ff98-153">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1ff98-153">pinMinimumLength</span></span>|<span data-ttu-id="1ff98-154">Int32</span><span class="sxs-lookup"><span data-stu-id="1ff98-154">Int32</span></span>|<span data-ttu-id="1ff98-155">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1ff98-155">Not yet documented</span></span>|
|<span data-ttu-id="1ff98-156">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="1ff98-156">pinMaximumLength</span></span>|<span data-ttu-id="1ff98-157">Int32</span><span class="sxs-lookup"><span data-stu-id="1ff98-157">Int32</span></span>|<span data-ttu-id="1ff98-158">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1ff98-158">Not yet documented</span></span>|
|<span data-ttu-id="1ff98-159">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1ff98-159">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="1ff98-160">Виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="1ff98-160">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="1ff98-161">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="1ff98-161">Not yet documented.</span></span> <span data-ttu-id="1ff98-162">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="1ff98-162">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="1ff98-163">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1ff98-163">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="1ff98-164">Виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="1ff98-164">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="1ff98-165">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="1ff98-165">Not yet documented.</span></span> <span data-ttu-id="1ff98-166">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="1ff98-166">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="1ff98-167">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="1ff98-167">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="1ff98-168">Виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="1ff98-168">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="1ff98-169">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="1ff98-169">Not yet documented.</span></span> <span data-ttu-id="1ff98-170">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="1ff98-170">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="1ff98-171">state</span><span class="sxs-lookup"><span data-stu-id="1ff98-171">state</span></span>|[<span data-ttu-id="1ff98-172">Включение</span><span class="sxs-lookup"><span data-stu-id="1ff98-172">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="1ff98-173">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="1ff98-173">Not yet documented.</span></span> <span data-ttu-id="1ff98-174">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1ff98-174">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="1ff98-175">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="1ff98-175">securityDeviceRequired</span></span>|<span data-ttu-id="1ff98-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ff98-176">Boolean</span></span>|<span data-ttu-id="1ff98-177">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="1ff98-177">Not yet documented</span></span>|
|<span data-ttu-id="1ff98-178">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="1ff98-178">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="1ff98-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ff98-179">Boolean</span></span>|<span data-ttu-id="1ff98-180">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="1ff98-180">Not yet documented</span></span>|
|<span data-ttu-id="1ff98-181">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="1ff98-181">remotePassportEnabled</span></span>|<span data-ttu-id="1ff98-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ff98-182">Boolean</span></span>|<span data-ttu-id="1ff98-183">Пока не задокументировано</span><span class="sxs-lookup"><span data-stu-id="1ff98-183">Not yet documented</span></span>|
|<span data-ttu-id="1ff98-184">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="1ff98-184">pinPreviousBlockCount</span></span>|<span data-ttu-id="1ff98-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1ff98-185">Int32</span></span>|<span data-ttu-id="1ff98-186">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1ff98-186">Not yet documented</span></span>|
|<span data-ttu-id="1ff98-187">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="1ff98-187">pinExpirationInDays</span></span>|<span data-ttu-id="1ff98-188">Int32</span><span class="sxs-lookup"><span data-stu-id="1ff98-188">Int32</span></span>|<span data-ttu-id="1ff98-189">Н/Д</span><span class="sxs-lookup"><span data-stu-id="1ff98-189">Not yet documented</span></span>|
|<span data-ttu-id="1ff98-190">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="1ff98-190">enhancedBiometricsState</span></span>|[<span data-ttu-id="1ff98-191">Включение</span><span class="sxs-lookup"><span data-stu-id="1ff98-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="1ff98-192">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="1ff98-192">Not yet documented.</span></span> <span data-ttu-id="1ff98-193">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1ff98-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="1ff98-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ff98-194">Response</span></span>
<span data-ttu-id="1ff98-195">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1ff98-195">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ff98-196">Пример</span><span class="sxs-lookup"><span data-stu-id="1ff98-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ff98-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ff98-197">Request</span></span>
<span data-ttu-id="1ff98-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ff98-198">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1ff98-199">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ff98-199">Response</span></span>
<span data-ttu-id="1ff98-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ff98-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




