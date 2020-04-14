---
title: Получение Депиосенроллментпрофиле
description: Чтение свойств и связей объекта Депиосенроллментпрофиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 14d03fad444ce0ecb5abc4211303450dace2f075
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43363990"
---
# <a name="get-depiosenrollmentprofile"></a><span data-ttu-id="59029-103">Получение Депиосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="59029-103">Get depIOSEnrollmentProfile</span></span>

<span data-ttu-id="59029-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59029-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59029-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59029-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59029-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="59029-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59029-107">Чтение свойств и связей объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="59029-107">Read properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59029-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="59029-108">Prerequisites</span></span>
<span data-ttu-id="59029-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59029-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59029-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59029-111">Permission type</span></span>|<span data-ttu-id="59029-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="59029-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59029-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59029-113">Delegated (work or school account)</span></span>|<span data-ttu-id="59029-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="59029-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="59029-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59029-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59029-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59029-116">Not supported.</span></span>|
|<span data-ttu-id="59029-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="59029-117">Application</span></span>|<span data-ttu-id="59029-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="59029-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59029-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59029-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="59029-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="59029-120">Optional query parameters</span></span>
<span data-ttu-id="59029-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="59029-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59029-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59029-122">Request headers</span></span>
|<span data-ttu-id="59029-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="59029-123">Header</span></span>|<span data-ttu-id="59029-124">Значение</span><span class="sxs-lookup"><span data-stu-id="59029-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59029-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="59029-125">Authorization</span></span>|<span data-ttu-id="59029-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59029-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59029-127">Accept</span><span class="sxs-lookup"><span data-stu-id="59029-127">Accept</span></span>|<span data-ttu-id="59029-128">application/json</span><span class="sxs-lookup"><span data-stu-id="59029-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59029-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59029-129">Request body</span></span>
<span data-ttu-id="59029-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="59029-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59029-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="59029-131">Response</span></span>
<span data-ttu-id="59029-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="59029-132">If successful, this method returns a `200 OK` response code and [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59029-133">Пример</span><span class="sxs-lookup"><span data-stu-id="59029-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="59029-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="59029-134">Request</span></span>
<span data-ttu-id="59029-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59029-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="59029-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="59029-136">Response</span></span>
<span data-ttu-id="59029-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59029-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



