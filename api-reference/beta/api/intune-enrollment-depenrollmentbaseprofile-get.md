---
title: Получить depEnrollmentBaseProfile
description: Чтение свойств и связей объекта depEnrollmentBaseProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ee7a2c421c0e94bb336669829505567a5a242cfd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149928"
---
# <a name="get-depenrollmentbaseprofile"></a><span data-ttu-id="9f26f-103">Получить depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="9f26f-103">Get depEnrollmentBaseProfile</span></span>

<span data-ttu-id="9f26f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f26f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f26f-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f26f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f26f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f26f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f26f-107">Чтение свойств и связей объекта [depEnrollmentBaseProfile.](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9f26f-107">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f26f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9f26f-108">Prerequisites</span></span>
<span data-ttu-id="9f26f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f26f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f26f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f26f-111">Permission type</span></span>|<span data-ttu-id="9f26f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f26f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f26f-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f26f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f26f-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f26f-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9f26f-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f26f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f26f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f26f-116">Not supported.</span></span>|
|<span data-ttu-id="9f26f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9f26f-117">Application</span></span>|<span data-ttu-id="9f26f-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f26f-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f26f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f26f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f26f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9f26f-120">Optional query parameters</span></span>
<span data-ttu-id="9f26f-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9f26f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f26f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f26f-122">Request headers</span></span>
|<span data-ttu-id="9f26f-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f26f-123">Header</span></span>|<span data-ttu-id="9f26f-124">Значение</span><span class="sxs-lookup"><span data-stu-id="9f26f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f26f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f26f-125">Authorization</span></span>|<span data-ttu-id="9f26f-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f26f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f26f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9f26f-127">Accept</span></span>|<span data-ttu-id="9f26f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9f26f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f26f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f26f-129">Request body</span></span>
<span data-ttu-id="9f26f-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f26f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f26f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f26f-131">Response</span></span>
<span data-ttu-id="9f26f-132">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` [объект depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9f26f-132">If successful, this method returns a `200 OK` response code and [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f26f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9f26f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f26f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f26f-134">Request</span></span>
<span data-ttu-id="9f26f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f26f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="9f26f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f26f-136">Response</span></span>
<span data-ttu-id="9f26f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f26f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1151

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
    "configurationWebUrl": true
  }
}
```




