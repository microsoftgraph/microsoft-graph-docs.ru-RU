---
title: Получение Депиосенроллментпрофиле
description: Чтение свойств и связей объекта Депиосенроллментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d389376dc1406dfeea1ec004bd537a158246124c
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087301"
---
# <a name="get-depiosenrollmentprofile"></a><span data-ttu-id="2f49a-103">Получение Депиосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="2f49a-103">Get depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="2f49a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f49a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f49a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f49a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f49a-106">Чтение свойств и связей объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2f49a-106">Read properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f49a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2f49a-107">Prerequisites</span></span>
<span data-ttu-id="2f49a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f49a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f49a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f49a-110">Permission type</span></span>|<span data-ttu-id="2f49a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f49a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f49a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f49a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f49a-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f49a-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2f49a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f49a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f49a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f49a-115">Not supported.</span></span>|
|<span data-ttu-id="2f49a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f49a-116">Application</span></span>|<span data-ttu-id="2f49a-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f49a-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f49a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f49a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f49a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2f49a-119">Optional query parameters</span></span>
<span data-ttu-id="2f49a-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2f49a-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f49a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f49a-121">Request headers</span></span>
|<span data-ttu-id="2f49a-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f49a-122">Header</span></span>|<span data-ttu-id="2f49a-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2f49a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f49a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f49a-124">Authorization</span></span>|<span data-ttu-id="2f49a-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f49a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f49a-126">Accept</span><span class="sxs-lookup"><span data-stu-id="2f49a-126">Accept</span></span>|<span data-ttu-id="2f49a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2f49a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f49a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f49a-128">Request body</span></span>
<span data-ttu-id="2f49a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f49a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f49a-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f49a-130">Response</span></span>
<span data-ttu-id="2f49a-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f49a-131">If successful, this method returns a `200 OK` response code and [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f49a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2f49a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f49a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f49a-133">Request</span></span>
<span data-ttu-id="2f49a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f49a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="2f49a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f49a-135">Response</span></span>
<span data-ttu-id="2f49a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f49a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2200

{
  "value": {
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
}
```






