---
title: Обновление Азуреадвиндовсаутопилотдеплойментпрофиле
description: Обновление свойств объекта Азуреадвиндовсаутопилотдеплойментпрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 510d8360fb5192d5d3952c2fc56496760d6621d5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32533921"
---
# <a name="update-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="347d0-103">Обновление Азуреадвиндовсаутопилотдеплойментпрофиле</span><span class="sxs-lookup"><span data-stu-id="347d0-103">Update azureADWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="347d0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="347d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="347d0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="347d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="347d0-106">Обновление свойств объекта [азуреадвиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="347d0-106">Update the properties of a [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="347d0-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="347d0-107">Prerequisites</span></span>
<span data-ttu-id="347d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="347d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="347d0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="347d0-110">Permission type</span></span>|<span data-ttu-id="347d0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="347d0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="347d0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="347d0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="347d0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="347d0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="347d0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="347d0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="347d0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="347d0-115">Not supported.</span></span>|
|<span data-ttu-id="347d0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="347d0-116">Application</span></span>|<span data-ttu-id="347d0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="347d0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="347d0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="347d0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="347d0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="347d0-119">Request headers</span></span>
|<span data-ttu-id="347d0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="347d0-120">Header</span></span>|<span data-ttu-id="347d0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="347d0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="347d0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="347d0-122">Authorization</span></span>|<span data-ttu-id="347d0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="347d0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="347d0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="347d0-124">Accept</span></span>|<span data-ttu-id="347d0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="347d0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="347d0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="347d0-126">Request body</span></span>
<span data-ttu-id="347d0-127">В тексте запроса добавьте представление объекта [Азуреадвиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="347d0-127">In the request body, supply a JSON representation for the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="347d0-128">В следующей таблице приведены свойства, необходимые при создании [азуреадвиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="347d0-128">The following table shows the properties that are required when you create the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="347d0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="347d0-129">Property</span></span>|<span data-ttu-id="347d0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="347d0-130">Type</span></span>|<span data-ttu-id="347d0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="347d0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="347d0-132">id</span><span class="sxs-lookup"><span data-stu-id="347d0-132">id</span></span>|<span data-ttu-id="347d0-133">Строка</span><span class="sxs-lookup"><span data-stu-id="347d0-133">String</span></span>|<span data-ttu-id="347d0-134">Ключ профиля, наСледуемый от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="347d0-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="347d0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="347d0-135">displayName</span></span>|<span data-ttu-id="347d0-136">Строка</span><span class="sxs-lookup"><span data-stu-id="347d0-136">String</span></span>|<span data-ttu-id="347d0-137">Имя профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="347d0-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="347d0-138">description</span><span class="sxs-lookup"><span data-stu-id="347d0-138">description</span></span>|<span data-ttu-id="347d0-139">String</span><span class="sxs-lookup"><span data-stu-id="347d0-139">String</span></span>|<span data-ttu-id="347d0-140">Описание профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="347d0-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="347d0-141">language</span><span class="sxs-lookup"><span data-stu-id="347d0-141">language</span></span>|<span data-ttu-id="347d0-142">String</span><span class="sxs-lookup"><span data-stu-id="347d0-142">String</span></span>|<span data-ttu-id="347d0-143">Язык, настроенный на устройстве, унаследованном от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="347d0-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="347d0-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="347d0-144">createdDateTime</span></span>|<span data-ttu-id="347d0-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="347d0-145">DateTimeOffset</span></span>|<span data-ttu-id="347d0-146">Время создания профиля, унаследованное от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="347d0-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="347d0-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="347d0-147">lastModifiedDateTime</span></span>|<span data-ttu-id="347d0-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="347d0-148">DateTimeOffset</span></span>|<span data-ttu-id="347d0-149">Время последнего изменения профиля, наСледуемого от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="347d0-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="347d0-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="347d0-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="347d0-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="347d0-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="347d0-152">Настройка "от" в рамке наСледуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="347d0-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="347d0-153">Енроллментстатусскринсеттингс</span><span class="sxs-lookup"><span data-stu-id="347d0-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="347d0-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="347d0-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="347d0-155">Параметр экрана состояния регистрации, наСледуемый от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="347d0-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="347d0-156">Екстраксардварехаш</span><span class="sxs-lookup"><span data-stu-id="347d0-156">extractHardwareHash</span></span>|<span data-ttu-id="347d0-157">Логический</span><span class="sxs-lookup"><span data-stu-id="347d0-157">Boolean</span></span>|<span data-ttu-id="347d0-158">Извлечение Хардварехаш для профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="347d0-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="347d0-159">Девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="347d0-159">deviceNameTemplate</span></span>|<span data-ttu-id="347d0-160">String</span><span class="sxs-lookup"><span data-stu-id="347d0-160">String</span></span>|<span data-ttu-id="347d0-161">Шаблон, используемый для именования автоПилотного устройства.</span><span class="sxs-lookup"><span data-stu-id="347d0-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="347d0-162">Это может быть настраиваемый текст, который также может содержать серийный номер устройства или случайное число.</span><span class="sxs-lookup"><span data-stu-id="347d0-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="347d0-163">Общая длина текста, созданного шаблоном, не может превышать 15 символов.</span><span class="sxs-lookup"><span data-stu-id="347d0-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="347d0-164">НаСледуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="347d0-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="347d0-165">deviceType</span><span class="sxs-lookup"><span data-stu-id="347d0-165">deviceType</span></span>|[<span data-ttu-id="347d0-166">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="347d0-166">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="347d0-167">Тип устройства автоПилота, к которому применяется этот профиль.</span><span class="sxs-lookup"><span data-stu-id="347d0-167">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="347d0-168">НаСледуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="347d0-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="347d0-169">Возможные значения: `windowsPc`, `surfaceHub2`.</span><span class="sxs-lookup"><span data-stu-id="347d0-169">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="347d0-170">Енаблевхитеглове</span><span class="sxs-lookup"><span data-stu-id="347d0-170">enableWhiteGlove</span></span>|<span data-ttu-id="347d0-171">Логический</span><span class="sxs-lookup"><span data-stu-id="347d0-171">Boolean</span></span>|<span data-ttu-id="347d0-172">Включите для профиля белый Глове для автопилотного развертывания.</span><span class="sxs-lookup"><span data-stu-id="347d0-172">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="347d0-173">НаСледуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="347d0-173">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="347d0-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="347d0-174">Response</span></span>
<span data-ttu-id="347d0-175">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [азуреадвиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="347d0-175">If successful, this method returns a `200 OK` response code and an updated [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="347d0-176">Пример</span><span class="sxs-lookup"><span data-stu-id="347d0-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="347d0-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="347d0-177">Request</span></span>
<span data-ttu-id="347d0-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="347d0-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1097

{
  "@odata.type": "#microsoft.graph.azureADWindowsAutopilotDeploymentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "language": "Language value",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "standard",
    "deviceUsageType": "shared",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "Custom Error Message value",
    "installProgressTimeoutInMinutes": 15,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "Device Name Template value",
  "deviceType": "surfaceHub2",
  "enableWhiteGlove": true
}
```

### <a name="response"></a><span data-ttu-id="347d0-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="347d0-179">Response</span></span>
<span data-ttu-id="347d0-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="347d0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1269

{
  "@odata.type": "#microsoft.graph.azureADWindowsAutopilotDeploymentProfile",
  "id": "e2ec4e69-4e69-e2ec-694e-ece2694eece2",
  "displayName": "Display Name value",
  "description": "Description value",
  "language": "Language value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "standard",
    "deviceUsageType": "shared",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "Custom Error Message value",
    "installProgressTimeoutInMinutes": 15,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "Device Name Template value",
  "deviceType": "surfaceHub2",
  "enableWhiteGlove": true
}
```





