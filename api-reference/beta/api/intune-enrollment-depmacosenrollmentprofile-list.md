---
title: Список depMacOSEnrollmentProfiles
description: Свойства списка и связей объектов depMacOSEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 262d17b29bc1dd0c8a0a1a25ec6b077a33be22c2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822479"
---
# <a name="list-depmacosenrollmentprofiles"></a><span data-ttu-id="00039-103">Список depMacOSEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="00039-103">List depMacOSEnrollmentProfiles</span></span>

> <span data-ttu-id="00039-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="00039-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00039-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00039-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00039-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="00039-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00039-107">Свойства списка и связей объектов [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="00039-107">List properties and relationships of the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="00039-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="00039-108">Prerequisites</span></span>
<span data-ttu-id="00039-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00039-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00039-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00039-111">Permission type</span></span>|<span data-ttu-id="00039-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00039-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00039-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00039-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00039-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="00039-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="00039-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00039-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00039-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00039-116">Not supported.</span></span>|
|<span data-ttu-id="00039-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00039-117">Application</span></span>|<span data-ttu-id="00039-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00039-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00039-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00039-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="00039-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00039-120">Request headers</span></span>
|<span data-ttu-id="00039-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00039-121">Header</span></span>|<span data-ttu-id="00039-122">Значение</span><span class="sxs-lookup"><span data-stu-id="00039-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00039-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="00039-123">Authorization</span></span>|<span data-ttu-id="00039-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="00039-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00039-125">Accept</span><span class="sxs-lookup"><span data-stu-id="00039-125">Accept</span></span>|<span data-ttu-id="00039-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00039-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00039-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="00039-127">Request body</span></span>
<span data-ttu-id="00039-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00039-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00039-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="00039-129">Response</span></span>
<span data-ttu-id="00039-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="00039-130">If successful, this method returns a `200 OK` response code and a collection of [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00039-131">Пример</span><span class="sxs-lookup"><span data-stu-id="00039-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="00039-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="00039-132">Request</span></span>
<span data-ttu-id="00039-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00039-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="00039-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="00039-134">Response</span></span>
<span data-ttu-id="00039-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="00039-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1114

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
      "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
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
      "registrationDisabled": true,
      "fileVaultDisabled": true,
      "iCloudDiagnosticsDisabled": true
    }
  ]
}
```





