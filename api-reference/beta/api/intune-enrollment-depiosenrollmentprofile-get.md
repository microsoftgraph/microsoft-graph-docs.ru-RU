---
title: Получение Депиосенроллментпрофиле
description: Чтение свойств и связей объекта Депиосенроллментпрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 035b18bad6b3bcb9af7699221c210f88edc794f1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979342"
---
# <a name="get-depiosenrollmentprofile"></a><span data-ttu-id="fa629-103">Получение Депиосенроллментпрофиле</span><span class="sxs-lookup"><span data-stu-id="fa629-103">Get depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="fa629-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa629-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa629-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa629-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa629-106">Чтение свойств и связей объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="fa629-106">Read properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa629-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fa629-107">Prerequisites</span></span>
<span data-ttu-id="fa629-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa629-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa629-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa629-110">Permission type</span></span>|<span data-ttu-id="fa629-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa629-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa629-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa629-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa629-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa629-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fa629-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa629-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa629-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa629-115">Not supported.</span></span>|
|<span data-ttu-id="fa629-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa629-116">Application</span></span>|<span data-ttu-id="fa629-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa629-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa629-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa629-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa629-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fa629-119">Optional query parameters</span></span>
<span data-ttu-id="fa629-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fa629-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa629-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa629-121">Request headers</span></span>
|<span data-ttu-id="fa629-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa629-122">Header</span></span>|<span data-ttu-id="fa629-123">Значение</span><span class="sxs-lookup"><span data-stu-id="fa629-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa629-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa629-124">Authorization</span></span>|<span data-ttu-id="fa629-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa629-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa629-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fa629-126">Accept</span></span>|<span data-ttu-id="fa629-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fa629-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa629-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fa629-128">Request body</span></span>
<span data-ttu-id="fa629-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa629-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa629-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa629-130">Response</span></span>
<span data-ttu-id="fa629-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa629-131">If successful, this method returns a `200 OK` response code and [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa629-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fa629-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa629-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa629-133">Request</span></span>
<span data-ttu-id="fa629-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa629-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="fa629-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa629-135">Response</span></span>
<span data-ttu-id="fa629-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa629-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1955

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
}
```





