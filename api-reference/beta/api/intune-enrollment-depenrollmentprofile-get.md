---
title: Получить depEnrollmentProfile
description: Чтение свойств и связей объекта depEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9fa0ac0a03c6630998ceff78628e767cff11979c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146015"
---
# <a name="get-depenrollmentprofile"></a><span data-ttu-id="1a095-103">Получить depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="1a095-103">Get depEnrollmentProfile</span></span>

<span data-ttu-id="1a095-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a095-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a095-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a095-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a095-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a095-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a095-107">Чтение свойств и связей объекта [depEnrollmentProfile.](../resources/intune-enrollment-depenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1a095-107">Read properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a095-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1a095-108">Prerequisites</span></span>
<span data-ttu-id="1a095-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a095-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a095-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a095-111">Permission type</span></span>|<span data-ttu-id="1a095-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a095-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a095-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a095-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a095-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a095-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1a095-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a095-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a095-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a095-116">Not supported.</span></span>|
|<span data-ttu-id="1a095-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1a095-117">Application</span></span>|<span data-ttu-id="1a095-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a095-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a095-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a095-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a095-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1a095-120">Optional query parameters</span></span>
<span data-ttu-id="1a095-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1a095-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a095-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a095-122">Request headers</span></span>
|<span data-ttu-id="1a095-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1a095-123">Header</span></span>|<span data-ttu-id="1a095-124">Значение</span><span class="sxs-lookup"><span data-stu-id="1a095-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a095-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a095-125">Authorization</span></span>|<span data-ttu-id="1a095-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a095-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a095-127">Accept</span><span class="sxs-lookup"><span data-stu-id="1a095-127">Accept</span></span>|<span data-ttu-id="1a095-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1a095-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a095-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a095-129">Request body</span></span>
<span data-ttu-id="1a095-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1a095-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a095-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a095-131">Response</span></span>
<span data-ttu-id="1a095-132">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [объект depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1a095-132">If successful, this method returns a `200 OK` response code and [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a095-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1a095-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a095-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a095-134">Request</span></span>
<span data-ttu-id="1a095-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a095-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="1a095-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a095-136">Response</span></span>
<span data-ttu-id="1a095-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a095-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




