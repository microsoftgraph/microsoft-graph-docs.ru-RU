---
title: Создание activeDirectoryWindowsAutopilotDeploymentProfile
description: Создайте новый объект activeDirectoryWindowsAutopilotDeploymentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d6eade2ae570bd0c4efa70f248ba8c04fc135d73
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135826"
---
# <a name="create-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="536f9-103">Создание activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="536f9-103">Create activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="536f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="536f9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="536f9-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="536f9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="536f9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="536f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="536f9-107">Создайте новый [объект activeDirectoryWindowsAutopilotDeploymentProfile.](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="536f9-107">Create a new [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="536f9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="536f9-108">Prerequisites</span></span>
<span data-ttu-id="536f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="536f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="536f9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="536f9-111">Permission type</span></span>|<span data-ttu-id="536f9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="536f9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="536f9-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="536f9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="536f9-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="536f9-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="536f9-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="536f9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="536f9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="536f9-116">Not supported.</span></span>|
|<span data-ttu-id="536f9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="536f9-117">Application</span></span>|<span data-ttu-id="536f9-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="536f9-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="536f9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="536f9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="536f9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="536f9-120">Request headers</span></span>
|<span data-ttu-id="536f9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="536f9-121">Header</span></span>|<span data-ttu-id="536f9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="536f9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="536f9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="536f9-123">Authorization</span></span>|<span data-ttu-id="536f9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="536f9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="536f9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="536f9-125">Accept</span></span>|<span data-ttu-id="536f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="536f9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="536f9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="536f9-127">Request body</span></span>
<span data-ttu-id="536f9-128">В теле запроса поставляем представление JSON для объекта activeDirectoryWindowsAutopilotDeploymentProfile.</span><span class="sxs-lookup"><span data-stu-id="536f9-128">In the request body, supply a JSON representation for the activeDirectoryWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="536f9-129">В следующей таблице показаны свойства, необходимые при создании activeDirectoryWindowsAutopilotDeploymentProfile.</span><span class="sxs-lookup"><span data-stu-id="536f9-129">The following table shows the properties that are required when you create the activeDirectoryWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="536f9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="536f9-130">Property</span></span>|<span data-ttu-id="536f9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="536f9-131">Type</span></span>|<span data-ttu-id="536f9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="536f9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="536f9-133">id</span><span class="sxs-lookup"><span data-stu-id="536f9-133">id</span></span>|<span data-ttu-id="536f9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="536f9-134">String</span></span>|<span data-ttu-id="536f9-135">Ключ профиля, унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="536f9-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="536f9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="536f9-136">displayName</span></span>|<span data-ttu-id="536f9-137">Строка</span><span class="sxs-lookup"><span data-stu-id="536f9-137">String</span></span>|<span data-ttu-id="536f9-138">Имя профиля, наследуемого [из windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="536f9-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="536f9-139">description</span><span class="sxs-lookup"><span data-stu-id="536f9-139">description</span></span>|<span data-ttu-id="536f9-140">Строка</span><span class="sxs-lookup"><span data-stu-id="536f9-140">String</span></span>|<span data-ttu-id="536f9-141">Описание профиля, наследуемого [из windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="536f9-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="536f9-142">language</span><span class="sxs-lookup"><span data-stu-id="536f9-142">language</span></span>|<span data-ttu-id="536f9-143">String</span><span class="sxs-lookup"><span data-stu-id="536f9-143">String</span></span>|<span data-ttu-id="536f9-144">Язык, настроенный на устройстве, наследуемом [из windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="536f9-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="536f9-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="536f9-145">createdDateTime</span></span>|<span data-ttu-id="536f9-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="536f9-146">DateTimeOffset</span></span>|<span data-ttu-id="536f9-147">Время создания профилей, унаследованных от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="536f9-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="536f9-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="536f9-148">lastModifiedDateTime</span></span>|<span data-ttu-id="536f9-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="536f9-149">DateTimeOffset</span></span>|<span data-ttu-id="536f9-150">Последний измененный профиль из [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="536f9-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="536f9-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="536f9-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="536f9-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="536f9-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="536f9-153">Параметр "Вне полей", унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="536f9-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="536f9-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="536f9-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="536f9-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="536f9-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="536f9-156">Параметр состояния регистрации, унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="536f9-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="536f9-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="536f9-157">extractHardwareHash</span></span>|<span data-ttu-id="536f9-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="536f9-158">Boolean</span></span>|<span data-ttu-id="536f9-159">HardwareHash Extraction для профиля, унаследованной от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="536f9-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="536f9-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="536f9-160">deviceNameTemplate</span></span>|<span data-ttu-id="536f9-161">Строка</span><span class="sxs-lookup"><span data-stu-id="536f9-161">String</span></span>|<span data-ttu-id="536f9-162">Шаблон, используемый для имени устройства АвтоПилот.</span><span class="sxs-lookup"><span data-stu-id="536f9-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="536f9-163">Это может быть пользовательский текст, который также может содержать либо серийный номер устройства, либо случайный генерируемый номер.</span><span class="sxs-lookup"><span data-stu-id="536f9-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="536f9-164">Общая длина текста, генерируемого шаблоном, может быть не более 15 символов.</span><span class="sxs-lookup"><span data-stu-id="536f9-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="536f9-165">Унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="536f9-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="536f9-166">deviceType</span><span class="sxs-lookup"><span data-stu-id="536f9-166">deviceType</span></span>|[<span data-ttu-id="536f9-167">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="536f9-167">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="536f9-168">Тип устройства AutoPilot, к который применим этот профиль.</span><span class="sxs-lookup"><span data-stu-id="536f9-168">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="536f9-169">Наследуется [от windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="536f9-169">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="536f9-170">Возможные значения: `windowsPc`, `surfaceHub2`, `holoLens`.</span><span class="sxs-lookup"><span data-stu-id="536f9-170">Possible values are: `windowsPc`, `surfaceHub2`, `holoLens`.</span></span>|
|<span data-ttu-id="536f9-171">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="536f9-171">enableWhiteGlove</span></span>|<span data-ttu-id="536f9-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="536f9-172">Boolean</span></span>|<span data-ttu-id="536f9-173">Включить белую перчатку автопилота для профиля.</span><span class="sxs-lookup"><span data-stu-id="536f9-173">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="536f9-174">Унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="536f9-174">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="536f9-175">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="536f9-175">roleScopeTagIds</span></span>|<span data-ttu-id="536f9-176">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="536f9-176">String collection</span></span>|<span data-ttu-id="536f9-177">Теги области для профиля.</span><span class="sxs-lookup"><span data-stu-id="536f9-177">Scope tags for the profile.</span></span> <span data-ttu-id="536f9-178">Унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="536f9-178">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="536f9-179">hybridAzureADJoinSkipConnectivityCheck</span><span class="sxs-lookup"><span data-stu-id="536f9-179">hybridAzureADJoinSkipConnectivityCheck</span></span>|<span data-ttu-id="536f9-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="536f9-180">Boolean</span></span>|<span data-ttu-id="536f9-181">Поток подключения гибридного Azure AD автопилота будет продолжаться, даже если он не устанавливает подключение контроллера домена во время OOBE.</span><span class="sxs-lookup"><span data-stu-id="536f9-181">The Autopilot Hybrid Azure AD join flow will continue even if it does not establish domain controller connectivity during OOBE.</span></span>|



## <a name="response"></a><span data-ttu-id="536f9-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="536f9-182">Response</span></span>
<span data-ttu-id="536f9-183">В случае успешного выполнения этот метод возвращает код ответа и `201 Created` [объект activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="536f9-183">If successful, this method returns a `201 Created` response code and a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="536f9-184">Пример</span><span class="sxs-lookup"><span data-stu-id="536f9-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="536f9-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="536f9-185">Request</span></span>
<span data-ttu-id="536f9-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="536f9-186">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
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

### <a name="response"></a><span data-ttu-id="536f9-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="536f9-187">Response</span></span>
<span data-ttu-id="536f9-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="536f9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




