---
title: Список Депенроллментбасепрофилес
description: Список свойств и связей объектов Депенроллментбасепрофиле.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e3f32d72989ab68ed726b9dc49f7fe0749f68686
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813413"
---
# <a name="list-depenrollmentbaseprofiles"></a><span data-ttu-id="91510-103">Список Депенроллментбасепрофилес</span><span class="sxs-lookup"><span data-stu-id="91510-103">List depEnrollmentBaseProfiles</span></span>

> <span data-ttu-id="91510-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91510-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91510-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91510-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91510-106">Список свойств и связей объектов [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="91510-106">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91510-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="91510-107">Prerequisites</span></span>
<span data-ttu-id="91510-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91510-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91510-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91510-110">Permission type</span></span>|<span data-ttu-id="91510-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="91510-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91510-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91510-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91510-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="91510-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="91510-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91510-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91510-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91510-115">Not supported.</span></span>|
|<span data-ttu-id="91510-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="91510-116">Application</span></span>|<span data-ttu-id="91510-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="91510-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91510-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91510-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="91510-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="91510-119">Request headers</span></span>
|<span data-ttu-id="91510-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="91510-120">Header</span></span>|<span data-ttu-id="91510-121">Значение</span><span class="sxs-lookup"><span data-stu-id="91510-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91510-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="91510-122">Authorization</span></span>|<span data-ttu-id="91510-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91510-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91510-124">Accept</span><span class="sxs-lookup"><span data-stu-id="91510-124">Accept</span></span>|<span data-ttu-id="91510-125">application/json</span><span class="sxs-lookup"><span data-stu-id="91510-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91510-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91510-126">Request body</span></span>
<span data-ttu-id="91510-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91510-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91510-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="91510-128">Response</span></span>
<span data-ttu-id="91510-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="91510-129">If successful, this method returns a `200 OK` response code and a collection of [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91510-130">Пример</span><span class="sxs-lookup"><span data-stu-id="91510-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="91510-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="91510-131">Request</span></span>
<span data-ttu-id="91510-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91510-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="91510-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="91510-133">Response</span></span>
<span data-ttu-id="91510-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="91510-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1281

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depEnrollmentBaseProfile",
      "id": "db378868-8868-db37-6888-37db688837db",
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
      "screenTimeScreenDisabled": true,
      "deviceNameTemplate": "Device Name Template value",
      "configurationWebUrl": true
    }
  ]
}
```




