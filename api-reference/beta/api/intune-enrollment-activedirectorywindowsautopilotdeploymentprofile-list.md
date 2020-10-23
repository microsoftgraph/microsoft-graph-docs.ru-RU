---
title: Список Активедиректоривиндовсаутопилотдеплойментпрофилес
description: Список свойств и связей объектов Активедиректоривиндовсаутопилотдеплойментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 90bad0ba77a3e9c78aa28e128e948bf2e6b0a072
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726075"
---
# <a name="list-activedirectorywindowsautopilotdeploymentprofiles"></a><span data-ttu-id="86e1b-103">Список Активедиректоривиндовсаутопилотдеплойментпрофилес</span><span class="sxs-lookup"><span data-stu-id="86e1b-103">List activeDirectoryWindowsAutopilotDeploymentProfiles</span></span>

<span data-ttu-id="86e1b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86e1b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86e1b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86e1b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86e1b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86e1b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86e1b-107">Список свойств и связей объектов [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="86e1b-107">List properties and relationships of the [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86e1b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="86e1b-108">Prerequisites</span></span>
<span data-ttu-id="86e1b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86e1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86e1b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86e1b-111">Permission type</span></span>|<span data-ttu-id="86e1b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="86e1b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86e1b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86e1b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86e1b-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="86e1b-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="86e1b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86e1b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86e1b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86e1b-116">Not supported.</span></span>|
|<span data-ttu-id="86e1b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86e1b-117">Application</span></span>|<span data-ttu-id="86e1b-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="86e1b-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86e1b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86e1b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="86e1b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="86e1b-120">Request headers</span></span>
|<span data-ttu-id="86e1b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86e1b-121">Header</span></span>|<span data-ttu-id="86e1b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="86e1b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86e1b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86e1b-123">Authorization</span></span>|<span data-ttu-id="86e1b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86e1b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86e1b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="86e1b-125">Accept</span></span>|<span data-ttu-id="86e1b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86e1b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86e1b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="86e1b-127">Request body</span></span>
<span data-ttu-id="86e1b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="86e1b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86e1b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="86e1b-129">Response</span></span>
<span data-ttu-id="86e1b-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [активедиректоривиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="86e1b-130">If successful, this method returns a `200 OK` response code and a collection of [activeDirectoryWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86e1b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="86e1b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="86e1b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="86e1b-132">Request</span></span>
<span data-ttu-id="86e1b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86e1b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
```

### <a name="response"></a><span data-ttu-id="86e1b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="86e1b-134">Response</span></span>
<span data-ttu-id="86e1b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86e1b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1559

{
  "value": [
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
      ],
      "hybridAzureADJoinSkipConnectivityCheck": true
    }
  ]
}
```





