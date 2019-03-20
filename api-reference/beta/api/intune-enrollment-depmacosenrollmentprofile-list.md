---
title: Список Депмакосенроллментпрофилес
description: Список свойств и связей объектов Депмакосенроллментпрофиле.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 503a27afe7d649e51b5194750f3af628d2882518
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572434"
---
# <a name="list-depmacosenrollmentprofiles"></a><span data-ttu-id="2be1c-103">Список Депмакосенроллментпрофилес</span><span class="sxs-lookup"><span data-stu-id="2be1c-103">List depMacOSEnrollmentProfiles</span></span>

> <span data-ttu-id="2be1c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2be1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2be1c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2be1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2be1c-106">Список свойств и связей объектов [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2be1c-106">List properties and relationships of the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2be1c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2be1c-107">Prerequisites</span></span>
<span data-ttu-id="2be1c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2be1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2be1c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2be1c-110">Permission type</span></span>|<span data-ttu-id="2be1c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2be1c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2be1c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2be1c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2be1c-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2be1c-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2be1c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2be1c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2be1c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2be1c-115">Not supported.</span></span>|
|<span data-ttu-id="2be1c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2be1c-116">Application</span></span>|<span data-ttu-id="2be1c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2be1c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2be1c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2be1c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="2be1c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2be1c-119">Request headers</span></span>
|<span data-ttu-id="2be1c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2be1c-120">Header</span></span>|<span data-ttu-id="2be1c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2be1c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2be1c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2be1c-122">Authorization</span></span>|<span data-ttu-id="2be1c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2be1c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2be1c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2be1c-124">Accept</span></span>|<span data-ttu-id="2be1c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2be1c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2be1c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2be1c-126">Request body</span></span>
<span data-ttu-id="2be1c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2be1c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2be1c-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="2be1c-128">Response</span></span>
<span data-ttu-id="2be1c-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [депмакосенроллментпрофиле](../resources/intune-enrollment-depmacosenrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2be1c-129">If successful, this method returns a `200 OK` response code and a collection of [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2be1c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2be1c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2be1c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2be1c-131">Request</span></span>
<span data-ttu-id="2be1c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2be1c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="2be1c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2be1c-133">Response</span></span>
<span data-ttu-id="2be1c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2be1c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1342

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
      "registrationDisabled": true,
      "fileVaultDisabled": true,
      "iCloudDiagnosticsDisabled": true,
      "iCloudStorageDisabled": true,
      "chooseYourLockScreenDisabled": true
    }
  ]
}
```




