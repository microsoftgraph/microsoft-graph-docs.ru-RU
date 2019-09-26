---
title: Получение depEnrollmentProfile
description: Чтение свойств и связей объекта depEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 981b7878ba5263df99013c05d5f508db7b8d51f6
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37185499"
---
# <a name="get-depenrollmentprofile"></a><span data-ttu-id="f4053-103">Получение depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="f4053-103">Get depEnrollmentProfile</span></span>

> <span data-ttu-id="f4053-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4053-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4053-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4053-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4053-106">Чтение свойств и связей объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f4053-106">Read properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4053-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f4053-107">Prerequisites</span></span>
<span data-ttu-id="f4053-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4053-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4053-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4053-110">Permission type</span></span>|<span data-ttu-id="f4053-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4053-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4053-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4053-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4053-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4053-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f4053-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4053-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4053-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4053-115">Not supported.</span></span>|
|<span data-ttu-id="f4053-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4053-116">Application</span></span>|<span data-ttu-id="f4053-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4053-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4053-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4053-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4053-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f4053-119">Optional query parameters</span></span>
<span data-ttu-id="f4053-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f4053-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4053-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4053-121">Request headers</span></span>
|<span data-ttu-id="f4053-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4053-122">Header</span></span>|<span data-ttu-id="f4053-123">Значение</span><span class="sxs-lookup"><span data-stu-id="f4053-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4053-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4053-124">Authorization</span></span>|<span data-ttu-id="f4053-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4053-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4053-126">Accept</span><span class="sxs-lookup"><span data-stu-id="f4053-126">Accept</span></span>|<span data-ttu-id="f4053-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f4053-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4053-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f4053-128">Request body</span></span>
<span data-ttu-id="f4053-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f4053-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4053-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="f4053-130">Response</span></span>
<span data-ttu-id="f4053-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f4053-131">If successful, this method returns a `200 OK` response code and [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4053-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f4053-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4053-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4053-133">Request</span></span>
<span data-ttu-id="f4053-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4053-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="f4053-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4053-135">Response</span></span>
<span data-ttu-id="f4053-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4053-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1498

{
  "value": {
    "@odata.type": "#microsoft.graph.depEnrollmentProfile",
    "id": "3d4534f7-34f7-3d45-f734-453df734453d",
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
    "iTunesPairingMode": "allow",
    "profileRemovalDisabled": true,
    "managementCertificates": [
      {
        "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
        "thumbprint": "Thumbprint value",
        "certificate": "Certificate value"
      }
    ],
    "restoreBlocked": true,
    "restoreFromAndroidDisabled": true,
    "appleIdDisabled": true,
    "termsAndConditionsDisabled": true,
    "touchIdDisabled": true,
    "applePayDisabled": true,
    "zoomDisabled": true,
    "siriDisabled": true,
    "diagnosticsDisabled": true,
    "macOSRegistrationDisabled": true,
    "macOSFileVaultDisabled": true,
    "awaitDeviceConfiguredConfirmation": true,
    "sharedIPadMaximumUserCount": 10,
    "enableSharedIPad": true
  }
}
```




