---
title: Список Депиосенроллментпрофилес
description: Список свойств и связей объектов Депиосенроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b69d5268c3168ffedc29df0713ec3ec67c295226
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093898"
---
# <a name="list-depiosenrollmentprofiles"></a><span data-ttu-id="1653e-103">Список Депиосенроллментпрофилес</span><span class="sxs-lookup"><span data-stu-id="1653e-103">List depIOSEnrollmentProfiles</span></span>

<span data-ttu-id="1653e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1653e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1653e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1653e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1653e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1653e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1653e-107">Список свойств и связей объектов [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="1653e-107">List properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1653e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1653e-108">Prerequisites</span></span>
<span data-ttu-id="1653e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1653e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1653e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1653e-111">Permission type</span></span>|<span data-ttu-id="1653e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1653e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1653e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1653e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1653e-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1653e-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="1653e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1653e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1653e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1653e-116">Not supported.</span></span>|
|<span data-ttu-id="1653e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1653e-117">Application</span></span>|<span data-ttu-id="1653e-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1653e-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1653e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1653e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="1653e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1653e-120">Request headers</span></span>
|<span data-ttu-id="1653e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1653e-121">Header</span></span>|<span data-ttu-id="1653e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1653e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1653e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1653e-123">Authorization</span></span>|<span data-ttu-id="1653e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1653e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1653e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1653e-125">Accept</span></span>|<span data-ttu-id="1653e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1653e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1653e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1653e-127">Request body</span></span>
<span data-ttu-id="1653e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1653e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1653e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1653e-129">Response</span></span>
<span data-ttu-id="1653e-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1653e-130">If successful, this method returns a `200 OK` response code and a collection of [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1653e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1653e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1653e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1653e-132">Request</span></span>
<span data-ttu-id="1653e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1653e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="1653e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1653e-134">Response</span></span>
<span data-ttu-id="1653e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1653e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2322

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
      "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
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
      "iTunesPairingMode": "allow",
      "managementCertificates": [
        {
          "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
          "thumbprint": "Thumbprint value",
          "certificate": "Certificate value"
        }
      ],
      "restoreFromAndroidDisabled": true,
      "awaitDeviceConfiguredConfirmation": true,
      "sharedIPadMaximumUserCount": 10,
      "enableSharedIPad": true,
      "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
      "enableSingleAppEnrollmentMode": true,
      "homeButtonScreenDisabled": true,
      "iMessageAndFaceTimeScreenDisabled": true,
      "onBoardingScreenDisabled": true,
      "simSetupScreenDisabled": true,
      "softwareUpdateScreenDisabled": true,
      "watchMigrationScreenDisabled": true,
      "appearanceScreenDisabled": true,
      "expressLanguageScreenDisabled": true,
      "preferredLanguageScreenDisabled": true,
      "deviceToDeviceMigrationDisabled": true,
      "welcomeScreenDisabled": true
    }
  ]
}
```






