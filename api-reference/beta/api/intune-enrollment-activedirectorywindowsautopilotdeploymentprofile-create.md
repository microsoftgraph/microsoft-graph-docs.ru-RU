---
title: Создание Активедиректоривиндовсаутопилотдеплойментпрофиле
description: Создание нового объекта Активедиректоривиндовсаутопилотдеплойментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1ce952d6f84f9666a46820821c071622e096d51e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978327"
---
# <a name="create-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="12c4b-103">Создание Активедиректоривиндовсаутопилотдеплойментпрофиле</span><span class="sxs-lookup"><span data-stu-id="12c4b-103">Create activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="12c4b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12c4b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12c4b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12c4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12c4b-106">Создание нового объекта [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="12c4b-106">Create a new [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12c4b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="12c4b-107">Prerequisites</span></span>
<span data-ttu-id="12c4b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12c4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12c4b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12c4b-110">Permission type</span></span>|<span data-ttu-id="12c4b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12c4b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12c4b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12c4b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12c4b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12c4b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="12c4b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12c4b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12c4b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12c4b-115">Not supported.</span></span>|
|<span data-ttu-id="12c4b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12c4b-116">Application</span></span>|<span data-ttu-id="12c4b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12c4b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12c4b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12c4b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="12c4b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12c4b-119">Request headers</span></span>
|<span data-ttu-id="12c4b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12c4b-120">Header</span></span>|<span data-ttu-id="12c4b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="12c4b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12c4b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12c4b-122">Authorization</span></span>|<span data-ttu-id="12c4b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12c4b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12c4b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="12c4b-124">Accept</span></span>|<span data-ttu-id="12c4b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12c4b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12c4b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="12c4b-126">Request body</span></span>
<span data-ttu-id="12c4b-127">В тексте запроса добавьте представление объекта Активедиректоривиндовсаутопилотдеплойментпрофиле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12c4b-127">In the request body, supply a JSON representation for the activeDirectoryWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="12c4b-128">В следующей таблице приведены свойства, необходимые при создании Активедиректоривиндовсаутопилотдеплойментпрофиле.</span><span class="sxs-lookup"><span data-stu-id="12c4b-128">The following table shows the properties that are required when you create the activeDirectoryWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="12c4b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="12c4b-129">Property</span></span>|<span data-ttu-id="12c4b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="12c4b-130">Type</span></span>|<span data-ttu-id="12c4b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="12c4b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12c4b-132">id</span><span class="sxs-lookup"><span data-stu-id="12c4b-132">id</span></span>|<span data-ttu-id="12c4b-133">Строка</span><span class="sxs-lookup"><span data-stu-id="12c4b-133">String</span></span>|<span data-ttu-id="12c4b-134">Ключ профиля, наследуемый от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="12c4b-134">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="12c4b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="12c4b-135">displayName</span></span>|<span data-ttu-id="12c4b-136">Строка</span><span class="sxs-lookup"><span data-stu-id="12c4b-136">String</span></span>|<span data-ttu-id="12c4b-137">Имя профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="12c4b-137">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="12c4b-138">description</span><span class="sxs-lookup"><span data-stu-id="12c4b-138">description</span></span>|<span data-ttu-id="12c4b-139">String</span><span class="sxs-lookup"><span data-stu-id="12c4b-139">String</span></span>|<span data-ttu-id="12c4b-140">Описание профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="12c4b-140">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="12c4b-141">language</span><span class="sxs-lookup"><span data-stu-id="12c4b-141">language</span></span>|<span data-ttu-id="12c4b-142">String</span><span class="sxs-lookup"><span data-stu-id="12c4b-142">String</span></span>|<span data-ttu-id="12c4b-143">Язык, настроенный на устройстве, унаследованном от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="12c4b-143">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="12c4b-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12c4b-144">createdDateTime</span></span>|<span data-ttu-id="12c4b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12c4b-145">DateTimeOffset</span></span>|<span data-ttu-id="12c4b-146">Время создания профиля, унаследованное от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="12c4b-146">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="12c4b-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12c4b-147">lastModifiedDateTime</span></span>|<span data-ttu-id="12c4b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12c4b-148">DateTimeOffset</span></span>|<span data-ttu-id="12c4b-149">Время последнего изменения профиля, наследуемого от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="12c4b-149">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="12c4b-150">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="12c4b-150">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="12c4b-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="12c4b-151">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="12c4b-152">Настройка "от" в рамке наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="12c4b-152">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="12c4b-153">Енроллментстатусскринсеттингс</span><span class="sxs-lookup"><span data-stu-id="12c4b-153">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="12c4b-154">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="12c4b-154">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="12c4b-155">Параметр экрана состояния регистрации, наследуемый от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="12c4b-155">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="12c4b-156">Екстраксардварехаш</span><span class="sxs-lookup"><span data-stu-id="12c4b-156">extractHardwareHash</span></span>|<span data-ttu-id="12c4b-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="12c4b-157">Boolean</span></span>|<span data-ttu-id="12c4b-158">Извлечение Хардварехаш для профиля, унаследованного от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="12c4b-158">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="12c4b-159">Девиценаметемплате</span><span class="sxs-lookup"><span data-stu-id="12c4b-159">deviceNameTemplate</span></span>|<span data-ttu-id="12c4b-160">String</span><span class="sxs-lookup"><span data-stu-id="12c4b-160">String</span></span>|<span data-ttu-id="12c4b-161">Шаблон, используемый для именования автопилотного устройства.</span><span class="sxs-lookup"><span data-stu-id="12c4b-161">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="12c4b-162">Это может быть настраиваемый текст, который также может содержать серийный номер устройства или случайное число.</span><span class="sxs-lookup"><span data-stu-id="12c4b-162">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="12c4b-163">Общая длина текста, созданного шаблоном, не может превышать 15 символов.</span><span class="sxs-lookup"><span data-stu-id="12c4b-163">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="12c4b-164">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="12c4b-164">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="12c4b-165">deviceType</span><span class="sxs-lookup"><span data-stu-id="12c4b-165">deviceType</span></span>|[<span data-ttu-id="12c4b-166">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="12c4b-166">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="12c4b-167">Тип устройства автопилота, к которому применяется этот профиль.</span><span class="sxs-lookup"><span data-stu-id="12c4b-167">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="12c4b-168">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="12c4b-168">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md).</span></span> <span data-ttu-id="12c4b-169">Возможные значения: `windowsPc`, `surfaceHub2`.</span><span class="sxs-lookup"><span data-stu-id="12c4b-169">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="12c4b-170">Енаблевхитеглове</span><span class="sxs-lookup"><span data-stu-id="12c4b-170">enableWhiteGlove</span></span>|<span data-ttu-id="12c4b-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="12c4b-171">Boolean</span></span>|<span data-ttu-id="12c4b-172">Включите для профиля белый Глове для автопилотного развертывания.</span><span class="sxs-lookup"><span data-stu-id="12c4b-172">Enable Autopilot White Glove for the profile.</span></span> <span data-ttu-id="12c4b-173">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="12c4b-173">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="12c4b-174">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="12c4b-174">roleScopeTagIds</span></span>|<span data-ttu-id="12c4b-175">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="12c4b-175">String collection</span></span>|<span data-ttu-id="12c4b-176">Теги областей для профиля.</span><span class="sxs-lookup"><span data-stu-id="12c4b-176">Scope tags for the profile.</span></span> <span data-ttu-id="12c4b-177">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="12c4b-177">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="12c4b-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="12c4b-178">Response</span></span>
<span data-ttu-id="12c4b-179">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="12c4b-179">If successful, this method returns a `201 Created` response code and a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12c4b-180">Пример</span><span class="sxs-lookup"><span data-stu-id="12c4b-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="12c4b-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="12c4b-181">Request</span></span>
<span data-ttu-id="12c4b-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12c4b-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
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

### <a name="response"></a><span data-ttu-id="12c4b-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="12c4b-183">Response</span></span>
<span data-ttu-id="12c4b-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12c4b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





