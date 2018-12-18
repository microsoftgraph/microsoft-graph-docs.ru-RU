---
title: Создание activeDirectoryWindowsAutopilotDeploymentProfile
description: Создание нового объекта activeDirectoryWindowsAutopilotDeploymentProfile.
author: tfitzmac
ms.openlocfilehash: 50959427a9634d2b8376cece9c3c33c908c69365
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324089"
---
# <a name="create-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="c5b1e-103">Создание activeDirectoryWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="c5b1e-103">Create activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="c5b1e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5b1e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5b1e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5b1e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5b1e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c5b1e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5b1e-107">Создание нового объекта [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c5b1e-107">Create a new [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c5b1e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c5b1e-108">Prerequisites</span></span>
<span data-ttu-id="c5b1e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5b1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5b1e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5b1e-111">Permission type</span></span>|<span data-ttu-id="c5b1e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5b1e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5b1e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5b1e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5b1e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5b1e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c5b1e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5b1e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5b1e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5b1e-116">Not supported.</span></span>|
|<span data-ttu-id="c5b1e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5b1e-117">Application</span></span>|<span data-ttu-id="c5b1e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5b1e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5b1e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5b1e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="c5b1e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5b1e-120">Request headers</span></span>
|<span data-ttu-id="c5b1e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5b1e-121">Header</span></span>|<span data-ttu-id="c5b1e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c5b1e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5b1e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5b1e-123">Authorization</span></span>|<span data-ttu-id="c5b1e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c5b1e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5b1e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c5b1e-125">Accept</span></span>|<span data-ttu-id="c5b1e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5b1e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5b1e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5b1e-127">Request body</span></span>
<span data-ttu-id="c5b1e-128">В тексте запроса укажите представление JSON для объекта activeDirectoryWindowsAutopilotDeploymentProfile.</span><span class="sxs-lookup"><span data-stu-id="c5b1e-128">In the request body, supply a JSON representation for the activeDirectoryWindowsAutopilotDeploymentProfile object.</span></span>

<span data-ttu-id="c5b1e-129">В следующей таблице показаны свойства, которые необходимы для создания activeDirectoryWindowsAutopilotDeploymentProfile.</span><span class="sxs-lookup"><span data-stu-id="c5b1e-129">The following table shows the properties that are required when you create the activeDirectoryWindowsAutopilotDeploymentProfile.</span></span>

|<span data-ttu-id="c5b1e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5b1e-130">Property</span></span>|<span data-ttu-id="c5b1e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c5b1e-131">Type</span></span>|<span data-ttu-id="c5b1e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c5b1e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5b1e-133">id</span><span class="sxs-lookup"><span data-stu-id="c5b1e-133">id</span></span>|<span data-ttu-id="c5b1e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c5b1e-134">String</span></span>|<span data-ttu-id="c5b1e-135">Профиль ключ наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c5b1e-135">Profile Key Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c5b1e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c5b1e-136">displayName</span></span>|<span data-ttu-id="c5b1e-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c5b1e-137">String</span></span>|<span data-ttu-id="c5b1e-138">Имя профиля, унаследованные от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c5b1e-138">Name of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c5b1e-139">описание</span><span class="sxs-lookup"><span data-stu-id="c5b1e-139">description</span></span>|<span data-ttu-id="c5b1e-140">Строка</span><span class="sxs-lookup"><span data-stu-id="c5b1e-140">String</span></span>|<span data-ttu-id="c5b1e-141">Описание профиля унаследованные от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c5b1e-141">Description of the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c5b1e-142">language</span><span class="sxs-lookup"><span data-stu-id="c5b1e-142">language</span></span>|<span data-ttu-id="c5b1e-143">String</span><span class="sxs-lookup"><span data-stu-id="c5b1e-143">String</span></span>|<span data-ttu-id="c5b1e-144">Язык, настроенных на устройстве унаследованные от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c5b1e-144">Language configured on the device Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c5b1e-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5b1e-145">createdDateTime</span></span>|<span data-ttu-id="c5b1e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5b1e-146">DateTimeOffset</span></span>|<span data-ttu-id="c5b1e-147">Время создания профилей унаследованные от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c5b1e-147">Profile creation time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c5b1e-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5b1e-148">lastModifiedDateTime</span></span>|<span data-ttu-id="c5b1e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5b1e-149">DateTimeOffset</span></span>|<span data-ttu-id="c5b1e-150">Профиль последнего изменения время унаследованные от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c5b1e-150">Profile last modified time Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c5b1e-151">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="c5b1e-151">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="c5b1e-152">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="c5b1e-152">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="c5b1e-153">В соответствующем взаимодействия параметру унаследованные от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c5b1e-153">Out of box experience setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c5b1e-154">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="c5b1e-154">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="c5b1e-155">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="c5b1e-155">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="c5b1e-156">Установка унаследованные от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) экрана состояния подачи заявок</span><span class="sxs-lookup"><span data-stu-id="c5b1e-156">Enrollment status screen setting Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c5b1e-157">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="c5b1e-157">extractHardwareHash</span></span>|<span data-ttu-id="c5b1e-158">Boolean.</span><span class="sxs-lookup"><span data-stu-id="c5b1e-158">Boolean</span></span>|<span data-ttu-id="c5b1e-159">Извлечение HardwareHash для профиля унаследованные от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c5b1e-159">HardwareHash Extraction for the profile Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|
|<span data-ttu-id="c5b1e-160">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="c5b1e-160">deviceNameTemplate</span></span>|<span data-ttu-id="c5b1e-161">String.</span><span class="sxs-lookup"><span data-stu-id="c5b1e-161">String</span></span>|<span data-ttu-id="c5b1e-162">Шаблон, используемый для имя устройства автопилот.</span><span class="sxs-lookup"><span data-stu-id="c5b1e-162">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="c5b1e-163">Это может быть настраиваемого текста, а также может содержать серийный номер устройства или случайное число.</span><span class="sxs-lookup"><span data-stu-id="c5b1e-163">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="c5b1e-164">Общая длина текста, созданной с помощью шаблона может быть не более 15 символов.</span><span class="sxs-lookup"><span data-stu-id="c5b1e-164">The total length of the text generated by the template can be no more than 15 characters.</span></span> <span data-ttu-id="c5b1e-165">Наследуется от [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c5b1e-165">Inherited from [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c5b1e-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5b1e-166">Response</span></span>
<span data-ttu-id="c5b1e-167">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c5b1e-167">If successful, this method returns a `201 Created` response code and a [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5b1e-168">Пример</span><span class="sxs-lookup"><span data-stu-id="c5b1e-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="c5b1e-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5b1e-169">Request</span></span>
<span data-ttu-id="c5b1e-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5b1e-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
Content-type: application/json
Content-length: 1108

{
  "@odata.type": "#microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "language": "Language value",
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

### <a name="response"></a><span data-ttu-id="c5b1e-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5b1e-171">Response</span></span>
<span data-ttu-id="c5b1e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c5b1e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1216

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
  "deviceNameTemplate": "Device Name Template value"
}
```





