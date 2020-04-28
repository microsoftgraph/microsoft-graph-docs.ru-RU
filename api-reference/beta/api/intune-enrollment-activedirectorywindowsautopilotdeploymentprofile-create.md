---
title: Создание Активедиректоривиндовсаутопилотдеплойментпрофиле
description: Создание нового объекта Активедиректоривиндовсаутопилотдеплойментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 416afe32e7aa95ea97d32ea93837a574ffd65e91
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43378129"
---
# <a name="create-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="e5353-103">Создание Активедиректоривиндовсаутопилотдеплойментпрофиле</span><span class="sxs-lookup"><span data-stu-id="e5353-103">Create activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="e5353-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5353-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5353-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5353-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5353-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5353-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5353-107">Создание нового объекта [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e5353-107">Create a new [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5353-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e5353-108">Prerequisites</span></span>
<span data-ttu-id="e5353-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5353-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5353-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5353-111">Permission type</span></span>|<span data-ttu-id="e5353-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5353-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5353-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5353-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5353-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5353-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e5353-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5353-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5353-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5353-116">Not supported.</span></span>|
|<span data-ttu-id="e5353-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5353-117">Application</span></span>|<span data-ttu-id="e5353-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5353-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5353-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5353-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="e5353-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e5353-120">Request headers</span></span>
|<span data-ttu-id="e5353-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5353-121">Header</span></span>|<span data-ttu-id="e5353-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e5353-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5353-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5353-123">Authorization</span></span>|<span data-ttu-id="e5353-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5353-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5353-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e5353-125">Accept</span></span>|<span data-ttu-id="e5353-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5353-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5353-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e5353-127">Request body</span></span>
<span data-ttu-id="e5353-128">В тексте запроса добавьте представление объекта Активедиректоривиндовсаутопилотдеплойментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5353-128">In the request body, supply a JSON representation for the activeDirectoryWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="e5353-129">В следующей таблице приведены свойства, необходимые при создании Активедиректоривиндовсаутопилотдеплойментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="e5353-129">The following table shows the properties that are required when you create the activeDirectoryWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="e5353-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5353-130">Property</span></span>|<span data-ttu-id="e5353-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e5353-131">Type</span></span>|<span data-ttu-id="e5353-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e5353-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5353-133">id</span><span class="sxs-lookup"><span data-stu-id="e5353-133">id</span></span>|<span data-ttu-id="e5353-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e5353-134">String</span></span>|<span data-ttu-id="e5353-135">Ключ профиля, наследуемый от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e5353-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e5353-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e5353-136">displayName</span></span>|<span data-ttu-id="e5353-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e5353-137">String</span></span>|<span data-ttu-id="e5353-138">Имя профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e5353-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e5353-139">description</span><span class="sxs-lookup"><span data-stu-id="e5353-139">description</span></span>|<span data-ttu-id="e5353-140">String</span><span class="sxs-lookup"><span data-stu-id="e5353-140">String</span></span>|<span data-ttu-id="e5353-141">Описание профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e5353-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e5353-142">language</span><span class="sxs-lookup"><span data-stu-id="e5353-142">language</span></span>|<span data-ttu-id="e5353-143">String</span><span class="sxs-lookup"><span data-stu-id="e5353-143">String</span></span>|<span data-ttu-id="e5353-144">Язык, настроенный на устройстве, унаследованном от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e5353-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e5353-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5353-145">createdDateTime</span></span>|<span data-ttu-id="e5353-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5353-146">DateTimeOffset</span></span>|<span data-ttu-id="e5353-147">Время создания профиля, унаследованное от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e5353-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e5353-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5353-148">lastModifiedDateTime</span></span>|<span data-ttu-id="e5353-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5353-149">DateTimeOffset</span></span>|<span data-ttu-id="e5353-150">Время последнего изменения профиля, наследуемого от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e5353-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e5353-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="e5353-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="e5353-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="e5353-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="e5353-153">Настройка "от" в рамке наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e5353-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e5353-154">енроллментстатусскринсеттингс</span><span class="sxs-lookup"><span data-stu-id="e5353-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="e5353-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="e5353-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="e5353-156">Параметр экрана состояния регистрации, наследуемый от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e5353-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e5353-157">екстраксардварехаш</span><span class="sxs-lookup"><span data-stu-id="e5353-157">extractHardwareHash</span></span>|<span data-ttu-id="e5353-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5353-158">Boolean</span></span>|<span data-ttu-id="e5353-159">Извлечение Хардварехаш для профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e5353-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e5353-160">девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="e5353-160">deviceNameTemplate</span></span>|<span data-ttu-id="e5353-161">String</span><span class="sxs-lookup"><span data-stu-id="e5353-161">String</span></span>|<span data-ttu-id="e5353-162">Шаблон, используемый для именования автопилотного устройства.</span><span class="sxs-lookup"><span data-stu-id="e5353-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="e5353-163">Это может быть настраиваемый текст, который также может содержать серийный номер устройства или случайное число.</span><span class="sxs-lookup"><span data-stu-id="e5353-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="e5353-164">Общая длина текста, созданного шаблоном, не может превышать 15 символов.</span><span class="sxs-lookup"><span data-stu-id="e5353-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="e5353-165">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e5353-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e5353-166">deviceType</span><span class="sxs-lookup"><span data-stu-id="e5353-166">deviceType</span></span>|[<span data-ttu-id="e5353-167">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="e5353-167">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="e5353-168">Тип устройства автопилота, к которому применяется этот профиль.</span><span class="sxs-lookup"><span data-stu-id="e5353-168">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="e5353-169">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="e5353-169">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="e5353-170">Возможные значения: `windowsPc`, `surfaceHub2`, `holoLens`.</span><span class="sxs-lookup"><span data-stu-id="e5353-170">Possible values are: `windowsPc`, `surfaceHub2`, `holoLens`.</span></span>|
|<span data-ttu-id="e5353-171">енаблевхитеглове</span><span class="sxs-lookup"><span data-stu-id="e5353-171">enableWhiteGlove</span></span>|<span data-ttu-id="e5353-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5353-172">Boolean</span></span>|<span data-ttu-id="e5353-173">Включите для профиля белый Глове для автопилотного развертывания.</span><span class="sxs-lookup"><span data-stu-id="e5353-173">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="e5353-174">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e5353-174">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e5353-175">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e5353-175">roleScopeTagIds</span></span>|<span data-ttu-id="e5353-176">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="e5353-176">String collection</span></span>|<span data-ttu-id="e5353-177">Теги областей для профиля.</span><span class="sxs-lookup"><span data-stu-id="e5353-177">Scope tags for the profile.</span></span> <span data-ttu-id="e5353-178">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e5353-178">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="e5353-179">хибридазуреаджоинскипконнективитичекк</span><span class="sxs-lookup"><span data-stu-id="e5353-179">hybridAzureADJoinSkipConnectivityCheck</span></span>|<span data-ttu-id="e5353-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5353-180">Boolean</span></span>|<span data-ttu-id="e5353-181">Процесс самопилотного подключения к гибридной среде Azure AD продолжится даже в том случае, если он не устанавливает подключение к контроллеру домена во время OOBE.</span><span class="sxs-lookup"><span data-stu-id="e5353-181">The Autopilot Hybrid Azure AD join flow will continue even if it does not establish domain controller connectivity during OOBE.</span></span>|



## <a name="response"></a><span data-ttu-id="e5353-182">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5353-182">Response</span></span>
<span data-ttu-id="e5353-183">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5353-183">If successful, this method returns a `201 Created` response code and a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5353-184">Пример</span><span class="sxs-lookup"><span data-stu-id="e5353-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5353-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5353-185">Request</span></span>
<span data-ttu-id="e5353-186">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5353-186">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e5353-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5353-187">Response</span></span>
<span data-ttu-id="e5353-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5353-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



