---
title: Get azureADWindowsAutopilotDeploymentProfile
description: Чтение свойств и связей объекта azureADWindowsAutopilotDeploymentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b6c6a0289e9457a51dfaac13d6185cd155ff5f0b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126271"
---
# <a name="get-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="fe785-103">Get azureADWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="fe785-103">Get azureADWindowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="fe785-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe785-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe785-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe785-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe785-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe785-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe785-107">Чтение свойств и связей объекта [azureADWindowsAutopilotDeploymentProfile.](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fe785-107">Read properties and relationships of the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe785-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fe785-108">Prerequisites</span></span>
<span data-ttu-id="fe785-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe785-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe785-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe785-111">Permission type</span></span>|<span data-ttu-id="fe785-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe785-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe785-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe785-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe785-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe785-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fe785-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe785-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe785-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe785-116">Not supported.</span></span>|
|<span data-ttu-id="fe785-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fe785-117">Application</span></span>|<span data-ttu-id="fe785-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe785-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe785-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe785-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe785-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fe785-120">Optional query parameters</span></span>
<span data-ttu-id="fe785-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fe785-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe785-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe785-122">Request headers</span></span>
|<span data-ttu-id="fe785-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe785-123">Header</span></span>|<span data-ttu-id="fe785-124">Значение</span><span class="sxs-lookup"><span data-stu-id="fe785-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe785-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe785-125">Authorization</span></span>|<span data-ttu-id="fe785-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe785-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe785-127">Accept</span><span class="sxs-lookup"><span data-stu-id="fe785-127">Accept</span></span>|<span data-ttu-id="fe785-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fe785-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe785-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe785-129">Request body</span></span>
<span data-ttu-id="fe785-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe785-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe785-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe785-131">Response</span></span>
<span data-ttu-id="fe785-132">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fe785-132">If successful, this method returns a `200 OK` response code and [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe785-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fe785-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe785-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe785-134">Request</span></span>
<span data-ttu-id="fe785-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe785-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="fe785-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe785-136">Response</span></span>
<span data-ttu-id="fe785-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe785-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1416

{
  "value": {
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
}
```




