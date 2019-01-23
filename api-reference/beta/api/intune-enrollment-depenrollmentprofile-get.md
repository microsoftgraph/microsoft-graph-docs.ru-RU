---
title: Получение depEnrollmentProfile
description: Чтение свойства и связи объекта depEnrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 852c13e7dde4fa8f993eb504612fc92992f95869
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418374"
---
# <a name="get-depenrollmentprofile"></a><span data-ttu-id="30193-103">Получение depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="30193-103">Get depEnrollmentProfile</span></span>

> <span data-ttu-id="30193-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="30193-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="30193-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30193-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30193-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30193-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30193-107">Чтение свойства и связи объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="30193-107">Read properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30193-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="30193-108">Prerequisites</span></span>
<span data-ttu-id="30193-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="30193-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="30193-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30193-111">Permission type</span></span>|<span data-ttu-id="30193-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30193-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30193-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30193-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30193-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="30193-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="30193-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30193-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30193-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30193-116">Not supported.</span></span>|
|<span data-ttu-id="30193-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30193-117">Application</span></span>|<span data-ttu-id="30193-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30193-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30193-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30193-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="30193-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="30193-120">Optional query parameters</span></span>
<span data-ttu-id="30193-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="30193-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30193-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30193-122">Request headers</span></span>
|<span data-ttu-id="30193-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30193-123">Header</span></span>|<span data-ttu-id="30193-124">Значение</span><span class="sxs-lookup"><span data-stu-id="30193-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30193-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="30193-125">Authorization</span></span>|<span data-ttu-id="30193-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="30193-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30193-127">Accept</span><span class="sxs-lookup"><span data-stu-id="30193-127">Accept</span></span>|<span data-ttu-id="30193-128">application/json</span><span class="sxs-lookup"><span data-stu-id="30193-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30193-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30193-129">Request body</span></span>
<span data-ttu-id="30193-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30193-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30193-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="30193-131">Response</span></span>
<span data-ttu-id="30193-132">Успешно завершена, этот метод возвращает `200 OK` объект [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="30193-132">If successful, this method returns a `200 OK` response code and [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30193-133">Пример</span><span class="sxs-lookup"><span data-stu-id="30193-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="30193-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="30193-134">Request</span></span>
<span data-ttu-id="30193-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30193-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="30193-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="30193-136">Response</span></span>
<span data-ttu-id="30193-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="30193-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1498

{
  "value": {
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
}
```




