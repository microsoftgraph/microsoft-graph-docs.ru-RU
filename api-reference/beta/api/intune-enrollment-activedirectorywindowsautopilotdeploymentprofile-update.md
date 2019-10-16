---
title: Обновление Активедиректоривиндовсаутопилотдеплойментпрофиле
description: Обновление свойств объекта Активедиректоривиндовсаутопилотдеплойментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8fedf84af6858b43c11f0e05d99a52ad7d8ea503
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37526262"
---
# <a name="update-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="ed254-103">Обновление Активедиректоривиндовсаутопилотдеплойментпрофиле</span><span class="sxs-lookup"><span data-stu-id="ed254-103">Update activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="ed254-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed254-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed254-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed254-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed254-106">Обновление свойств объекта [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ed254-106">Update the properties of a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed254-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ed254-107">Prerequisites</span></span>
<span data-ttu-id="ed254-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed254-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed254-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed254-110">Permission type</span></span>|<span data-ttu-id="ed254-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed254-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed254-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed254-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ed254-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed254-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ed254-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed254-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed254-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed254-115">Not supported.</span></span>|
|<span data-ttu-id="ed254-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ed254-116">Application</span></span>|<span data-ttu-id="ed254-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed254-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed254-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed254-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="ed254-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed254-119">Request headers</span></span>
|<span data-ttu-id="ed254-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ed254-120">Header</span></span>|<span data-ttu-id="ed254-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ed254-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed254-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ed254-122">Authorization</span></span>|<span data-ttu-id="ed254-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed254-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed254-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ed254-124">Accept</span></span>|<span data-ttu-id="ed254-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ed254-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed254-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ed254-126">Request body</span></span>
<span data-ttu-id="ed254-127">В тексте запроса добавьте представление объекта [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed254-127">In the request body, supply a JSON representation for the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="ed254-128">В следующей таблице приведены свойства, необходимые при создании [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="ed254-128">The following table shows the properties that are required when you create the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="ed254-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed254-129">Property</span></span>|<span data-ttu-id="ed254-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ed254-130">Type</span></span>|<span data-ttu-id="ed254-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ed254-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed254-132">id</span><span class="sxs-lookup"><span data-stu-id="ed254-132">id</span></span>|<span data-ttu-id="ed254-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ed254-133">String</span></span>|<span data-ttu-id="ed254-134">Ключ профиля, наследуемый от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ed254-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ed254-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ed254-135">displayName</span></span>|<span data-ttu-id="ed254-136">Строка</span><span class="sxs-lookup"><span data-stu-id="ed254-136">String</span></span>|<span data-ttu-id="ed254-137">Имя профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ed254-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ed254-138">description</span><span class="sxs-lookup"><span data-stu-id="ed254-138">description</span></span>|<span data-ttu-id="ed254-139">String</span><span class="sxs-lookup"><span data-stu-id="ed254-139">String</span></span>|<span data-ttu-id="ed254-140">Описание профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ed254-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ed254-141">language</span><span class="sxs-lookup"><span data-stu-id="ed254-141">language</span></span>|<span data-ttu-id="ed254-142">String</span><span class="sxs-lookup"><span data-stu-id="ed254-142">String</span></span>|<span data-ttu-id="ed254-143">Язык, настроенный на устройстве, унаследованном от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ed254-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ed254-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed254-144">createdDateTime</span></span>|<span data-ttu-id="ed254-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed254-145">DateTimeOffset</span></span>|<span data-ttu-id="ed254-146">Время создания профиля, унаследованное от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ed254-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ed254-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed254-147">lastModifiedDateTime</span></span>|<span data-ttu-id="ed254-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed254-148">DateTimeOffset</span></span>|<span data-ttu-id="ed254-149">Время последнего изменения профиля, наследуемого от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ed254-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ed254-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="ed254-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="ed254-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="ed254-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="ed254-152">Настройка "от" в рамке наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ed254-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ed254-153">енроллментстатусскринсеттингс</span><span class="sxs-lookup"><span data-stu-id="ed254-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="ed254-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="ed254-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="ed254-155">Параметр экрана состояния регистрации, наследуемый от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ed254-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ed254-156">екстраксардварехаш</span><span class="sxs-lookup"><span data-stu-id="ed254-156">extractHardwareHash</span></span>|<span data-ttu-id="ed254-157">Логический</span><span class="sxs-lookup"><span data-stu-id="ed254-157">Boolean</span></span>|<span data-ttu-id="ed254-158">Извлечение Хардварехаш для профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ed254-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ed254-159">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="ed254-159">deviceNameTemplate</span></span>|<span data-ttu-id="ed254-160">String</span><span class="sxs-lookup"><span data-stu-id="ed254-160">String</span></span>|<span data-ttu-id="ed254-161">Шаблон, используемый для именования автопилотного устройства.</span><span class="sxs-lookup"><span data-stu-id="ed254-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="ed254-162">Это может быть настраиваемый текст, который также может содержать серийный номер устройства или случайное число.</span><span class="sxs-lookup"><span data-stu-id="ed254-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="ed254-163">Общая длина текста, созданного шаблоном, не может превышать 15 символов.</span><span class="sxs-lookup"><span data-stu-id="ed254-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="ed254-164">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ed254-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ed254-165">deviceType</span><span class="sxs-lookup"><span data-stu-id="ed254-165">deviceType</span></span>|[<span data-ttu-id="ed254-166">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="ed254-166">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="ed254-167">Тип устройства автопилота, к которому применяется этот профиль.</span><span class="sxs-lookup"><span data-stu-id="ed254-167">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="ed254-168">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="ed254-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="ed254-169">Возможные значения: `windowsPc`, `surfaceHub2`.</span><span class="sxs-lookup"><span data-stu-id="ed254-169">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="ed254-170">енаблевхитеглове</span><span class="sxs-lookup"><span data-stu-id="ed254-170">enableWhiteGlove</span></span>|<span data-ttu-id="ed254-171">Логический</span><span class="sxs-lookup"><span data-stu-id="ed254-171">Boolean</span></span>|<span data-ttu-id="ed254-172">Включите для профиля белый Глове для автопилотного развертывания.</span><span class="sxs-lookup"><span data-stu-id="ed254-172">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="ed254-173">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ed254-173">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="ed254-174">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ed254-174">roleScopeTagIds</span></span>|<span data-ttu-id="ed254-175">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ed254-175">String collection</span></span>|<span data-ttu-id="ed254-176">Теги областей для профиля.</span><span class="sxs-lookup"><span data-stu-id="ed254-176">Scope tags for the profile.</span></span> <span data-ttu-id="ed254-177">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ed254-177">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ed254-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed254-178">Response</span></span>
<span data-ttu-id="ed254-179">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ed254-179">If successful, this method returns a `200 OK` response code and an updated [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed254-180">Пример</span><span class="sxs-lookup"><span data-stu-id="ed254-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed254-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed254-181">Request</span></span>
<span data-ttu-id="ed254-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed254-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1167

{
  "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
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
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="ed254-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed254-183">Response</span></span>
<span data-ttu-id="ed254-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ed254-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1339

{
  "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
  "id": "49fe234a-234a-49fe-4a23-fe494a23fe49",
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
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```






