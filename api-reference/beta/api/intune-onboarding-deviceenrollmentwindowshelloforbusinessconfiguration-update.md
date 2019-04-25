---
title: Обновление deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Обновление свойств объекта deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 44a938e652ba71c6d18846a6a4e85a87b7653ca8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32528836"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="ba726-103">Обновление deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba726-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="ba726-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba726-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba726-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba726-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba726-106">Обновление свойств объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba726-106">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba726-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ba726-107">Prerequisites</span></span>
<span data-ttu-id="ba726-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba726-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba726-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba726-110">Permission type</span></span>|<span data-ttu-id="ba726-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba726-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba726-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba726-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba726-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba726-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ba726-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba726-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba726-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba726-115">Not supported.</span></span>|
|<span data-ttu-id="ba726-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba726-116">Application</span></span>|<span data-ttu-id="ba726-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba726-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba726-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba726-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ba726-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba726-119">Request headers</span></span>
|<span data-ttu-id="ba726-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba726-120">Header</span></span>|<span data-ttu-id="ba726-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ba726-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba726-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba726-122">Authorization</span></span>|<span data-ttu-id="ba726-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba726-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba726-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ba726-124">Accept</span></span>|<span data-ttu-id="ba726-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba726-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba726-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba726-126">Request body</span></span>
<span data-ttu-id="ba726-127">В теле запроса добавьте представление объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba726-127">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="ba726-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba726-128">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="ba726-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba726-129">Property</span></span>|<span data-ttu-id="ba726-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ba726-130">Type</span></span>|<span data-ttu-id="ba726-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ba726-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba726-132">id</span><span class="sxs-lookup"><span data-stu-id="ba726-132">id</span></span>|<span data-ttu-id="ba726-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ba726-133">String</span></span>|<span data-ttu-id="ba726-134">Идентификатор конфигурации страницы состояния регистрации, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba726-134">Id of the Enrollment Status Page configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ba726-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ba726-135">displayName</span></span>|<span data-ttu-id="ba726-136">String</span><span class="sxs-lookup"><span data-stu-id="ba726-136">String</span></span>|<span data-ttu-id="ba726-137">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba726-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ba726-138">description</span><span class="sxs-lookup"><span data-stu-id="ba726-138">description</span></span>|<span data-ttu-id="ba726-139">String</span><span class="sxs-lookup"><span data-stu-id="ba726-139">String</span></span>|<span data-ttu-id="ba726-140">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba726-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ba726-141">priority</span><span class="sxs-lookup"><span data-stu-id="ba726-141">priority</span></span>|<span data-ttu-id="ba726-142">Int32</span><span class="sxs-lookup"><span data-stu-id="ba726-142">Int32</span></span>|<span data-ttu-id="ba726-143">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba726-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ba726-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ba726-144">createdDateTime</span></span>|<span data-ttu-id="ba726-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba726-145">DateTimeOffset</span></span>|<span data-ttu-id="ba726-146">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba726-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ba726-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba726-147">lastModifiedDateTime</span></span>|<span data-ttu-id="ba726-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba726-148">DateTimeOffset</span></span>|<span data-ttu-id="ba726-149">Еще не задокументировано. Наследуется от объекта [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba726-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ba726-150">version</span><span class="sxs-lookup"><span data-stu-id="ba726-150">version</span></span>|<span data-ttu-id="ba726-151">Int32</span><span class="sxs-lookup"><span data-stu-id="ba726-151">Int32</span></span>|<span data-ttu-id="ba726-152">Еще не задокументировано. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba726-152">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="ba726-153">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ba726-153">pinMinimumLength</span></span>|<span data-ttu-id="ba726-154">Int32</span><span class="sxs-lookup"><span data-stu-id="ba726-154">Int32</span></span>|<span data-ttu-id="ba726-155">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ba726-155">Not yet documented</span></span>|
|<span data-ttu-id="ba726-156">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="ba726-156">pinMaximumLength</span></span>|<span data-ttu-id="ba726-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ba726-157">Int32</span></span>|<span data-ttu-id="ba726-158">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ba726-158">Not yet documented</span></span>|
|<span data-ttu-id="ba726-159">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="ba726-159">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="ba726-160">Виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="ba726-160">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="ba726-161">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ba726-161">Not yet documented.</span></span> <span data-ttu-id="ba726-162">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="ba726-162">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="ba726-163">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="ba726-163">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="ba726-164">Виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="ba726-164">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="ba726-165">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ba726-165">Not yet documented.</span></span> <span data-ttu-id="ba726-166">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="ba726-166">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="ba726-167">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="ba726-167">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="ba726-168">Виндовшеллофорбусинесспинусаже</span><span class="sxs-lookup"><span data-stu-id="ba726-168">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="ba726-169">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ba726-169">Not yet documented.</span></span> <span data-ttu-id="ba726-170">Возможные значения: `allowed`, `required`, `disallowed`.</span><span class="sxs-lookup"><span data-stu-id="ba726-170">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="ba726-171">state</span><span class="sxs-lookup"><span data-stu-id="ba726-171">state</span></span>|[<span data-ttu-id="ba726-172">Включение</span><span class="sxs-lookup"><span data-stu-id="ba726-172">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ba726-173">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ba726-173">Not yet documented.</span></span> <span data-ttu-id="ba726-174">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ba726-174">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ba726-175">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="ba726-175">securityDeviceRequired</span></span>|<span data-ttu-id="ba726-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba726-176">Boolean</span></span>|<span data-ttu-id="ba726-177">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ba726-177">Not yet documented</span></span>|
|<span data-ttu-id="ba726-178">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="ba726-178">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="ba726-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba726-179">Boolean</span></span>|<span data-ttu-id="ba726-180">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ba726-180">Not yet documented</span></span>|
|<span data-ttu-id="ba726-181">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="ba726-181">remotePassportEnabled</span></span>|<span data-ttu-id="ba726-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba726-182">Boolean</span></span>|<span data-ttu-id="ba726-183">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ba726-183">Not yet documented</span></span>|
|<span data-ttu-id="ba726-184">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="ba726-184">pinPreviousBlockCount</span></span>|<span data-ttu-id="ba726-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ba726-185">Int32</span></span>|<span data-ttu-id="ba726-186">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ba726-186">Not yet documented</span></span>|
|<span data-ttu-id="ba726-187">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="ba726-187">pinExpirationInDays</span></span>|<span data-ttu-id="ba726-188">Int32</span><span class="sxs-lookup"><span data-stu-id="ba726-188">Int32</span></span>|<span data-ttu-id="ba726-189">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ba726-189">Not yet documented</span></span>|
|<span data-ttu-id="ba726-190">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="ba726-190">enhancedBiometricsState</span></span>|[<span data-ttu-id="ba726-191">Включение</span><span class="sxs-lookup"><span data-stu-id="ba726-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ba726-192">Еще не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="ba726-192">Not yet documented.</span></span> <span data-ttu-id="ba726-193">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ba726-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="ba726-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba726-194">Response</span></span>
<span data-ttu-id="ba726-195">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ba726-195">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba726-196">Пример</span><span class="sxs-lookup"><span data-stu-id="ba726-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba726-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba726-197">Request</span></span>
<span data-ttu-id="ba726-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba726-198">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
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

### <a name="response"></a><span data-ttu-id="ba726-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba726-199">Response</span></span>
<span data-ttu-id="ba726-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba726-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





