---
title: Список enrollmentProfiles
description: Список свойств и связей объектов объекта enrollmentprofile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a3588ff0e16008f2a3ed3db35ec2201276f5a79b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466901"
---
# <a name="list-enrollmentprofiles"></a><span data-ttu-id="5e5da-103">Список enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="5e5da-103">List enrollmentProfiles</span></span>

<span data-ttu-id="5e5da-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5e5da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e5da-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e5da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e5da-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e5da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e5da-107">Список свойств и связей объектов [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5e5da-107">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e5da-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5e5da-108">Prerequisites</span></span>
<span data-ttu-id="5e5da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e5da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e5da-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e5da-111">Permission type</span></span>|<span data-ttu-id="5e5da-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e5da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e5da-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e5da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e5da-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e5da-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5e5da-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e5da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e5da-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e5da-116">Not supported.</span></span>|
|<span data-ttu-id="5e5da-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e5da-117">Application</span></span>|<span data-ttu-id="5e5da-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e5da-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e5da-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e5da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="5e5da-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5e5da-120">Request headers</span></span>
|<span data-ttu-id="5e5da-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e5da-121">Header</span></span>|<span data-ttu-id="5e5da-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5e5da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e5da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e5da-123">Authorization</span></span>|<span data-ttu-id="5e5da-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e5da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e5da-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5e5da-125">Accept</span></span>|<span data-ttu-id="5e5da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e5da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e5da-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e5da-127">Request body</span></span>
<span data-ttu-id="5e5da-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5e5da-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e5da-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e5da-129">Response</span></span>
<span data-ttu-id="5e5da-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e5da-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e5da-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5e5da-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e5da-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e5da-132">Request</span></span>
<span data-ttu-id="5e5da-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e5da-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="5e5da-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e5da-134">Response</span></span>
<span data-ttu-id="5e5da-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e5da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





