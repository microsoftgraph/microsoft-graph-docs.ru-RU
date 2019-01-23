---
title: Список azureADWindowsAutopilotDeploymentProfiles
description: Свойства списка и связей объектов azureADWindowsAutopilotDeploymentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c9eed8f4e0f9af7ca3520e390595d77828990e70
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394994"
---
# <a name="list-azureadwindowsautopilotdeploymentprofiles"></a><span data-ttu-id="2e894-103">Список azureADWindowsAutopilotDeploymentProfiles</span><span class="sxs-lookup"><span data-stu-id="2e894-103">List azureADWindowsAutopilotDeploymentProfiles</span></span>

> <span data-ttu-id="2e894-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2e894-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2e894-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e894-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e894-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e894-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e894-107">Свойства списка и связей объектов [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2e894-107">List properties and relationships of the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e894-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="2e894-108">Prerequisites</span></span>
<span data-ttu-id="2e894-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2e894-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2e894-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e894-111">Permission type</span></span>|<span data-ttu-id="2e894-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e894-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e894-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e894-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e894-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e894-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2e894-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e894-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e894-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e894-116">Not supported.</span></span>|
|<span data-ttu-id="2e894-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e894-117">Application</span></span>|<span data-ttu-id="2e894-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e894-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e894-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e894-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="2e894-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e894-120">Request headers</span></span>
|<span data-ttu-id="2e894-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e894-121">Header</span></span>|<span data-ttu-id="2e894-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2e894-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e894-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e894-123">Authorization</span></span>|<span data-ttu-id="2e894-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2e894-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e894-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2e894-125">Accept</span></span>|<span data-ttu-id="2e894-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2e894-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e894-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e894-127">Request body</span></span>
<span data-ttu-id="2e894-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e894-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e894-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e894-129">Response</span></span>
<span data-ttu-id="2e894-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2e894-130">If successful, this method returns a `200 OK` response code and a collection of [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e894-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2e894-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e894-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e894-132">Request</span></span>
<span data-ttu-id="2e894-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e894-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles
```

### <a name="response"></a><span data-ttu-id="2e894-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e894-134">Response</span></span>
<span data-ttu-id="2e894-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2e894-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1353

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
      "deviceNameTemplate": "Device Name Template value"
    }
  ]
}
```




