---
title: Список Депиосенроллментпрофилес
description: Список свойств и связей объектов Депиосенроллментпрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5c75d0a77cb372fbbd47a9c27c9ddd442376e475
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966280"
---
# <a name="list-depiosenrollmentprofiles"></a><span data-ttu-id="f9b3d-103">Список Депиосенроллментпрофилес</span><span class="sxs-lookup"><span data-stu-id="f9b3d-103">List depIOSEnrollmentProfiles</span></span>

> <span data-ttu-id="f9b3d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9b3d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9b3d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9b3d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9b3d-106">Список свойств и связей объектов [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f9b3d-106">List properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9b3d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f9b3d-107">Prerequisites</span></span>
<span data-ttu-id="f9b3d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9b3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9b3d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9b3d-110">Permission type</span></span>|<span data-ttu-id="f9b3d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9b3d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9b3d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9b3d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9b3d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9b3d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f9b3d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9b3d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9b3d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9b3d-115">Not supported.</span></span>|
|<span data-ttu-id="f9b3d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9b3d-116">Application</span></span>|<span data-ttu-id="f9b3d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9b3d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9b3d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9b3d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="f9b3d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9b3d-119">Request headers</span></span>
|<span data-ttu-id="f9b3d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f9b3d-120">Header</span></span>|<span data-ttu-id="f9b3d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f9b3d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9b3d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9b3d-122">Authorization</span></span>|<span data-ttu-id="f9b3d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9b3d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9b3d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f9b3d-124">Accept</span></span>|<span data-ttu-id="f9b3d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9b3d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9b3d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9b3d-126">Request body</span></span>
<span data-ttu-id="f9b3d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f9b3d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9b3d-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9b3d-128">Response</span></span>
<span data-ttu-id="f9b3d-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f9b3d-129">If successful, this method returns a `200 OK` response code and a collection of [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9b3d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f9b3d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9b3d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9b3d-131">Request</span></span>
<span data-ttu-id="f9b3d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f9b3d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="f9b3d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9b3d-133">Response</span></span>
<span data-ttu-id="f9b3d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f9b3d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2006

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




