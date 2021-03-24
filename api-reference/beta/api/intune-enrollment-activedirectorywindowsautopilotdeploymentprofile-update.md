---
title: Обновление activeDirectoryWindowsAutopilotDeploymentProfile
description: Обновление свойств объекта activeDirectoryWindowsAutopilotDeploymentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 69d91e90dfd21f67690c58931e4204a94da96622
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126278"
---
# <a name="update-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="c8235-103">Обновление activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="c8235-103">Update activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="c8235-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8235-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8235-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8235-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8235-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8235-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8235-107">Обновление свойств объекта [activeDirectoryWindowsAutopilotDeploymentProfile.](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c8235-107">Update the properties of a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8235-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c8235-108">Prerequisites</span></span>
<span data-ttu-id="c8235-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8235-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8235-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8235-111">Permission type</span></span>|<span data-ttu-id="c8235-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8235-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8235-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8235-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8235-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8235-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c8235-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8235-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8235-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8235-116">Not supported.</span></span>|
|<span data-ttu-id="c8235-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c8235-117">Application</span></span>|<span data-ttu-id="c8235-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8235-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8235-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8235-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="c8235-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c8235-120">Request headers</span></span>
|<span data-ttu-id="c8235-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8235-121">Header</span></span>|<span data-ttu-id="c8235-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c8235-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8235-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8235-123">Authorization</span></span>|<span data-ttu-id="c8235-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8235-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8235-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c8235-125">Accept</span></span>|<span data-ttu-id="c8235-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8235-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8235-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8235-127">Request body</span></span>
<span data-ttu-id="c8235-128">В теле запроса поставляем представление JSON для [объекта activeDirectoryWindowsAutopilotDeploymentProfile.](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c8235-128">In the request body, supply a JSON representation for the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="c8235-129">В следующей таблице показаны свойства, необходимые при создании [activeDirectoryWindowsAutopilotDeploymentProfile.](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c8235-129">The following table shows the properties that are required when you create the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="c8235-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8235-130">Property</span></span>|<span data-ttu-id="c8235-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c8235-131">Type</span></span>|<span data-ttu-id="c8235-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c8235-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8235-133">id</span><span class="sxs-lookup"><span data-stu-id="c8235-133">id</span></span>|<span data-ttu-id="c8235-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c8235-134">String</span></span>|<span data-ttu-id="c8235-135">Ключ профиля, унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c8235-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c8235-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c8235-136">displayName</span></span>|<span data-ttu-id="c8235-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c8235-137">String</span></span>|<span data-ttu-id="c8235-138">Имя профиля, наследуемого [из windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c8235-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c8235-139">description</span><span class="sxs-lookup"><span data-stu-id="c8235-139">description</span></span>|<span data-ttu-id="c8235-140">Строка</span><span class="sxs-lookup"><span data-stu-id="c8235-140">String</span></span>|<span data-ttu-id="c8235-141">Описание профиля, наследуемого [из windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c8235-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c8235-142">language</span><span class="sxs-lookup"><span data-stu-id="c8235-142">language</span></span>|<span data-ttu-id="c8235-143">String</span><span class="sxs-lookup"><span data-stu-id="c8235-143">String</span></span>|<span data-ttu-id="c8235-144">Язык, настроенный на устройстве, наследуемом [из windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c8235-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c8235-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8235-145">createdDateTime</span></span>|<span data-ttu-id="c8235-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8235-146">DateTimeOffset</span></span>|<span data-ttu-id="c8235-147">Время создания профилей, унаследованных от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c8235-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c8235-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8235-148">lastModifiedDateTime</span></span>|<span data-ttu-id="c8235-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8235-149">DateTimeOffset</span></span>|<span data-ttu-id="c8235-150">Последний измененный профиль из [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c8235-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c8235-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="c8235-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="c8235-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="c8235-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="c8235-153">Параметр "Вне полей", унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c8235-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c8235-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="c8235-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="c8235-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="c8235-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="c8235-156">Параметр состояния регистрации, унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c8235-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c8235-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="c8235-157">extractHardwareHash</span></span>|<span data-ttu-id="c8235-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8235-158">Boolean</span></span>|<span data-ttu-id="c8235-159">HardwareHash Extraction для профиля, унаследованной от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c8235-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c8235-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="c8235-160">deviceNameTemplate</span></span>|<span data-ttu-id="c8235-161">Строка</span><span class="sxs-lookup"><span data-stu-id="c8235-161">String</span></span>|<span data-ttu-id="c8235-162">Шаблон, используемый для имени устройства АвтоПилот.</span><span class="sxs-lookup"><span data-stu-id="c8235-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="c8235-163">Это может быть пользовательский текст, который также может содержать либо серийный номер устройства, либо случайный генерируемый номер.</span><span class="sxs-lookup"><span data-stu-id="c8235-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="c8235-164">Общая длина текста, генерируемого шаблоном, может быть не более 15 символов.</span><span class="sxs-lookup"><span data-stu-id="c8235-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="c8235-165">Унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c8235-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c8235-166">deviceType</span><span class="sxs-lookup"><span data-stu-id="c8235-166">deviceType</span></span>|[<span data-ttu-id="c8235-167">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="c8235-167">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="c8235-168">Тип устройства AutoPilot, к который применим этот профиль.</span><span class="sxs-lookup"><span data-stu-id="c8235-168">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="c8235-169">Наследуется [от windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="c8235-169">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="c8235-170">Возможные значения: `windowsPc`, `surfaceHub2`, `holoLens`.</span><span class="sxs-lookup"><span data-stu-id="c8235-170">Possible values are: `windowsPc`, `surfaceHub2`, `holoLens`.</span></span>|
|<span data-ttu-id="c8235-171">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="c8235-171">enableWhiteGlove</span></span>|<span data-ttu-id="c8235-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8235-172">Boolean</span></span>|<span data-ttu-id="c8235-173">Включить белую перчатку автопилота для профиля.</span><span class="sxs-lookup"><span data-stu-id="c8235-173">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="c8235-174">Унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c8235-174">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c8235-175">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c8235-175">roleScopeTagIds</span></span>|<span data-ttu-id="c8235-176">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c8235-176">String collection</span></span>|<span data-ttu-id="c8235-177">Теги области для профиля.</span><span class="sxs-lookup"><span data-stu-id="c8235-177">Scope tags for the profile.</span></span> <span data-ttu-id="c8235-178">Унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c8235-178">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c8235-179">hybridAzureADJoinSkipConnectivityCheck</span><span class="sxs-lookup"><span data-stu-id="c8235-179">hybridAzureADJoinSkipConnectivityCheck</span></span>|<span data-ttu-id="c8235-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8235-180">Boolean</span></span>|<span data-ttu-id="c8235-181">Поток подключения гибридного Azure AD автопилота будет продолжаться, даже если он не устанавливает подключение контроллера домена во время OOBE.</span><span class="sxs-lookup"><span data-stu-id="c8235-181">The Autopilot Hybrid Azure AD join flow will continue even if it does not establish domain controller connectivity during OOBE.</span></span>|



## <a name="response"></a><span data-ttu-id="c8235-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8235-182">Response</span></span>
<span data-ttu-id="c8235-183">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c8235-183">If successful, this method returns a `200 OK` response code and an updated [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8235-184">Пример</span><span class="sxs-lookup"><span data-stu-id="c8235-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8235-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8235-185">Request</span></span>
<span data-ttu-id="c8235-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8235-186">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c8235-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8235-187">Response</span></span>
<span data-ttu-id="c8235-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8235-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




