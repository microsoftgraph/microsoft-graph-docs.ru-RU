---
title: Получение windowsAutopilotDeploymentProfile
description: Чтение свойств и связей объекта windowsAutopilotDeploymentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92aad7b681d4e49a0857a31bf0718c6c72766f9e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145495"
---
# <a name="get-windowsautopilotdeploymentprofile"></a><span data-ttu-id="57611-103">Получение windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="57611-103">Get windowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="57611-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57611-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57611-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57611-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57611-106">Чтение свойств и связей объекта [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="57611-106">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57611-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="57611-107">Prerequisites</span></span>
<span data-ttu-id="57611-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="57611-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="57611-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57611-110">Permission type</span></span>|<span data-ttu-id="57611-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="57611-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57611-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57611-112">Delegated (work or school account)</span></span>|<span data-ttu-id="57611-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="57611-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="57611-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57611-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57611-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57611-115">Not supported.</span></span>|
|<span data-ttu-id="57611-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57611-116">Application</span></span>|<span data-ttu-id="57611-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57611-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57611-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57611-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="57611-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="57611-119">Optional query parameters</span></span>
<span data-ttu-id="57611-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="57611-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="57611-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57611-121">Request headers</span></span>
|<span data-ttu-id="57611-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57611-122">Header</span></span>|<span data-ttu-id="57611-123">Значение</span><span class="sxs-lookup"><span data-stu-id="57611-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57611-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57611-124">Authorization</span></span>|<span data-ttu-id="57611-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="57611-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57611-126">Accept</span><span class="sxs-lookup"><span data-stu-id="57611-126">Accept</span></span>|<span data-ttu-id="57611-127">application/json</span><span class="sxs-lookup"><span data-stu-id="57611-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57611-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57611-128">Request body</span></span>
<span data-ttu-id="57611-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57611-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57611-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="57611-130">Response</span></span>
<span data-ttu-id="57611-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57611-131">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57611-132">Пример</span><span class="sxs-lookup"><span data-stu-id="57611-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="57611-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="57611-133">Request</span></span>
<span data-ttu-id="57611-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57611-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="57611-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="57611-135">Response</span></span>
<span data-ttu-id="57611-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57611-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1307

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
    "enableWhiteGlove": true
  }
}
```




