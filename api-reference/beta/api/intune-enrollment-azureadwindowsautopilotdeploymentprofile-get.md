---
title: Получение azureADWindowsAutopilotDeploymentProfile
description: Чтение свойства и связи объекта azureADWindowsAutopilotDeploymentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0c01d9c3a62d7c75aa03b6c72bc7a2c9897a5ce0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954836"
---
# <a name="get-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="56381-103">Получение azureADWindowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="56381-103">Get azureADWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="56381-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="56381-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56381-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56381-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56381-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="56381-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56381-107">Чтение свойства и связи объекта [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="56381-107">Read properties and relationships of the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56381-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="56381-108">Prerequisites</span></span>
<span data-ttu-id="56381-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56381-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56381-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56381-111">Permission type</span></span>|<span data-ttu-id="56381-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="56381-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56381-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56381-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56381-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="56381-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="56381-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56381-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56381-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56381-116">Not supported.</span></span>|
|<span data-ttu-id="56381-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56381-117">Application</span></span>|<span data-ttu-id="56381-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56381-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56381-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56381-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56381-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="56381-120">Optional query parameters</span></span>
<span data-ttu-id="56381-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="56381-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="56381-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56381-122">Request headers</span></span>
|<span data-ttu-id="56381-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="56381-123">Header</span></span>|<span data-ttu-id="56381-124">Значение</span><span class="sxs-lookup"><span data-stu-id="56381-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56381-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="56381-125">Authorization</span></span>|<span data-ttu-id="56381-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="56381-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56381-127">Accept</span><span class="sxs-lookup"><span data-stu-id="56381-127">Accept</span></span>|<span data-ttu-id="56381-128">application/json</span><span class="sxs-lookup"><span data-stu-id="56381-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56381-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="56381-129">Request body</span></span>
<span data-ttu-id="56381-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="56381-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56381-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="56381-131">Response</span></span>
<span data-ttu-id="56381-132">Успешно завершена, этот метод возвращает `200 OK` объект [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="56381-132">If successful, this method returns a `200 OK` response code and [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56381-133">Пример</span><span class="sxs-lookup"><span data-stu-id="56381-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="56381-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="56381-134">Request</span></span>
<span data-ttu-id="56381-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56381-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="56381-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="56381-136">Response</span></span>
<span data-ttu-id="56381-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="56381-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1283

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
    "deviceNameTemplate": "Device Name Template value"
  }
}
```





