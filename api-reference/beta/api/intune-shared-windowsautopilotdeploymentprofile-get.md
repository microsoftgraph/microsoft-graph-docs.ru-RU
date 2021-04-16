---
title: Получить windowsAutopilotDeploymentProfile
description: Чтение свойств и связей объекта windowsAutopilotDeploymentProfile.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3ab309a198887601778724f473f31e622a6ec9c0
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866400"
---
# <a name="get-windowsautopilotdeploymentprofile"></a><span data-ttu-id="ba078-103">Получить windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="ba078-103">Get windowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="ba078-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba078-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba078-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba078-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba078-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba078-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba078-107">Чтение свойств и связей [объекта windowsAutopilotDeploymentProfile.](../resources/intune-shared-windowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ba078-107">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba078-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ba078-108">Prerequisites</span></span>
<span data-ttu-id="ba078-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba078-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba078-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba078-111">Permission type</span></span>|<span data-ttu-id="ba078-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba078-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba078-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba078-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ba078-114">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="ba078-114">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="ba078-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba078-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="ba078-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="ba078-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ba078-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba078-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ba078-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba078-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba078-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba078-119">Not supported.</span></span>|
|<span data-ttu-id="ba078-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ba078-120">Application</span></span>||
| <span data-ttu-id="ba078-121">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="ba078-121">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="ba078-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba078-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="ba078-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="ba078-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ba078-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba078-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba078-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba078-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba078-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ba078-126">Optional query parameters</span></span>
<span data-ttu-id="ba078-127">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ba078-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba078-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba078-128">Request headers</span></span>
|<span data-ttu-id="ba078-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba078-129">Header</span></span>|<span data-ttu-id="ba078-130">Значение</span><span class="sxs-lookup"><span data-stu-id="ba078-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba078-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba078-131">Authorization</span></span>|<span data-ttu-id="ba078-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba078-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba078-133">Accept</span><span class="sxs-lookup"><span data-stu-id="ba078-133">Accept</span></span>|<span data-ttu-id="ba078-134">application/json</span><span class="sxs-lookup"><span data-stu-id="ba078-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba078-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba078-135">Request body</span></span>
<span data-ttu-id="ba078-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba078-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba078-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba078-137">Response</span></span>
<span data-ttu-id="ba078-138">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект WindowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ba078-138">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba078-139">Пример</span><span class="sxs-lookup"><span data-stu-id="ba078-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba078-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba078-140">Request</span></span>
<span data-ttu-id="ba078-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba078-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="ba078-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba078-142">Response</span></span>
<span data-ttu-id="ba078-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba078-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







