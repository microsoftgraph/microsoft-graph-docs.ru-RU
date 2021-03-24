---
title: Список depEnrollmentProfiles
description: Список свойств и связей объектов depEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 60f10769dadec31f38e475e0896a197811f0620d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146002"
---
# <a name="list-depenrollmentprofiles"></a><span data-ttu-id="721cf-103">Список depEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="721cf-103">List depEnrollmentProfiles</span></span>

<span data-ttu-id="721cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="721cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="721cf-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="721cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="721cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="721cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="721cf-107">Список свойств и связей объектов [depEnrollmentProfile.](../resources/intune-enrollment-depenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="721cf-107">List properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="721cf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="721cf-108">Prerequisites</span></span>
<span data-ttu-id="721cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="721cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="721cf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="721cf-111">Permission type</span></span>|<span data-ttu-id="721cf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="721cf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="721cf-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="721cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="721cf-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="721cf-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="721cf-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="721cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="721cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="721cf-116">Not supported.</span></span>|
|<span data-ttu-id="721cf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="721cf-117">Application</span></span>|<span data-ttu-id="721cf-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="721cf-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="721cf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="721cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="721cf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="721cf-120">Request headers</span></span>
|<span data-ttu-id="721cf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="721cf-121">Header</span></span>|<span data-ttu-id="721cf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="721cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="721cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="721cf-123">Authorization</span></span>|<span data-ttu-id="721cf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="721cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="721cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="721cf-125">Accept</span></span>|<span data-ttu-id="721cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="721cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="721cf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="721cf-127">Request body</span></span>
<span data-ttu-id="721cf-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="721cf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="721cf-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="721cf-129">Response</span></span>
<span data-ttu-id="721cf-130">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="721cf-130">If successful, this method returns a `200 OK` response code and a collection of [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="721cf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="721cf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="721cf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="721cf-132">Request</span></span>
<span data-ttu-id="721cf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="721cf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="721cf-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="721cf-134">Response</span></span>
<span data-ttu-id="721cf-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="721cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1588

{
  "value": [
    {
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
  ]
}
```




