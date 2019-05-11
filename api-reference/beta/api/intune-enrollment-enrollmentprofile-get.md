---
title: Получение объекта enrollmentprofile
description: Чтение свойств и связей объекта объекта enrollmentprofile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d5d58a70429dae06636cb05b53bb2a2cc9fa9992
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908583"
---
# <a name="get-enrollmentprofile"></a><span data-ttu-id="fc649-103">Получение объекта enrollmentprofile</span><span class="sxs-lookup"><span data-stu-id="fc649-103">Get enrollmentProfile</span></span>

> <span data-ttu-id="fc649-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc649-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc649-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc649-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc649-106">Чтение свойств и связей объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="fc649-106">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc649-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fc649-107">Prerequisites</span></span>
<span data-ttu-id="fc649-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc649-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc649-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc649-110">Permission type</span></span>|<span data-ttu-id="fc649-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc649-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc649-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc649-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fc649-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc649-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fc649-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc649-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc649-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc649-115">Not supported.</span></span>|
|<span data-ttu-id="fc649-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc649-116">Application</span></span>|<span data-ttu-id="fc649-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc649-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc649-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc649-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fc649-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fc649-119">Optional query parameters</span></span>
<span data-ttu-id="fc649-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fc649-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc649-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc649-121">Request headers</span></span>
|<span data-ttu-id="fc649-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc649-122">Header</span></span>|<span data-ttu-id="fc649-123">Значение</span><span class="sxs-lookup"><span data-stu-id="fc649-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc649-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc649-124">Authorization</span></span>|<span data-ttu-id="fc649-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc649-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc649-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fc649-126">Accept</span></span>|<span data-ttu-id="fc649-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fc649-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc649-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fc649-128">Request body</span></span>
<span data-ttu-id="fc649-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fc649-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc649-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fc649-130">Response</span></span>
<span data-ttu-id="fc649-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc649-131">If successful, this method returns a `200 OK` response code and [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc649-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fc649-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc649-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc649-133">Request</span></span>
<span data-ttu-id="fc649-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc649-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="fc649-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc649-135">Response</span></span>
<span data-ttu-id="fc649-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc649-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 454

{
  "value": {
    "@odata.type": "#microsoft.graph.enrollmentProfile",
    "id": "012d8d5e-8d5e-012d-5e8d-2d015e8d2d01",
    "displayName": "Display Name value",
    "description": "Description value",
    "requiresUserAuthentication": true,
    "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
    "enableAuthenticationViaCompanyPortal": true,
    "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
  }
}
```




