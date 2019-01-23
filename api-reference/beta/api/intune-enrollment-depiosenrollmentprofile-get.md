---
title: Получение depIOSEnrollmentProfile
description: Чтение свойства и связи объекта depIOSEnrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0bc4363e1f84830f91fd5defc543325ad3d3b8ad
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423239"
---
# <a name="get-depiosenrollmentprofile"></a><span data-ttu-id="e439f-103">Получение depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e439f-103">Get depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="e439f-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e439f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e439f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e439f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e439f-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e439f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e439f-107">Чтение свойства и связи объекта [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e439f-107">Read properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e439f-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="e439f-108">Prerequisites</span></span>
<span data-ttu-id="e439f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e439f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e439f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e439f-111">Permission type</span></span>|<span data-ttu-id="e439f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e439f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e439f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e439f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e439f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e439f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e439f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e439f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e439f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e439f-116">Not supported.</span></span>|
|<span data-ttu-id="e439f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e439f-117">Application</span></span>|<span data-ttu-id="e439f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e439f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e439f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e439f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e439f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e439f-120">Optional query parameters</span></span>
<span data-ttu-id="e439f-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e439f-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e439f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e439f-122">Request headers</span></span>
|<span data-ttu-id="e439f-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e439f-123">Header</span></span>|<span data-ttu-id="e439f-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e439f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e439f-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e439f-125">Authorization</span></span>|<span data-ttu-id="e439f-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e439f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e439f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e439f-127">Accept</span></span>|<span data-ttu-id="e439f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e439f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e439f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e439f-129">Request body</span></span>
<span data-ttu-id="e439f-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e439f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e439f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e439f-131">Response</span></span>
<span data-ttu-id="e439f-132">Успешно завершена, этот метод возвращает `200 OK` объект [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e439f-132">If successful, this method returns a `200 OK` response code and [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e439f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e439f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e439f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e439f-134">Request</span></span>
<span data-ttu-id="e439f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e439f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="e439f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e439f-136">Response</span></span>
<span data-ttu-id="e439f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e439f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1898

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




