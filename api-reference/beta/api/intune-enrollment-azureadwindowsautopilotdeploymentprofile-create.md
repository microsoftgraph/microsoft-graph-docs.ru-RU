---
title: Создание azureADWindowsAutopilotDeploymentProfile
description: Создайте новый объект azureADWindowsAutopilotDeploymentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 94c8816c71808a2ee7175cf89c90d78d0ba6cbd7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146050"
---
# <a name="create-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="0ba97-103">Создание azureADWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="0ba97-103">Create azureADWindowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="0ba97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ba97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ba97-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ba97-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ba97-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ba97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ba97-107">Создайте новый [объект azureADWindowsAutopilotDeploymentProfile.](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ba97-107">Create a new [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ba97-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0ba97-108">Prerequisites</span></span>
<span data-ttu-id="0ba97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ba97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ba97-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ba97-111">Permission type</span></span>|<span data-ttu-id="0ba97-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ba97-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ba97-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ba97-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ba97-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ba97-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0ba97-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ba97-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ba97-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ba97-116">Not supported.</span></span>|
|<span data-ttu-id="0ba97-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0ba97-117">Application</span></span>|<span data-ttu-id="0ba97-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ba97-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ba97-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ba97-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="0ba97-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0ba97-120">Request headers</span></span>
|<span data-ttu-id="0ba97-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ba97-121">Header</span></span>|<span data-ttu-id="0ba97-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0ba97-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ba97-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ba97-123">Authorization</span></span>|<span data-ttu-id="0ba97-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ba97-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ba97-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ba97-125">Accept</span></span>|<span data-ttu-id="0ba97-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ba97-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ba97-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ba97-127">Request body</span></span>
<span data-ttu-id="0ba97-128">В теле запроса поставляем представление JSON для объекта azureADWindowsAutopilotDeploymentProfile.</span><span class="sxs-lookup"><span data-stu-id="0ba97-128">In the request body, supply a JSON representation for the azureADWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="0ba97-129">В следующей таблице показаны свойства, необходимые при создании azureADWindowsAutopilotDeploymentProfile.</span><span class="sxs-lookup"><span data-stu-id="0ba97-129">The following table shows the properties that are required when you create the azureADWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="0ba97-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ba97-130">Property</span></span>|<span data-ttu-id="0ba97-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0ba97-131">Type</span></span>|<span data-ttu-id="0ba97-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0ba97-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ba97-133">id</span><span class="sxs-lookup"><span data-stu-id="0ba97-133">id</span></span>|<span data-ttu-id="0ba97-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0ba97-134">String</span></span>|<span data-ttu-id="0ba97-135">Ключ профиля, унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ba97-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="0ba97-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0ba97-136">displayName</span></span>|<span data-ttu-id="0ba97-137">Строка</span><span class="sxs-lookup"><span data-stu-id="0ba97-137">String</span></span>|<span data-ttu-id="0ba97-138">Имя профиля, наследуемого [из windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ba97-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="0ba97-139">description</span><span class="sxs-lookup"><span data-stu-id="0ba97-139">description</span></span>|<span data-ttu-id="0ba97-140">Строка</span><span class="sxs-lookup"><span data-stu-id="0ba97-140">String</span></span>|<span data-ttu-id="0ba97-141">Описание профиля, наследуемого [из windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ba97-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="0ba97-142">language</span><span class="sxs-lookup"><span data-stu-id="0ba97-142">language</span></span>|<span data-ttu-id="0ba97-143">String</span><span class="sxs-lookup"><span data-stu-id="0ba97-143">String</span></span>|<span data-ttu-id="0ba97-144">Язык, настроенный на устройстве, наследуемом [из windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ba97-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="0ba97-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ba97-145">createdDateTime</span></span>|<span data-ttu-id="0ba97-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ba97-146">DateTimeOffset</span></span>|<span data-ttu-id="0ba97-147">Время создания профилей, унаследованных от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ba97-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="0ba97-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ba97-148">lastModifiedDateTime</span></span>|<span data-ttu-id="0ba97-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ba97-149">DateTimeOffset</span></span>|<span data-ttu-id="0ba97-150">Последний измененный профиль из [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ba97-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="0ba97-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="0ba97-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="0ba97-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="0ba97-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="0ba97-153">Параметр "Вне полей", унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ba97-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="0ba97-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="0ba97-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="0ba97-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="0ba97-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="0ba97-156">Параметр состояния регистрации, унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ba97-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="0ba97-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="0ba97-157">extractHardwareHash</span></span>|<span data-ttu-id="0ba97-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ba97-158">Boolean</span></span>|<span data-ttu-id="0ba97-159">HardwareHash Extraction для профиля, унаследованной от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ba97-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="0ba97-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="0ba97-160">deviceNameTemplate</span></span>|<span data-ttu-id="0ba97-161">Строка</span><span class="sxs-lookup"><span data-stu-id="0ba97-161">String</span></span>|<span data-ttu-id="0ba97-162">Шаблон, используемый для имени устройства АвтоПилот.</span><span class="sxs-lookup"><span data-stu-id="0ba97-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="0ba97-163">Это может быть пользовательский текст, который также может содержать либо серийный номер устройства, либо случайный генерируемый номер.</span><span class="sxs-lookup"><span data-stu-id="0ba97-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="0ba97-164">Общая длина текста, генерируемого шаблоном, может быть не более 15 символов.</span><span class="sxs-lookup"><span data-stu-id="0ba97-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="0ba97-165">Унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ba97-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="0ba97-166">deviceType</span><span class="sxs-lookup"><span data-stu-id="0ba97-166">deviceType</span></span>|[<span data-ttu-id="0ba97-167">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="0ba97-167">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="0ba97-168">Тип устройства AutoPilot, к который применим этот профиль.</span><span class="sxs-lookup"><span data-stu-id="0ba97-168">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="0ba97-169">Наследуется [от windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="0ba97-169">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="0ba97-170">Возможные значения: `windowsPc`, `surfaceHub2`, `holoLens`.</span><span class="sxs-lookup"><span data-stu-id="0ba97-170">Possible values are: `windowsPc`, `surfaceHub2`, `holoLens`.</span></span>|
|<span data-ttu-id="0ba97-171">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="0ba97-171">enableWhiteGlove</span></span>|<span data-ttu-id="0ba97-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ba97-172">Boolean</span></span>|<span data-ttu-id="0ba97-173">Включить белую перчатку автопилота для профиля.</span><span class="sxs-lookup"><span data-stu-id="0ba97-173">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="0ba97-174">Унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ba97-174">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="0ba97-175">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0ba97-175">roleScopeTagIds</span></span>|<span data-ttu-id="0ba97-176">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0ba97-176">String collection</span></span>|<span data-ttu-id="0ba97-177">Теги области для профиля.</span><span class="sxs-lookup"><span data-stu-id="0ba97-177">Scope tags for the profile.</span></span> <span data-ttu-id="0ba97-178">Унаследованный от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ba97-178">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0ba97-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ba97-179">Response</span></span>
<span data-ttu-id="0ba97-180">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0ba97-180">If successful, this method returns a `201 Created` response code and a [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ba97-181">Пример</span><span class="sxs-lookup"><span data-stu-id="0ba97-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ba97-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ba97-182">Request</span></span>
<span data-ttu-id="0ba97-183">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ba97-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
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

### <a name="response"></a><span data-ttu-id="0ba97-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ba97-184">Response</span></span>
<span data-ttu-id="0ba97-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ba97-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




