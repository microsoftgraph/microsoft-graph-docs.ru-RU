---
title: Список Азуреадвиндовсаутопилотдеплойментпрофилес
description: Список свойств и связей объектов Азуреадвиндовсаутопилотдеплойментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd407f67e94bbae6d8a71284554198e96bd45c45
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37185520"
---
# <a name="list-azureadwindowsautopilotdeploymentprofiles"></a><span data-ttu-id="ae687-103">Список Азуреадвиндовсаутопилотдеплойментпрофилес</span><span class="sxs-lookup"><span data-stu-id="ae687-103">List azureADWindowsAutopilotDeploymentProfiles</span></span>

> <span data-ttu-id="ae687-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae687-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae687-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae687-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae687-106">Список свойств и связей объектов [азуреадвиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ae687-106">List properties and relationships of the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae687-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ae687-107">Prerequisites</span></span>
<span data-ttu-id="ae687-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae687-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae687-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae687-110">Permission type</span></span>|<span data-ttu-id="ae687-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae687-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae687-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae687-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae687-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae687-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ae687-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae687-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae687-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae687-115">Not supported.</span></span>|
|<span data-ttu-id="ae687-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae687-116">Application</span></span>|<span data-ttu-id="ae687-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae687-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae687-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae687-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="ae687-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae687-119">Request headers</span></span>
|<span data-ttu-id="ae687-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae687-120">Header</span></span>|<span data-ttu-id="ae687-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ae687-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae687-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae687-122">Authorization</span></span>|<span data-ttu-id="ae687-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae687-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae687-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ae687-124">Accept</span></span>|<span data-ttu-id="ae687-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae687-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae687-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ae687-126">Request body</span></span>
<span data-ttu-id="ae687-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae687-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae687-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ae687-128">Response</span></span>
<span data-ttu-id="ae687-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [азуреадвиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ae687-129">If successful, this method returns a `200 OK` response code and a collection of [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae687-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ae687-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae687-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae687-131">Request</span></span>
<span data-ttu-id="ae687-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae687-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
```

### <a name="response"></a><span data-ttu-id="ae687-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae687-133">Response</span></span>
<span data-ttu-id="ae687-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae687-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1496

{
  "value": [
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
      "deviceNameTemplate": "Device Name Template value",
      "deviceType": "surfaceHub2",
      "enableWhiteGlove": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




