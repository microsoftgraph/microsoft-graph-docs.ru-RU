---
title: Список Депмакосенроллментпрофилес
description: Список свойств и связей объектов Депмакосенроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c347220d6290405681c41519a14e35e58e05e4ba
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443494"
---
# <a name="list-depmacosenrollmentprofiles"></a><span data-ttu-id="68054-103">Список Депмакосенроллментпрофилес</span><span class="sxs-lookup"><span data-stu-id="68054-103">List depMacOSEnrollmentProfiles</span></span>

<span data-ttu-id="68054-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68054-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68054-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68054-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68054-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68054-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68054-107">Список свойств и связей объектов [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="68054-107">List properties and relationships of the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68054-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="68054-108">Prerequisites</span></span>
<span data-ttu-id="68054-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68054-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68054-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68054-111">Permission type</span></span>|<span data-ttu-id="68054-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68054-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68054-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68054-113">Delegated (work or school account)</span></span>|<span data-ttu-id="68054-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="68054-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="68054-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68054-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68054-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68054-116">Not supported.</span></span>|
|<span data-ttu-id="68054-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="68054-117">Application</span></span>|<span data-ttu-id="68054-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="68054-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68054-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68054-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="68054-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="68054-120">Request headers</span></span>
|<span data-ttu-id="68054-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68054-121">Header</span></span>|<span data-ttu-id="68054-122">Значение</span><span class="sxs-lookup"><span data-stu-id="68054-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68054-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="68054-123">Authorization</span></span>|<span data-ttu-id="68054-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68054-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68054-125">Accept</span><span class="sxs-lookup"><span data-stu-id="68054-125">Accept</span></span>|<span data-ttu-id="68054-126">application/json</span><span class="sxs-lookup"><span data-stu-id="68054-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68054-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68054-127">Request body</span></span>
<span data-ttu-id="68054-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68054-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68054-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="68054-129">Response</span></span>
<span data-ttu-id="68054-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="68054-130">If successful, this method returns a `200 OK` response code and a collection of [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68054-131">Пример</span><span class="sxs-lookup"><span data-stu-id="68054-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="68054-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="68054-132">Request</span></span>
<span data-ttu-id="68054-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68054-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="68054-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="68054-134">Response</span></span>
<span data-ttu-id="68054-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68054-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1478

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
      "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
      "displayName": "Display Name value",
      "description": "Description value",
      "requiresUserAuthentication": true,
      "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
      "enableAuthenticationViaCompanyPortal": true,
      "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
      "isDefault": true,
      "supervisedModeEnabled": true,
      "supportDepartment": "Support Department value",
      "passCodeDisabled": true,
      "isMandatory": true,
      "locationDisabled": true,
      "supportPhoneNumber": "Support Phone Number value",
      "profileRemovalDisabled": true,
      "restoreBlocked": true,
      "appleIdDisabled": true,
      "termsAndConditionsDisabled": true,
      "touchIdDisabled": true,
      "applePayDisabled": true,
      "zoomDisabled": true,
      "siriDisabled": true,
      "diagnosticsDisabled": true,
      "displayToneSetupDisabled": true,
      "privacyPaneDisabled": true,
      "screenTimeScreenDisabled": true,
      "deviceNameTemplate": "Device Name Template value",
      "configurationWebUrl": true,
      "registrationDisabled": true,
      "fileVaultDisabled": true,
      "iCloudDiagnosticsDisabled": true,
      "iCloudStorageDisabled": true,
      "chooseYourLockScreenDisabled": true
    }
  ]
}
```



