---
title: Список Депиосенроллментпрофилес
description: Список свойств и связей объектов Депиосенроллментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aff96cc3d91c9c6d573724bc5d93b1dab7e09e79
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348251"
---
# <a name="list-depiosenrollmentprofiles"></a><span data-ttu-id="474f0-103">Список Депиосенроллментпрофилес</span><span class="sxs-lookup"><span data-stu-id="474f0-103">List depIOSEnrollmentProfiles</span></span>

> <span data-ttu-id="474f0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="474f0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="474f0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="474f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="474f0-106">Список свойств и связей объектов [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="474f0-106">List properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="474f0-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="474f0-107">Prerequisites</span></span>
<span data-ttu-id="474f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="474f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="474f0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="474f0-110">Permission type</span></span>|<span data-ttu-id="474f0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="474f0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="474f0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="474f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="474f0-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="474f0-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="474f0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="474f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="474f0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="474f0-115">Not supported.</span></span>|
|<span data-ttu-id="474f0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="474f0-116">Application</span></span>|<span data-ttu-id="474f0-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="474f0-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="474f0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="474f0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="474f0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="474f0-119">Request headers</span></span>
|<span data-ttu-id="474f0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="474f0-120">Header</span></span>|<span data-ttu-id="474f0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="474f0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="474f0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="474f0-122">Authorization</span></span>|<span data-ttu-id="474f0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="474f0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="474f0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="474f0-124">Accept</span></span>|<span data-ttu-id="474f0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="474f0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="474f0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="474f0-126">Request body</span></span>
<span data-ttu-id="474f0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="474f0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="474f0-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="474f0-128">Response</span></span>
<span data-ttu-id="474f0-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="474f0-129">If successful, this method returns a `200 OK` response code and a collection of [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="474f0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="474f0-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="474f0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="474f0-131">Request</span></span>
<span data-ttu-id="474f0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="474f0-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="474f0-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="474f0-133">Response</span></span>
<span data-ttu-id="474f0-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="474f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2065

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
      "deviceNameTemplate": "Device Name Template value",
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
      "screenTimeScreenDisabled": true,
      "simSetupScreenDisabled": true,
      "softwareUpdateScreenDisabled": true,
      "watchMigrationScreenDisabled": true
    }
  ]
}
```






