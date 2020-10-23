---
title: Список Депенроллментбасепрофилес
description: Список свойств и связей объектов Депенроллментбасепрофиле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aadd17e4d7cc7d3ed885a1b819bf6f83d3a96955
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726789"
---
# <a name="list-depenrollmentbaseprofiles"></a><span data-ttu-id="57c2f-103">Список Депенроллментбасепрофилес</span><span class="sxs-lookup"><span data-stu-id="57c2f-103">List depEnrollmentBaseProfiles</span></span>

<span data-ttu-id="57c2f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57c2f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57c2f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57c2f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57c2f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="57c2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57c2f-107">Список свойств и связей объектов [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="57c2f-107">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57c2f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="57c2f-108">Prerequisites</span></span>
<span data-ttu-id="57c2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57c2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57c2f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57c2f-111">Permission type</span></span>|<span data-ttu-id="57c2f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="57c2f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57c2f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57c2f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57c2f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="57c2f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="57c2f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57c2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57c2f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57c2f-116">Not supported.</span></span>|
|<span data-ttu-id="57c2f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57c2f-117">Application</span></span>|<span data-ttu-id="57c2f-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="57c2f-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57c2f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57c2f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="57c2f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="57c2f-120">Request headers</span></span>
|<span data-ttu-id="57c2f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57c2f-121">Header</span></span>|<span data-ttu-id="57c2f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="57c2f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57c2f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57c2f-123">Authorization</span></span>|<span data-ttu-id="57c2f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57c2f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57c2f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="57c2f-125">Accept</span></span>|<span data-ttu-id="57c2f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57c2f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57c2f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="57c2f-127">Request body</span></span>
<span data-ttu-id="57c2f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57c2f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57c2f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="57c2f-129">Response</span></span>
<span data-ttu-id="57c2f-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57c2f-130">If successful, this method returns a `200 OK` response code and a collection of [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57c2f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="57c2f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="57c2f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="57c2f-132">Request</span></span>
<span data-ttu-id="57c2f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57c2f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="57c2f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="57c2f-134">Response</span></span>
<span data-ttu-id="57c2f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57c2f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1219

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
  ]
}
```





