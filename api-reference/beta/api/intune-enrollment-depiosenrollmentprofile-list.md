---
title: Список depIOSEnrollmentProfiles
description: Свойства списка и связей объектов depIOSEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ade3539e14d39ba6285662bfa7e876726252c5e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817180"
---
# <a name="list-depiosenrollmentprofiles"></a><span data-ttu-id="477af-103">Список depIOSEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="477af-103">List depIOSEnrollmentProfiles</span></span>

> <span data-ttu-id="477af-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="477af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="477af-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="477af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="477af-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="477af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="477af-107">Свойства списка и связей объектов [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="477af-107">List properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="477af-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="477af-108">Prerequisites</span></span>
<span data-ttu-id="477af-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="477af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="477af-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="477af-111">Permission type</span></span>|<span data-ttu-id="477af-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="477af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="477af-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="477af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="477af-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="477af-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="477af-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="477af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="477af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="477af-116">Not supported.</span></span>|
|<span data-ttu-id="477af-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="477af-117">Application</span></span>|<span data-ttu-id="477af-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="477af-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="477af-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="477af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="477af-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="477af-120">Request headers</span></span>
|<span data-ttu-id="477af-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="477af-121">Header</span></span>|<span data-ttu-id="477af-122">Значение</span><span class="sxs-lookup"><span data-stu-id="477af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="477af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="477af-123">Authorization</span></span>|<span data-ttu-id="477af-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="477af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="477af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="477af-125">Accept</span></span>|<span data-ttu-id="477af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="477af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="477af-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="477af-127">Request body</span></span>
<span data-ttu-id="477af-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="477af-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="477af-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="477af-129">Response</span></span>
<span data-ttu-id="477af-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="477af-130">If successful, this method returns a `200 OK` response code and a collection of [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="477af-131">Пример</span><span class="sxs-lookup"><span data-stu-id="477af-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="477af-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="477af-132">Request</span></span>
<span data-ttu-id="477af-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="477af-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="477af-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="477af-134">Response</span></span>
<span data-ttu-id="477af-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="477af-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1559

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
      "enableSingleAppEnrollmentMode": true
    }
  ]
}
```





