---
title: Получение windowsAutopilotDeploymentProfile
description: Чтение свойств и связей объекта windowsAutopilotDeploymentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 475f04a3222c5ea32c0555d2991b4f263e1a1cd8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217426"
---
# <a name="get-windowsautopilotdeploymentprofile"></a><span data-ttu-id="c8e03-103">Получение windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="c8e03-103">Get windowsAutopilotDeploymentProfile</span></span>

<span data-ttu-id="c8e03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8e03-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8e03-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8e03-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8e03-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8e03-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8e03-107">Чтение свойств и связей объекта [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="c8e03-107">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8e03-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c8e03-108">Prerequisites</span></span>
<span data-ttu-id="c8e03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8e03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8e03-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8e03-111">Permission type</span></span>|<span data-ttu-id="c8e03-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8e03-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8e03-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8e03-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c8e03-114">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="c8e03-114">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="c8e03-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8e03-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="c8e03-116">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="c8e03-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c8e03-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8e03-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c8e03-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8e03-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8e03-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8e03-119">Not supported.</span></span>|
|<span data-ttu-id="c8e03-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="c8e03-120">Application</span></span>||
| <span data-ttu-id="c8e03-121">&nbsp;&nbsp; **Регистрация**</span><span class="sxs-lookup"><span data-stu-id="c8e03-121">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="c8e03-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8e03-122">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
| <span data-ttu-id="c8e03-123">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="c8e03-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="c8e03-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8e03-124">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8e03-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8e03-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8e03-126">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c8e03-126">Optional query parameters</span></span>
<span data-ttu-id="c8e03-127">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c8e03-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8e03-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c8e03-128">Request headers</span></span>
|<span data-ttu-id="c8e03-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8e03-129">Header</span></span>|<span data-ttu-id="c8e03-130">Значение</span><span class="sxs-lookup"><span data-stu-id="c8e03-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8e03-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8e03-131">Authorization</span></span>|<span data-ttu-id="c8e03-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8e03-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8e03-133">Accept</span><span class="sxs-lookup"><span data-stu-id="c8e03-133">Accept</span></span>|<span data-ttu-id="c8e03-134">application/json</span><span class="sxs-lookup"><span data-stu-id="c8e03-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8e03-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8e03-135">Request body</span></span>
<span data-ttu-id="c8e03-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c8e03-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8e03-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8e03-137">Response</span></span>
<span data-ttu-id="c8e03-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c8e03-138">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8e03-139">Пример</span><span class="sxs-lookup"><span data-stu-id="c8e03-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8e03-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8e03-140">Request</span></span>
<span data-ttu-id="c8e03-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8e03-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="c8e03-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8e03-142">Response</span></span>
<span data-ttu-id="c8e03-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8e03-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







