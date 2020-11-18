---
title: Список Депиосенроллментпрофилес
description: Список свойств и связей объектов Депиосенроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c30b97a09e0068ef3ad7808fb15035c646f2bca1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49201956"
---
# <a name="list-depiosenrollmentprofiles"></a><span data-ttu-id="0a468-103">Список Депиосенроллментпрофилес</span><span class="sxs-lookup"><span data-stu-id="0a468-103">List depIOSEnrollmentProfiles</span></span>

<span data-ttu-id="0a468-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a468-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a468-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a468-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a468-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a468-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a468-107">Список свойств и связей объектов [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0a468-107">List properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a468-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0a468-108">Prerequisites</span></span>
<span data-ttu-id="0a468-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a468-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a468-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a468-111">Permission type</span></span>|<span data-ttu-id="0a468-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a468-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a468-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a468-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a468-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a468-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="0a468-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a468-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a468-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a468-116">Not supported.</span></span>|
|<span data-ttu-id="0a468-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0a468-117">Application</span></span>|<span data-ttu-id="0a468-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a468-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a468-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a468-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="0a468-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0a468-120">Request headers</span></span>
|<span data-ttu-id="0a468-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a468-121">Header</span></span>|<span data-ttu-id="0a468-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0a468-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a468-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a468-123">Authorization</span></span>|<span data-ttu-id="0a468-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a468-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a468-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0a468-125">Accept</span></span>|<span data-ttu-id="0a468-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a468-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a468-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a468-127">Request body</span></span>
<span data-ttu-id="0a468-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0a468-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a468-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a468-129">Response</span></span>
<span data-ttu-id="0a468-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0a468-130">If successful, this method returns a `200 OK` response code and a collection of [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a468-131">Пример</span><span class="sxs-lookup"><span data-stu-id="0a468-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a468-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a468-132">Request</span></span>
<span data-ttu-id="0a468-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a468-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="0a468-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a468-134">Response</span></span>
<span data-ttu-id="0a468-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a468-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2414

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
      "isMandatory": true,
      "locationDisabled": true,
      "supportPhoneNumber": "Support Phone Number value",
      "profileRemovalDisabled": true,
      "restoreBlocked": true,
      "appleIdDisabled": true,
      "termsAndConditionsDisabled": true,
      "touchIdDisabled": true,
      "applePayDisabled": true,
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
      "welcomeScreenDisabled": true,
      "passCodeDisabled": true,
      "zoomDisabled": true,
      "restoreCompletedScreenDisabled": true,
      "updateCompleteScreenDisabled": true
    }
  ]
}
```




