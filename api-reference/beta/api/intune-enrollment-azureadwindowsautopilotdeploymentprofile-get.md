---
title: Получение Азуреадвиндовсаутопилотдеплойментпрофиле
description: Чтение свойств и связей объекта Азуреадвиндовсаутопилотдеплойментпрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ff7614253e98abc88c22307b8ea8e105f3c73c4
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30570796"
---
# <a name="get-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="194ac-103">Получение Азуреадвиндовсаутопилотдеплойментпрофиле</span><span class="sxs-lookup"><span data-stu-id="194ac-103">Get azureADWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="194ac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="194ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="194ac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="194ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="194ac-106">Чтение свойств и связей объекта [азуреадвиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="194ac-106">Read properties and relationships of the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="194ac-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="194ac-107">Prerequisites</span></span>
<span data-ttu-id="194ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="194ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="194ac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="194ac-110">Permission type</span></span>|<span data-ttu-id="194ac-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="194ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="194ac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="194ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="194ac-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="194ac-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="194ac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="194ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="194ac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="194ac-115">Not supported.</span></span>|
|<span data-ttu-id="194ac-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="194ac-116">Application</span></span>|<span data-ttu-id="194ac-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="194ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="194ac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="194ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="194ac-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="194ac-119">Optional query parameters</span></span>
<span data-ttu-id="194ac-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="194ac-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="194ac-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="194ac-121">Request headers</span></span>
|<span data-ttu-id="194ac-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="194ac-122">Header</span></span>|<span data-ttu-id="194ac-123">Значение</span><span class="sxs-lookup"><span data-stu-id="194ac-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="194ac-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="194ac-124">Authorization</span></span>|<span data-ttu-id="194ac-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="194ac-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="194ac-126">Accept</span><span class="sxs-lookup"><span data-stu-id="194ac-126">Accept</span></span>|<span data-ttu-id="194ac-127">application/json</span><span class="sxs-lookup"><span data-stu-id="194ac-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="194ac-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="194ac-128">Request body</span></span>
<span data-ttu-id="194ac-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="194ac-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="194ac-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="194ac-130">Response</span></span>
<span data-ttu-id="194ac-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [азуреадвиндовсаутопилотдеплойментпрофиле](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="194ac-131">If successful, this method returns a `200 OK` response code and [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="194ac-132">Пример</span><span class="sxs-lookup"><span data-stu-id="194ac-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="194ac-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="194ac-133">Request</span></span>
<span data-ttu-id="194ac-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="194ac-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="194ac-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="194ac-135">Response</span></span>
<span data-ttu-id="194ac-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="194ac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1348

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
    "enableWhiteGlove": true
  }
}
```




