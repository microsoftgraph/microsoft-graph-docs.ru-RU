---
title: Получение depEnrollmentProfile
description: Чтение свойств и связей объекта depEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 77f389e4e2ac26f57e0d10dc2e55a2604c4246e6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706648"
---
# <a name="get-depenrollmentprofile"></a><span data-ttu-id="8a968-103">Получение depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="8a968-103">Get depEnrollmentProfile</span></span>

<span data-ttu-id="8a968-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a968-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a968-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a968-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a968-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8a968-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a968-107">Чтение свойств и связей объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8a968-107">Read properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a968-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8a968-108">Prerequisites</span></span>
<span data-ttu-id="8a968-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a968-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a968-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a968-111">Permission type</span></span>|<span data-ttu-id="8a968-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a968-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a968-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a968-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a968-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a968-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8a968-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a968-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a968-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a968-116">Not supported.</span></span>|
|<span data-ttu-id="8a968-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a968-117">Application</span></span>|<span data-ttu-id="8a968-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a968-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a968-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a968-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8a968-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8a968-120">Optional query parameters</span></span>
<span data-ttu-id="8a968-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8a968-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8a968-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a968-122">Request headers</span></span>
|<span data-ttu-id="8a968-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8a968-123">Header</span></span>|<span data-ttu-id="8a968-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8a968-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a968-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a968-125">Authorization</span></span>|<span data-ttu-id="8a968-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a968-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a968-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8a968-127">Accept</span></span>|<span data-ttu-id="8a968-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8a968-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a968-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8a968-129">Request body</span></span>
<span data-ttu-id="8a968-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8a968-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a968-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="8a968-131">Response</span></span>
<span data-ttu-id="8a968-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8a968-132">If successful, this method returns a `200 OK` response code and [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a968-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8a968-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a968-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a968-134">Request</span></span>
<span data-ttu-id="8a968-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a968-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="8a968-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a968-136">Response</span></span>
<span data-ttu-id="8a968-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8a968-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





