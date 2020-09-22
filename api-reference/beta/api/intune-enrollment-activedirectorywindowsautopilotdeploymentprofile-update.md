---
title: Обновление Активедиректоривиндовсаутопилотдеплойментпрофиле
description: Обновление свойств объекта Активедиректоривиндовсаутопилотдеплойментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a754b4e05286762bf4a7d0847a534b556be853bc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040758"
---
# <a name="update-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="93276-103">Обновление Активедиректоривиндовсаутопилотдеплойментпрофиле</span><span class="sxs-lookup"><span data-stu-id="93276-103">Update activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="93276-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93276-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93276-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93276-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93276-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93276-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93276-107">Обновление свойств объекта [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="93276-107">Update the properties of a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93276-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="93276-108">Prerequisites</span></span>
<span data-ttu-id="93276-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93276-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93276-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93276-111">Permission type</span></span>|<span data-ttu-id="93276-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="93276-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93276-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93276-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93276-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93276-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="93276-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93276-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93276-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93276-116">Not supported.</span></span>|
|<span data-ttu-id="93276-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93276-117">Application</span></span>|<span data-ttu-id="93276-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93276-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93276-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93276-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="93276-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="93276-120">Request headers</span></span>
|<span data-ttu-id="93276-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93276-121">Header</span></span>|<span data-ttu-id="93276-122">Значение</span><span class="sxs-lookup"><span data-stu-id="93276-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93276-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="93276-123">Authorization</span></span>|<span data-ttu-id="93276-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93276-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93276-125">Accept</span><span class="sxs-lookup"><span data-stu-id="93276-125">Accept</span></span>|<span data-ttu-id="93276-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93276-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93276-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93276-127">Request body</span></span>
<span data-ttu-id="93276-128">В тексте запроса добавьте представление объекта [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93276-128">In the request body, supply a JSON representation for the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="93276-129">В следующей таблице приведены свойства, необходимые при создании [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="93276-129">The following table shows the properties that are required when you create the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="93276-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="93276-130">Property</span></span>|<span data-ttu-id="93276-131">Тип</span><span class="sxs-lookup"><span data-stu-id="93276-131">Type</span></span>|<span data-ttu-id="93276-132">Описание</span><span class="sxs-lookup"><span data-stu-id="93276-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93276-133">id</span><span class="sxs-lookup"><span data-stu-id="93276-133">id</span></span>|<span data-ttu-id="93276-134">Строка</span><span class="sxs-lookup"><span data-stu-id="93276-134">String</span></span>|<span data-ttu-id="93276-135">Ключ профиля, наследуемый от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93276-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="93276-136">displayName</span><span class="sxs-lookup"><span data-stu-id="93276-136">displayName</span></span>|<span data-ttu-id="93276-137">Строка</span><span class="sxs-lookup"><span data-stu-id="93276-137">String</span></span>|<span data-ttu-id="93276-138">Имя профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93276-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="93276-139">description</span><span class="sxs-lookup"><span data-stu-id="93276-139">description</span></span>|<span data-ttu-id="93276-140">String</span><span class="sxs-lookup"><span data-stu-id="93276-140">String</span></span>|<span data-ttu-id="93276-141">Описание профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93276-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="93276-142">language</span><span class="sxs-lookup"><span data-stu-id="93276-142">language</span></span>|<span data-ttu-id="93276-143">String</span><span class="sxs-lookup"><span data-stu-id="93276-143">String</span></span>|<span data-ttu-id="93276-144">Язык, настроенный на устройстве, унаследованном от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93276-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="93276-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93276-145">createdDateTime</span></span>|<span data-ttu-id="93276-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93276-146">DateTimeOffset</span></span>|<span data-ttu-id="93276-147">Время создания профиля, унаследованное от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93276-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="93276-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93276-148">lastModifiedDateTime</span></span>|<span data-ttu-id="93276-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93276-149">DateTimeOffset</span></span>|<span data-ttu-id="93276-150">Время последнего изменения профиля, наследуемого от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93276-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="93276-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="93276-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="93276-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="93276-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="93276-153">Настройка "от" в рамке наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93276-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="93276-154">енроллментстатусскринсеттингс</span><span class="sxs-lookup"><span data-stu-id="93276-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="93276-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="93276-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="93276-156">Параметр экрана состояния регистрации, наследуемый от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93276-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="93276-157">екстраксардварехаш</span><span class="sxs-lookup"><span data-stu-id="93276-157">extractHardwareHash</span></span>|<span data-ttu-id="93276-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="93276-158">Boolean</span></span>|<span data-ttu-id="93276-159">Извлечение Хардварехаш для профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93276-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="93276-160">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="93276-160">deviceNameTemplate</span></span>|<span data-ttu-id="93276-161">Строка</span><span class="sxs-lookup"><span data-stu-id="93276-161">String</span></span>|<span data-ttu-id="93276-162">Шаблон, используемый для именования автопилотного устройства.</span><span class="sxs-lookup"><span data-stu-id="93276-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="93276-163">Это может быть настраиваемый текст, который также может содержать серийный номер устройства или случайное число.</span><span class="sxs-lookup"><span data-stu-id="93276-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="93276-164">Общая длина текста, созданного шаблоном, не может превышать 15 символов.</span><span class="sxs-lookup"><span data-stu-id="93276-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="93276-165">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93276-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="93276-166">deviceType</span><span class="sxs-lookup"><span data-stu-id="93276-166">deviceType</span></span>|[<span data-ttu-id="93276-167">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="93276-167">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="93276-168">Тип устройства автопилота, к которому применяется этот профиль.</span><span class="sxs-lookup"><span data-stu-id="93276-168">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="93276-169">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="93276-169">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="93276-170">Возможные значения: `windowsPc`, `surfaceHub2`, `holoLens`.</span><span class="sxs-lookup"><span data-stu-id="93276-170">Possible values are: `windowsPc`, `surfaceHub2`, `holoLens`.</span></span>|
|<span data-ttu-id="93276-171">енаблевхитеглове</span><span class="sxs-lookup"><span data-stu-id="93276-171">enableWhiteGlove</span></span>|<span data-ttu-id="93276-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="93276-172">Boolean</span></span>|<span data-ttu-id="93276-173">Включите для профиля белый Глове для автопилотного развертывания.</span><span class="sxs-lookup"><span data-stu-id="93276-173">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="93276-174">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93276-174">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="93276-175">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="93276-175">roleScopeTagIds</span></span>|<span data-ttu-id="93276-176">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="93276-176">String collection</span></span>|<span data-ttu-id="93276-177">Теги областей для профиля.</span><span class="sxs-lookup"><span data-stu-id="93276-177">Scope tags for the profile.</span></span> <span data-ttu-id="93276-178">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="93276-178">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="93276-179">хибридазуреаджоинскипконнективитичекк</span><span class="sxs-lookup"><span data-stu-id="93276-179">hybridAzureADJoinSkipConnectivityCheck</span></span>|<span data-ttu-id="93276-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="93276-180">Boolean</span></span>|<span data-ttu-id="93276-181">Процесс самопилотного подключения к гибридной среде Azure AD продолжится даже в том случае, если он не устанавливает подключение к контроллеру домена во время OOBE.</span><span class="sxs-lookup"><span data-stu-id="93276-181">The Autopilot Hybrid Azure AD join flow will continue even if it does not establish domain controller connectivity during OOBE.</span></span>|



## <a name="response"></a><span data-ttu-id="93276-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="93276-182">Response</span></span>
<span data-ttu-id="93276-183">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="93276-183">If successful, this method returns a `200 OK` response code and an updated [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93276-184">Пример</span><span class="sxs-lookup"><span data-stu-id="93276-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="93276-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="93276-185">Request</span></span>
<span data-ttu-id="93276-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93276-186">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1218

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
  ],
  "hybridAzureADJoinSkipConnectivityCheck": true
}
```

### <a name="response"></a><span data-ttu-id="93276-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="93276-187">Response</span></span>
<span data-ttu-id="93276-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93276-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1390

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
  ],
  "hybridAzureADJoinSkipConnectivityCheck": true
}
```






