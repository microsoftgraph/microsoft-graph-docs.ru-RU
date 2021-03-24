---
title: Получить depMacOSEnrollmentProfile
description: Чтение свойств и связей объекта depMacOSEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9f056023ab857659094c17a4279091a03e0980a9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145924"
---
# <a name="get-depmacosenrollmentprofile"></a><span data-ttu-id="d04f3-103">Получить depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d04f3-103">Get depMacOSEnrollmentProfile</span></span>

<span data-ttu-id="d04f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d04f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d04f3-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d04f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d04f3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d04f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d04f3-107">Чтение свойств и связей объекта [depMacOSEnrollmentProfile.](../resources/intune-enrollment-depmacosenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d04f3-107">Read properties and relationships of the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d04f3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d04f3-108">Prerequisites</span></span>
<span data-ttu-id="d04f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d04f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d04f3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d04f3-111">Permission type</span></span>|<span data-ttu-id="d04f3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d04f3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d04f3-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d04f3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d04f3-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d04f3-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d04f3-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d04f3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d04f3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d04f3-116">Not supported.</span></span>|
|<span data-ttu-id="d04f3-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d04f3-117">Application</span></span>|<span data-ttu-id="d04f3-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d04f3-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d04f3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d04f3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d04f3-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d04f3-120">Optional query parameters</span></span>
<span data-ttu-id="d04f3-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d04f3-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d04f3-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d04f3-122">Request headers</span></span>
|<span data-ttu-id="d04f3-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d04f3-123">Header</span></span>|<span data-ttu-id="d04f3-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d04f3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d04f3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d04f3-125">Authorization</span></span>|<span data-ttu-id="d04f3-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d04f3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d04f3-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d04f3-127">Accept</span></span>|<span data-ttu-id="d04f3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d04f3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d04f3-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d04f3-129">Request body</span></span>
<span data-ttu-id="d04f3-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d04f3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d04f3-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d04f3-131">Response</span></span>
<span data-ttu-id="d04f3-132">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [объект depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d04f3-132">If successful, this method returns a `200 OK` response code and [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d04f3-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d04f3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d04f3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d04f3-134">Request</span></span>
<span data-ttu-id="d04f3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d04f3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="d04f3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d04f3-136">Response</span></span>
<span data-ttu-id="d04f3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d04f3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1438

{
  "value": {
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
    "isMandatory": true,
    "locationDisabled": true,
    "supportPhoneNumber": "Support Phone Number value",
    "profileRemovalDisabled": true,
    "restoreBlocked": true,
    "appleIdDisabled": true,
    "termsAndConditionsDisabled": true,
    "touchIdDisabled": true,
    "applePayDisabled": true,
    "siriDisabled": true,
    "diagnosticsDisabled": true,
    "displayToneSetupDisabled": true,
    "privacyPaneDisabled": true,
    "screenTimeScreenDisabled": true,
    "deviceNameTemplate": "Device Name Template value",
    "configurationWebUrl": true,
    "registrationDisabled": true,
    "fileVaultDisabled": true,
    "iCloudDiagnosticsDisabled": true,
    "passCodeDisabled": true,
    "zoomDisabled": true,
    "iCloudStorageDisabled": true,
    "chooseYourLockScreenDisabled": true,
    "accessibilityScreenDisabled": true
  }
}
```




