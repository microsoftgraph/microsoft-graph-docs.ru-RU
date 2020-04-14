---
title: Получение Активедиректоривиндовсаутопилотдеплойментпрофиле
description: Чтение свойств и связей объекта Активедиректоривиндовсаутопилотдеплойментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fcb0f41f13c3daed54ffc5d0f7382e4dc29ed572
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43378019"
---
# <a name="get-activedirectorywindowsautopilotdeploymentprofile"></a><span data-ttu-id="6bab9-103">Получение Активедиректоривиндовсаутопилотдеплойментпрофиле</span><span class="sxs-lookup"><span data-stu-id="6bab9-103">Get activeDirectoryWindowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="6bab9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bab9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6bab9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bab9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bab9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6bab9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bab9-107">Чтение свойств и связей объекта [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6bab9-107">Read properties and relationships of the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6bab9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6bab9-108">Prerequisites</span></span>
<span data-ttu-id="6bab9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bab9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bab9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6bab9-111">Permission type</span></span>|<span data-ttu-id="6bab9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6bab9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bab9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6bab9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6bab9-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bab9-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6bab9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6bab9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bab9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bab9-116">Not supported.</span></span>|
|<span data-ttu-id="6bab9-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6bab9-117">Application</span></span>|<span data-ttu-id="6bab9-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6bab9-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bab9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6bab9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6bab9-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6bab9-120">Optional query parameters</span></span>
<span data-ttu-id="6bab9-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6bab9-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6bab9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6bab9-122">Request headers</span></span>
|<span data-ttu-id="6bab9-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6bab9-123">Header</span></span>|<span data-ttu-id="6bab9-124">Значение</span><span class="sxs-lookup"><span data-stu-id="6bab9-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bab9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bab9-125">Authorization</span></span>|<span data-ttu-id="6bab9-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6bab9-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bab9-127">Accept</span><span class="sxs-lookup"><span data-stu-id="6bab9-127">Accept</span></span>|<span data-ttu-id="6bab9-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6bab9-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bab9-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6bab9-129">Request body</span></span>
<span data-ttu-id="6bab9-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6bab9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6bab9-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="6bab9-131">Response</span></span>
<span data-ttu-id="6bab9-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6bab9-132">If successful, this method returns a `200 OK` response code and [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bab9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="6bab9-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="6bab9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bab9-134">Request</span></span>
<span data-ttu-id="6bab9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6bab9-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="6bab9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bab9-136">Response</span></span>
<span data-ttu-id="6bab9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6bab9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1477

{
  "value": {
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
}
```



