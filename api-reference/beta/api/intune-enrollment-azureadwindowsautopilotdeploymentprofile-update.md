---
title: Обновление azureADWindowsAutopilotDeploymentProfile
description: Обновление свойств объекта azureADWindowsAutopilotDeploymentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c51ab8c146678aa6e01aaa187cee1fcc6d2145cb
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149963"
---
# <a name="update-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="f29f8-103">Обновление azureADWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="f29f8-103">Update azureADWindowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="f29f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f29f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f29f8-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f29f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f29f8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f29f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f29f8-107">Обновление свойств объекта [azureADWindowsAutopilotDeploymentProfile.](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f29f8-107">Update the properties of a [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f29f8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f29f8-108">Prerequisites</span></span>
<span data-ttu-id="f29f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f29f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f29f8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f29f8-111">Permission type</span></span>|<span data-ttu-id="f29f8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f29f8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f29f8-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f29f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f29f8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f29f8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f29f8-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f29f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f29f8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f29f8-116">Not supported.</span></span>|
|<span data-ttu-id="f29f8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f29f8-117">Application</span></span>|<span data-ttu-id="f29f8-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f29f8-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f29f8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f29f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="f29f8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f29f8-120">Request headers</span></span>
|<span data-ttu-id="f29f8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f29f8-121">Header</span></span>|<span data-ttu-id="f29f8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f29f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f29f8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f29f8-123">Authorization</span></span>|<span data-ttu-id="f29f8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f29f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f29f8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f29f8-125">Accept</span></span>|<span data-ttu-id="f29f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f29f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f29f8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f29f8-127">Request body</span></span>
<span data-ttu-id="f29f8-128">В теле запроса поставляем представление JSON для [объекта azureADWindowsAutopilotDeploymentProfile.](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f29f8-128">In the request body, supply a JSON representation for the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="f29f8-129">В следующей таблице показаны свойства, необходимые при создании [azureADWindowsAutopilotDeploymentProfile.](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f29f8-129">The following table shows the properties that are required when you create the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="f29f8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f29f8-130">Property</span></span>|<span data-ttu-id="f29f8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f29f8-131">Type</span></span>|<span data-ttu-id="f29f8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f29f8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f29f8-133">id</span><span class="sxs-lookup"><span data-stu-id="f29f8-133">id</span></span>|<span data-ttu-id="f29f8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f29f8-134">String</span></span>|<span data-ttu-id="f29f8-135">Ключ профиля, унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f29f8-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f29f8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f29f8-136">displayName</span></span>|<span data-ttu-id="f29f8-137">Строка</span><span class="sxs-lookup"><span data-stu-id="f29f8-137">String</span></span>|<span data-ttu-id="f29f8-138">Имя профиля, наследуемого [из windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f29f8-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f29f8-139">description</span><span class="sxs-lookup"><span data-stu-id="f29f8-139">description</span></span>|<span data-ttu-id="f29f8-140">Строка</span><span class="sxs-lookup"><span data-stu-id="f29f8-140">String</span></span>|<span data-ttu-id="f29f8-141">Описание профиля, наследуемого [из windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f29f8-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f29f8-142">language</span><span class="sxs-lookup"><span data-stu-id="f29f8-142">language</span></span>|<span data-ttu-id="f29f8-143">String</span><span class="sxs-lookup"><span data-stu-id="f29f8-143">String</span></span>|<span data-ttu-id="f29f8-144">Язык, настроенный на устройстве, наследуемом [из windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f29f8-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f29f8-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f29f8-145">createdDateTime</span></span>|<span data-ttu-id="f29f8-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f29f8-146">DateTimeOffset</span></span>|<span data-ttu-id="f29f8-147">Время создания профилей, унаследованных от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f29f8-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f29f8-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f29f8-148">lastModifiedDateTime</span></span>|<span data-ttu-id="f29f8-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f29f8-149">DateTimeOffset</span></span>|<span data-ttu-id="f29f8-150">Последний измененный профиль из [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f29f8-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f29f8-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="f29f8-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="f29f8-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="f29f8-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="f29f8-153">Параметр "Вне полей", унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f29f8-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f29f8-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="f29f8-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="f29f8-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="f29f8-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="f29f8-156">Параметр состояния регистрации, унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f29f8-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f29f8-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="f29f8-157">extractHardwareHash</span></span>|<span data-ttu-id="f29f8-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="f29f8-158">Boolean</span></span>|<span data-ttu-id="f29f8-159">HardwareHash Extraction для профиля, унаследованной от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f29f8-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f29f8-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="f29f8-160">deviceNameTemplate</span></span>|<span data-ttu-id="f29f8-161">Строка</span><span class="sxs-lookup"><span data-stu-id="f29f8-161">String</span></span>|<span data-ttu-id="f29f8-162">Шаблон, используемый для имени устройства АвтоПилот.</span><span class="sxs-lookup"><span data-stu-id="f29f8-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="f29f8-163">Это может быть пользовательский текст, который также может содержать либо серийный номер устройства, либо случайный генерируемый номер.</span><span class="sxs-lookup"><span data-stu-id="f29f8-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="f29f8-164">Общая длина текста, генерируемого шаблоном, может быть не более 15 символов.</span><span class="sxs-lookup"><span data-stu-id="f29f8-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="f29f8-165">Унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f29f8-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f29f8-166">deviceType</span><span class="sxs-lookup"><span data-stu-id="f29f8-166">deviceType</span></span>|[<span data-ttu-id="f29f8-167">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="f29f8-167">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="f29f8-168">Тип устройства AutoPilot, к который применим этот профиль.</span><span class="sxs-lookup"><span data-stu-id="f29f8-168">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="f29f8-169">Наследуется [от windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f29f8-169">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="f29f8-170">Возможные значения: `windowsPc`, `surfaceHub2`, `holoLens`.</span><span class="sxs-lookup"><span data-stu-id="f29f8-170">Possible values are: `windowsPc`, `surfaceHub2`, `holoLens`.</span></span>|
|<span data-ttu-id="f29f8-171">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="f29f8-171">enableWhiteGlove</span></span>|<span data-ttu-id="f29f8-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="f29f8-172">Boolean</span></span>|<span data-ttu-id="f29f8-173">Включить белую перчатку автопилота для профиля.</span><span class="sxs-lookup"><span data-stu-id="f29f8-173">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="f29f8-174">Унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f29f8-174">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f29f8-175">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f29f8-175">roleScopeTagIds</span></span>|<span data-ttu-id="f29f8-176">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f29f8-176">String collection</span></span>|<span data-ttu-id="f29f8-177">Теги области для профиля.</span><span class="sxs-lookup"><span data-stu-id="f29f8-177">Scope tags for the profile.</span></span> <span data-ttu-id="f29f8-178">Унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f29f8-178">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f29f8-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="f29f8-179">Response</span></span>
<span data-ttu-id="f29f8-180">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f29f8-180">If successful, this method returns a `200 OK` response code and an updated [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f29f8-181">Пример</span><span class="sxs-lookup"><span data-stu-id="f29f8-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="f29f8-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="f29f8-182">Request</span></span>
<span data-ttu-id="f29f8-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f29f8-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1159

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
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="f29f8-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="f29f8-184">Response</span></span>
<span data-ttu-id="f29f8-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f29f8-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1331

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
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




