---
title: Обновление Активедиректоривиндовсаутопилотдеплойментпрофиле
description: Обновление свойств объекта Активедиректоривиндовсаутопилотдеплойментпрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e76fc466195989c82728bf1bba972e876c9ef186
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160062"
---
# <a name="update-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="723b5-103">Обновление Активедиректоривиндовсаутопилотдеплойментпрофиле</span><span class="sxs-lookup"><span data-stu-id="723b5-103">Update activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="723b5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="723b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="723b5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="723b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="723b5-106">Обновление свойств объекта [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="723b5-106">Update the properties of a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="723b5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="723b5-107">Prerequisites</span></span>
<span data-ttu-id="723b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="723b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="723b5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="723b5-110">Permission type</span></span>|<span data-ttu-id="723b5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="723b5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="723b5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="723b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="723b5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="723b5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="723b5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="723b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="723b5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="723b5-115">Not supported.</span></span>|
|<span data-ttu-id="723b5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="723b5-116">Application</span></span>|<span data-ttu-id="723b5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="723b5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="723b5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="723b5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="request-headers"></a><span data-ttu-id="723b5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="723b5-119">Request headers</span></span>
|<span data-ttu-id="723b5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="723b5-120">Header</span></span>|<span data-ttu-id="723b5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="723b5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="723b5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="723b5-122">Authorization</span></span>|<span data-ttu-id="723b5-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="723b5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="723b5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="723b5-124">Accept</span></span>|<span data-ttu-id="723b5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="723b5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="723b5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="723b5-126">Request body</span></span>
<span data-ttu-id="723b5-127">В тексте запроса добавьте представление объекта [Активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="723b5-127">In the request body, supply a JSON representation for the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

<span data-ttu-id="723b5-128">В следующей таблице приведены свойства, необходимые при создании [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="723b5-128">The following table shows the properties that are required when you create the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md).</span></span>

|<span data-ttu-id="723b5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="723b5-129">Property</span></span>|<span data-ttu-id="723b5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="723b5-130">Type</span></span>|<span data-ttu-id="723b5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="723b5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="723b5-132">id</span><span class="sxs-lookup"><span data-stu-id="723b5-132">id</span></span>|<span data-ttu-id="723b5-133">String</span><span class="sxs-lookup"><span data-stu-id="723b5-133">String</span></span>|<span data-ttu-id="723b5-134">Ключ профиля, наСледуемый от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="723b5-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="723b5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="723b5-135">displayName</span></span>|<span data-ttu-id="723b5-136">String</span><span class="sxs-lookup"><span data-stu-id="723b5-136">String</span></span>|<span data-ttu-id="723b5-137">Имя профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="723b5-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="723b5-138">description</span><span class="sxs-lookup"><span data-stu-id="723b5-138">description</span></span>|<span data-ttu-id="723b5-139">Строка</span><span class="sxs-lookup"><span data-stu-id="723b5-139">String</span></span>|<span data-ttu-id="723b5-140">Описание профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="723b5-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="723b5-141">language</span><span class="sxs-lookup"><span data-stu-id="723b5-141">language</span></span>|<span data-ttu-id="723b5-142">String</span><span class="sxs-lookup"><span data-stu-id="723b5-142">String</span></span>|<span data-ttu-id="723b5-143">Язык, настроенный на устройстве, унаследованном от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="723b5-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="723b5-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="723b5-144">createdDateTime</span></span>|<span data-ttu-id="723b5-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="723b5-145">DateTimeOffset</span></span>|<span data-ttu-id="723b5-146">Время создания профиля, унаследованное от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="723b5-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="723b5-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="723b5-147">lastModifiedDateTime</span></span>|<span data-ttu-id="723b5-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="723b5-148">DateTimeOffset</span></span>|<span data-ttu-id="723b5-149">Время последнего изменения профиля, наСледуемого от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="723b5-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="723b5-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="723b5-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="723b5-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="723b5-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="723b5-152">Настройка "от" в рамке наСледуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="723b5-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="723b5-153">Енроллментстатусскринсеттингс</span><span class="sxs-lookup"><span data-stu-id="723b5-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="723b5-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="723b5-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="723b5-155">Параметр экрана состояния регистрации, наСледуемый от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="723b5-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="723b5-156">Екстраксардварехаш</span><span class="sxs-lookup"><span data-stu-id="723b5-156">extractHardwareHash</span></span>|<span data-ttu-id="723b5-157">Логический</span><span class="sxs-lookup"><span data-stu-id="723b5-157">Boolean</span></span>|<span data-ttu-id="723b5-158">Извлечение Хардварехаш для профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="723b5-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="723b5-159">Девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="723b5-159">deviceNameTemplate</span></span>|<span data-ttu-id="723b5-160">String</span><span class="sxs-lookup"><span data-stu-id="723b5-160">String</span></span>|<span data-ttu-id="723b5-161">Шаблон, используемый для именования автоПилотного устройства.</span><span class="sxs-lookup"><span data-stu-id="723b5-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="723b5-162">Это может быть настраиваемый текст, который также может содержать серийный номер устройства или случайное число.</span><span class="sxs-lookup"><span data-stu-id="723b5-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="723b5-163">Общая длина текста, созданного шаблоном, не может превышать 15 символов.</span><span class="sxs-lookup"><span data-stu-id="723b5-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="723b5-164">НаСледуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="723b5-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="723b5-165">Енаблевхитеглове</span><span class="sxs-lookup"><span data-stu-id="723b5-165">enableWhiteGlove</span></span>|<span data-ttu-id="723b5-166">Логический</span><span class="sxs-lookup"><span data-stu-id="723b5-166">Boolean</span></span>|<span data-ttu-id="723b5-167">Включите для профиля белый Глове для автопилотного развертывания.</span><span class="sxs-lookup"><span data-stu-id="723b5-167">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="723b5-168">НаСледуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="723b5-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="723b5-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="723b5-169">Response</span></span>
<span data-ttu-id="723b5-170">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="723b5-170">If successful, this method returns a `200 OK` response code and an updated [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="723b5-171">Пример</span><span class="sxs-lookup"><span data-stu-id="723b5-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="723b5-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="723b5-172">Request</span></span>
<span data-ttu-id="723b5-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="723b5-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
Content-type: application/json
Content-length: 1073

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
  "enableWhiteGlove": true
}
```

### <a name="response"></a><span data-ttu-id="723b5-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="723b5-174">Response</span></span>
<span data-ttu-id="723b5-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="723b5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1245

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
  "enableWhiteGlove": true
}
```




