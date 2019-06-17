---
title: Обновление Активедиректоривиндовсаутопилотдеплойментпрофиле
description: Обновление свойств объекта Активедиректоривиндовсаутопилотдеплойментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b2a45e0fa86e54aef6e42503866d19fc3d6a90c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979146"
---
# <a name="update-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="f4074-103">Обновление Активедиректоривиндовсаутопилотдеплойментпрофиле</span><span class="sxs-lookup"><span data-stu-id="f4074-103">Update activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="f4074-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4074-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4074-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4074-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4074-106">Обновление свойств объекта [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f4074-106">Update the properties of a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4074-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f4074-107">Prerequisites</span></span>
<span data-ttu-id="f4074-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4074-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4074-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4074-110">Permission type</span></span>|<span data-ttu-id="f4074-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4074-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4074-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4074-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4074-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4074-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f4074-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4074-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4074-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4074-115">Not supported.</span></span>|
|<span data-ttu-id="f4074-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4074-116">Application</span></span>|<span data-ttu-id="f4074-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4074-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4074-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4074-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="f4074-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4074-119">Request headers</span></span>
|<span data-ttu-id="f4074-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4074-120">Header</span></span>|<span data-ttu-id="f4074-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f4074-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4074-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4074-122">Authorization</span></span>|<span data-ttu-id="f4074-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4074-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4074-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f4074-124">Accept</span></span>|<span data-ttu-id="f4074-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4074-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4074-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f4074-126">Request body</span></span>
<span data-ttu-id="f4074-127">В тексте запроса добавьте представление объекта [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4074-127">In the request body, supply a JSON representation for the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="f4074-128">В следующей таблице приведены свойства, необходимые при создании [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f4074-128">The following table shows the properties that are required when you create the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="f4074-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4074-129">Property</span></span>|<span data-ttu-id="f4074-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f4074-130">Type</span></span>|<span data-ttu-id="f4074-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f4074-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4074-132">id</span><span class="sxs-lookup"><span data-stu-id="f4074-132">id</span></span>|<span data-ttu-id="f4074-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f4074-133">String</span></span>|<span data-ttu-id="f4074-134">Ключ профиля, наследуемый от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4074-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4074-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f4074-135">displayName</span></span>|<span data-ttu-id="f4074-136">Строка</span><span class="sxs-lookup"><span data-stu-id="f4074-136">String</span></span>|<span data-ttu-id="f4074-137">Имя профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4074-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4074-138">description</span><span class="sxs-lookup"><span data-stu-id="f4074-138">description</span></span>|<span data-ttu-id="f4074-139">String</span><span class="sxs-lookup"><span data-stu-id="f4074-139">String</span></span>|<span data-ttu-id="f4074-140">Описание профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4074-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4074-141">language</span><span class="sxs-lookup"><span data-stu-id="f4074-141">language</span></span>|<span data-ttu-id="f4074-142">String</span><span class="sxs-lookup"><span data-stu-id="f4074-142">String</span></span>|<span data-ttu-id="f4074-143">Язык, настроенный на устройстве, унаследованном от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4074-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4074-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4074-144">createdDateTime</span></span>|<span data-ttu-id="f4074-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4074-145">DateTimeOffset</span></span>|<span data-ttu-id="f4074-146">Время создания профиля, унаследованное от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4074-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4074-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4074-147">lastModifiedDateTime</span></span>|<span data-ttu-id="f4074-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4074-148">DateTimeOffset</span></span>|<span data-ttu-id="f4074-149">Время последнего изменения профиля, наследуемого от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4074-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4074-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="f4074-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="f4074-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="f4074-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="f4074-152">Настройка "от" в рамке наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4074-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4074-153">Енроллментстатусскринсеттингс</span><span class="sxs-lookup"><span data-stu-id="f4074-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="f4074-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="f4074-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="f4074-155">Параметр экрана состояния регистрации, наследуемый от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4074-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4074-156">Екстраксардварехаш</span><span class="sxs-lookup"><span data-stu-id="f4074-156">extractHardwareHash</span></span>|<span data-ttu-id="f4074-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4074-157">Boolean</span></span>|<span data-ttu-id="f4074-158">Извлечение Хардварехаш для профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4074-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4074-159">Девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="f4074-159">deviceNameTemplate</span></span>|<span data-ttu-id="f4074-160">String</span><span class="sxs-lookup"><span data-stu-id="f4074-160">String</span></span>|<span data-ttu-id="f4074-161">Шаблон, используемый для именования автопилотного устройства.</span><span class="sxs-lookup"><span data-stu-id="f4074-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="f4074-162">Это может быть настраиваемый текст, который также может содержать серийный номер устройства или случайное число.</span><span class="sxs-lookup"><span data-stu-id="f4074-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="f4074-163">Общая длина текста, созданного шаблоном, не может превышать 15 символов.</span><span class="sxs-lookup"><span data-stu-id="f4074-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="f4074-164">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4074-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4074-165">deviceType</span><span class="sxs-lookup"><span data-stu-id="f4074-165">deviceType</span></span>|[<span data-ttu-id="f4074-166">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="f4074-166">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="f4074-167">Тип устройства автопилота, к которому применяется этот профиль.</span><span class="sxs-lookup"><span data-stu-id="f4074-167">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="f4074-168">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f4074-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="f4074-169">Возможные значения: `windowsPc`, `surfaceHub2`.</span><span class="sxs-lookup"><span data-stu-id="f4074-169">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="f4074-170">Енаблевхитеглове</span><span class="sxs-lookup"><span data-stu-id="f4074-170">enableWhiteGlove</span></span>|<span data-ttu-id="f4074-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4074-171">Boolean</span></span>|<span data-ttu-id="f4074-172">Включите для профиля белый Глове для автопилотного развертывания.</span><span class="sxs-lookup"><span data-stu-id="f4074-172">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="f4074-173">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4074-173">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4074-174">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f4074-174">roleScopeTagIds</span></span>|<span data-ttu-id="f4074-175">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f4074-175">String collection</span></span>|<span data-ttu-id="f4074-176">Теги областей для профиля.</span><span class="sxs-lookup"><span data-stu-id="f4074-176">Scope tags for the profile.</span></span> <span data-ttu-id="f4074-177">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4074-177">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f4074-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4074-178">Response</span></span>
<span data-ttu-id="f4074-179">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f4074-179">If successful, this method returns a `200 OK` response code and an updated [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4074-180">Пример</span><span class="sxs-lookup"><span data-stu-id="f4074-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4074-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4074-181">Request</span></span>
<span data-ttu-id="f4074-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4074-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4074-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4074-183">Response</span></span>
<span data-ttu-id="f4074-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4074-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





