---
title: Список enrollmentProfiles
description: Список свойств и связей объектов объекта enrollmentprofile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 369d0f6c2739d7ae5c1c744d60994fc480cf0402
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050439"
---
# <a name="list-enrollmentprofiles"></a><span data-ttu-id="581dd-103">Список enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="581dd-103">List enrollmentProfiles</span></span>

<span data-ttu-id="581dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="581dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="581dd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="581dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="581dd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="581dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="581dd-107">Список свойств и связей объектов [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="581dd-107">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="581dd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="581dd-108">Prerequisites</span></span>
<span data-ttu-id="581dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="581dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="581dd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="581dd-111">Permission type</span></span>|<span data-ttu-id="581dd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="581dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="581dd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="581dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="581dd-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="581dd-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="581dd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="581dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="581dd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="581dd-116">Not supported.</span></span>|
|<span data-ttu-id="581dd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="581dd-117">Application</span></span>|<span data-ttu-id="581dd-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="581dd-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="581dd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="581dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="581dd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="581dd-120">Request headers</span></span>
|<span data-ttu-id="581dd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="581dd-121">Header</span></span>|<span data-ttu-id="581dd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="581dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="581dd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="581dd-123">Authorization</span></span>|<span data-ttu-id="581dd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="581dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="581dd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="581dd-125">Accept</span></span>|<span data-ttu-id="581dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="581dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="581dd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="581dd-127">Request body</span></span>
<span data-ttu-id="581dd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="581dd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="581dd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="581dd-129">Response</span></span>
<span data-ttu-id="581dd-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="581dd-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="581dd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="581dd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="581dd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="581dd-132">Request</span></span>
<span data-ttu-id="581dd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="581dd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="581dd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="581dd-134">Response</span></span>
<span data-ttu-id="581dd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="581dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentProfile",
      "id": "012d8d5e-8d5e-012d-5e8d-2d015e8d2d01",
      "displayName": "Display Name value",
      "description": "Description value",
      "requiresUserAuthentication": true,
      "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
      "enableAuthenticationViaCompanyPortal": true,
      "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
    }
  ]
}
```






