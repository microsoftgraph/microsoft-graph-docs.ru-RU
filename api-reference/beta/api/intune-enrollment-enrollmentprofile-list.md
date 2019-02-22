---
title: Список enrollmentProfiles
description: Список свойств и связей объектов объекта enrollmentprofile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2569a7b762a54b91065fe8e8e842d5a113387252
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167041"
---
# <a name="list-enrollmentprofiles"></a><span data-ttu-id="4b60d-103">Список enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="4b60d-103">List enrollmentProfiles</span></span>

> <span data-ttu-id="4b60d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b60d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b60d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b60d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b60d-106">Список свойств и связей объектов [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4b60d-106">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b60d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4b60d-107">Prerequisites</span></span>
<span data-ttu-id="4b60d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4b60d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4b60d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b60d-110">Permission type</span></span>|<span data-ttu-id="4b60d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b60d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b60d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b60d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b60d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b60d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4b60d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b60d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b60d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b60d-115">Not supported.</span></span>|
|<span data-ttu-id="4b60d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b60d-116">Application</span></span>|<span data-ttu-id="4b60d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b60d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b60d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b60d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="4b60d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b60d-119">Request headers</span></span>
|<span data-ttu-id="4b60d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b60d-120">Header</span></span>|<span data-ttu-id="4b60d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4b60d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b60d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b60d-122">Authorization</span></span>|<span data-ttu-id="4b60d-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4b60d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b60d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4b60d-124">Accept</span></span>|<span data-ttu-id="4b60d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4b60d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b60d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b60d-126">Request body</span></span>
<span data-ttu-id="4b60d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4b60d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b60d-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b60d-128">Response</span></span>
<span data-ttu-id="4b60d-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b60d-129">If successful, this method returns a `200 OK` response code and a collection of [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b60d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4b60d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b60d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b60d-131">Request</span></span>
<span data-ttu-id="4b60d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b60d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="4b60d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b60d-133">Response</span></span>
<span data-ttu-id="4b60d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b60d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




