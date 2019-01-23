---
title: Создание azureADWindowsAutopilotDeploymentProfile
description: Создание нового объекта azureADWindowsAutopilotDeploymentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62b73c9041477a5aa103e08ce952c5d713bed83b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398830"
---
# <a name="create-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="f4d00-103">Создание azureADWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="f4d00-103">Create azureADWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="f4d00-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f4d00-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f4d00-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4d00-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4d00-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4d00-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4d00-107">Создание нового объекта [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f4d00-107">Create a new [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4d00-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="f4d00-108">Prerequisites</span></span>
<span data-ttu-id="f4d00-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f4d00-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f4d00-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4d00-111">Permission type</span></span>|<span data-ttu-id="f4d00-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4d00-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4d00-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4d00-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4d00-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4d00-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f4d00-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4d00-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4d00-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4d00-116">Not supported.</span></span>|
|<span data-ttu-id="f4d00-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4d00-117">Application</span></span>|<span data-ttu-id="f4d00-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4d00-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4d00-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4d00-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="f4d00-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4d00-120">Request headers</span></span>
|<span data-ttu-id="f4d00-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4d00-121">Header</span></span>|<span data-ttu-id="f4d00-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f4d00-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4d00-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4d00-123">Authorization</span></span>|<span data-ttu-id="f4d00-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f4d00-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4d00-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f4d00-125">Accept</span></span>|<span data-ttu-id="f4d00-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4d00-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4d00-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4d00-127">Request body</span></span>
<span data-ttu-id="f4d00-128">В тексте запроса укажите представление JSON для объекта azureADWindowsAutopilotDeploymentProfile.</span><span class="sxs-lookup"><span data-stu-id="f4d00-128">In the request body, supply a JSON representation for the azureADWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="f4d00-129">В следующей таблице показаны свойства, которые необходимы для создания azureADWindowsAutopilotDeploymentProfile.</span><span class="sxs-lookup"><span data-stu-id="f4d00-129">The following table shows the properties that are required when you create the azureADWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="f4d00-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4d00-130">Property</span></span>|<span data-ttu-id="f4d00-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f4d00-131">Type</span></span>|<span data-ttu-id="f4d00-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f4d00-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4d00-133">id</span><span class="sxs-lookup"><span data-stu-id="f4d00-133">id</span></span>|<span data-ttu-id="f4d00-134">String</span><span class="sxs-lookup"><span data-stu-id="f4d00-134">String</span></span>|<span data-ttu-id="f4d00-135">Профиль ключ наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d00-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4d00-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f4d00-136">displayName</span></span>|<span data-ttu-id="f4d00-137">String</span><span class="sxs-lookup"><span data-stu-id="f4d00-137">String</span></span>|<span data-ttu-id="f4d00-138">Имя профиля, унаследованные от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d00-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4d00-139">description</span><span class="sxs-lookup"><span data-stu-id="f4d00-139">description</span></span>|<span data-ttu-id="f4d00-140">String</span><span class="sxs-lookup"><span data-stu-id="f4d00-140">String</span></span>|<span data-ttu-id="f4d00-141">Описание профиля унаследованные от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d00-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4d00-142">language</span><span class="sxs-lookup"><span data-stu-id="f4d00-142">language</span></span>|<span data-ttu-id="f4d00-143">String</span><span class="sxs-lookup"><span data-stu-id="f4d00-143">String</span></span>|<span data-ttu-id="f4d00-144">Язык, настроенных на устройстве унаследованные от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d00-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4d00-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4d00-145">createdDateTime</span></span>|<span data-ttu-id="f4d00-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4d00-146">DateTimeOffset</span></span>|<span data-ttu-id="f4d00-147">Время создания профилей унаследованные от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d00-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4d00-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4d00-148">lastModifiedDateTime</span></span>|<span data-ttu-id="f4d00-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4d00-149">DateTimeOffset</span></span>|<span data-ttu-id="f4d00-150">Профиль последнего изменения время унаследованные от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d00-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4d00-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="f4d00-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="f4d00-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="f4d00-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="f4d00-153">В соответствующем взаимодействия параметру унаследованные от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d00-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4d00-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="f4d00-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="f4d00-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="f4d00-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="f4d00-156">Установка унаследованные от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) экрана состояния подачи заявок</span><span class="sxs-lookup"><span data-stu-id="f4d00-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4d00-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="f4d00-157">extractHardwareHash</span></span>|<span data-ttu-id="f4d00-158">Логический</span><span class="sxs-lookup"><span data-stu-id="f4d00-158">Boolean</span></span>|<span data-ttu-id="f4d00-159">Извлечение HardwareHash для профиля унаследованные от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d00-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="f4d00-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="f4d00-160">deviceNameTemplate</span></span>|<span data-ttu-id="f4d00-161">String</span><span class="sxs-lookup"><span data-stu-id="f4d00-161">String</span></span>|<span data-ttu-id="f4d00-162">Шаблон, используемый для имя устройства автопилот.</span><span class="sxs-lookup"><span data-stu-id="f4d00-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="f4d00-163">Это может быть настраиваемого текста, а также может содержать серийный номер устройства или случайное число.</span><span class="sxs-lookup"><span data-stu-id="f4d00-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="f4d00-164">Общая длина текста, созданной с помощью шаблона может быть не более 15 символов.</span><span class="sxs-lookup"><span data-stu-id="f4d00-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="f4d00-165">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f4d00-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f4d00-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4d00-166">Response</span></span>
<span data-ttu-id="f4d00-167">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f4d00-167">If successful, this method returns a `201 Created` response code and a [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4d00-168">Пример</span><span class="sxs-lookup"><span data-stu-id="f4d00-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4d00-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4d00-169">Request</span></span>
<span data-ttu-id="f4d00-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4d00-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
Content-type: application/json
Content-length: 1036

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
  "deviceNameTemplate": "Device Name Template value"
}
```

### <a name="response"></a><span data-ttu-id="f4d00-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4d00-171">Response</span></span>
<span data-ttu-id="f4d00-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f4d00-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1208

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
  "deviceNameTemplate": "Device Name Template value"
}
```




