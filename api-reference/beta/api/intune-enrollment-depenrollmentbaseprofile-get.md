---
title: Получение Депенроллментбасепрофиле
description: Чтение свойств и связей объекта Депенроллментбасепрофиле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d3c46f8525f5c14eaedb30a15a7dd0a288ad0d4c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35985506"
---
# <a name="get-depenrollmentbaseprofile"></a><span data-ttu-id="cf013-103">Получение Депенроллментбасепрофиле</span><span class="sxs-lookup"><span data-stu-id="cf013-103">Get depEnrollmentBaseProfile</span></span>

> <span data-ttu-id="cf013-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf013-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf013-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf013-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf013-106">Чтение свойств и связей объекта [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="cf013-106">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf013-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cf013-107">Prerequisites</span></span>
<span data-ttu-id="cf013-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf013-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf013-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf013-110">Permission type</span></span>|<span data-ttu-id="cf013-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf013-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf013-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf013-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cf013-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf013-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="cf013-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf013-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf013-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf013-115">Not supported.</span></span>|
|<span data-ttu-id="cf013-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf013-116">Application</span></span>|<span data-ttu-id="cf013-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf013-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf013-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf013-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf013-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cf013-119">Optional query parameters</span></span>
<span data-ttu-id="cf013-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cf013-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf013-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf013-121">Request headers</span></span>
|<span data-ttu-id="cf013-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf013-122">Header</span></span>|<span data-ttu-id="cf013-123">Значение</span><span class="sxs-lookup"><span data-stu-id="cf013-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf013-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cf013-124">Authorization</span></span>|<span data-ttu-id="cf013-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cf013-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf013-126">Accept</span><span class="sxs-lookup"><span data-stu-id="cf013-126">Accept</span></span>|<span data-ttu-id="cf013-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cf013-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf013-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cf013-128">Request body</span></span>
<span data-ttu-id="cf013-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cf013-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf013-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf013-130">Response</span></span>
<span data-ttu-id="cf013-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cf013-131">If successful, this method returns a `200 OK` response code and [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf013-132">Пример</span><span class="sxs-lookup"><span data-stu-id="cf013-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf013-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf013-133">Request</span></span>
<span data-ttu-id="cf013-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf013-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="cf013-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cf013-135">Response</span></span>
<span data-ttu-id="cf013-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cf013-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1136

{
  "value": {
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
    "deviceNameTemplate": "Device Name Template value"
  }
}
```





