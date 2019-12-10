---
title: Получение windowsAutopilotDeploymentProfile
description: Чтение свойств и связей объекта windowsAutopilotDeploymentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4fb3564e3cb20a88ef56d23b63c48524f2d40757
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939404"
---
# <a name="get-windowsautopilotdeploymentprofile"></a><span data-ttu-id="322d6-103">Получение windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="322d6-103">Get windowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="322d6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="322d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="322d6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="322d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="322d6-106">Чтение свойств и связей объекта [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="322d6-106">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="322d6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="322d6-107">Prerequisites</span></span>
<span data-ttu-id="322d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="322d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="322d6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="322d6-110">Permission type</span></span>|<span data-ttu-id="322d6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="322d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="322d6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="322d6-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="322d6-113">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="322d6-113">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="322d6-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="322d6-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="322d6-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="322d6-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="322d6-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="322d6-116">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="322d6-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="322d6-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="322d6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="322d6-118">Not supported.</span></span>|
|<span data-ttu-id="322d6-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="322d6-119">Application</span></span>||
| <span data-ttu-id="322d6-120">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="322d6-120">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="322d6-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="322d6-121">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="322d6-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="322d6-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="322d6-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="322d6-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="322d6-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="322d6-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="322d6-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="322d6-125">Optional query parameters</span></span>
<span data-ttu-id="322d6-126">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="322d6-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="322d6-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="322d6-127">Request headers</span></span>
|<span data-ttu-id="322d6-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="322d6-128">Header</span></span>|<span data-ttu-id="322d6-129">Значение</span><span class="sxs-lookup"><span data-stu-id="322d6-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="322d6-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="322d6-130">Authorization</span></span>|<span data-ttu-id="322d6-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="322d6-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="322d6-132">Accept</span><span class="sxs-lookup"><span data-stu-id="322d6-132">Accept</span></span>|<span data-ttu-id="322d6-133">application/json</span><span class="sxs-lookup"><span data-stu-id="322d6-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="322d6-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="322d6-134">Request body</span></span>
<span data-ttu-id="322d6-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="322d6-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="322d6-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="322d6-136">Response</span></span>
<span data-ttu-id="322d6-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="322d6-137">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="322d6-138">Пример</span><span class="sxs-lookup"><span data-stu-id="322d6-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="322d6-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="322d6-139">Request</span></span>
<span data-ttu-id="322d6-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="322d6-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="322d6-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="322d6-141">Response</span></span>
<span data-ttu-id="322d6-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="322d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1409

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfile",
    "id": "9d6394a9-94a9-9d63-a994-639da994639d",
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
}
```








