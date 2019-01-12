---
title: Список depEnrollmentProfiles
description: Свойства списка и связей объектов depEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e5b8528991b26237ae665394e37d9e50c2483fe2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975535"
---
# <a name="list-depenrollmentprofiles"></a><span data-ttu-id="14be6-103">Список depEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="14be6-103">List depEnrollmentProfiles</span></span>

> <span data-ttu-id="14be6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="14be6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14be6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14be6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14be6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="14be6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14be6-107">Свойства списка и связей объектов [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="14be6-107">List properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="14be6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="14be6-108">Prerequisites</span></span>
<span data-ttu-id="14be6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14be6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14be6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14be6-111">Permission type</span></span>|<span data-ttu-id="14be6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="14be6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14be6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14be6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14be6-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="14be6-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="14be6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14be6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14be6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14be6-116">Not supported.</span></span>|
|<span data-ttu-id="14be6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14be6-117">Application</span></span>|<span data-ttu-id="14be6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14be6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14be6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14be6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="14be6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14be6-120">Request headers</span></span>
|<span data-ttu-id="14be6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14be6-121">Header</span></span>|<span data-ttu-id="14be6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="14be6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14be6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14be6-123">Authorization</span></span>|<span data-ttu-id="14be6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="14be6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14be6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="14be6-125">Accept</span></span>|<span data-ttu-id="14be6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14be6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14be6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="14be6-127">Request body</span></span>
<span data-ttu-id="14be6-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="14be6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14be6-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="14be6-129">Response</span></span>
<span data-ttu-id="14be6-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="14be6-130">If successful, this method returns a `200 OK` response code and a collection of [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14be6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="14be6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="14be6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="14be6-132">Request</span></span>
<span data-ttu-id="14be6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14be6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="14be6-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="14be6-134">Response</span></span>
<span data-ttu-id="14be6-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="14be6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1520

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





