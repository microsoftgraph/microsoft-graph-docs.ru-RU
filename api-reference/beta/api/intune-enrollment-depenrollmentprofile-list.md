---
title: Список Депенроллментпрофилес
description: Список свойств и связей объектов depEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fe781f69ed50f4f6d206f53030f7d232cc67951b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467251"
---
# <a name="list-depenrollmentprofiles"></a><span data-ttu-id="03458-103">Список Депенроллментпрофилес</span><span class="sxs-lookup"><span data-stu-id="03458-103">List depEnrollmentProfiles</span></span>

<span data-ttu-id="03458-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="03458-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03458-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03458-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03458-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03458-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03458-107">Список свойств и связей объектов [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="03458-107">List properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03458-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="03458-108">Prerequisites</span></span>
<span data-ttu-id="03458-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03458-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03458-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03458-111">Permission type</span></span>|<span data-ttu-id="03458-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03458-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03458-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03458-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03458-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="03458-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="03458-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03458-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03458-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03458-116">Not supported.</span></span>|
|<span data-ttu-id="03458-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03458-117">Application</span></span>|<span data-ttu-id="03458-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="03458-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03458-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03458-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="03458-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="03458-120">Request headers</span></span>
|<span data-ttu-id="03458-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03458-121">Header</span></span>|<span data-ttu-id="03458-122">Значение</span><span class="sxs-lookup"><span data-stu-id="03458-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03458-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03458-123">Authorization</span></span>|<span data-ttu-id="03458-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03458-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03458-125">Accept</span><span class="sxs-lookup"><span data-stu-id="03458-125">Accept</span></span>|<span data-ttu-id="03458-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03458-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03458-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03458-127">Request body</span></span>
<span data-ttu-id="03458-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03458-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03458-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="03458-129">Response</span></span>
<span data-ttu-id="03458-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03458-130">If successful, this method returns a `200 OK` response code and a collection of [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03458-131">Пример</span><span class="sxs-lookup"><span data-stu-id="03458-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="03458-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="03458-132">Request</span></span>
<span data-ttu-id="03458-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03458-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="03458-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="03458-134">Response</span></span>
<span data-ttu-id="03458-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03458-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





