---
title: Получение объекта managedAppPolicyDeploymentSummary
description: Чтение свойств и связей объекта managedAppPolicyDeploymentSummary.
ms.openlocfilehash: 46abf9b5c0eedb8c8990646cf96317a8083e2a21
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082754"
---
# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="9f82b-103">Получение объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="9f82b-103">Get managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="9f82b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9f82b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f82b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f82b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f82b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9f82b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f82b-107">Чтение свойств и связей объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="9f82b-107">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f82b-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9f82b-108">Prerequisites</span></span>
<span data-ttu-id="9f82b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f82b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f82b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f82b-111">Permission type</span></span>|<span data-ttu-id="9f82b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f82b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f82b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f82b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f82b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f82b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9f82b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f82b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f82b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f82b-116">Not supported.</span></span>|
|<span data-ttu-id="9f82b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f82b-117">Application</span></span>|<span data-ttu-id="9f82b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f82b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f82b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f82b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/deploymentSummary
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/deploymentSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f82b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9f82b-120">Optional query parameters</span></span>
<span data-ttu-id="9f82b-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9f82b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9f82b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f82b-122">Request headers</span></span>
|<span data-ttu-id="9f82b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f82b-123">Header</span></span>|<span data-ttu-id="9f82b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="9f82b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f82b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f82b-125">Authorization</span></span>|<span data-ttu-id="9f82b-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9f82b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f82b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9f82b-127">Accept</span></span>|<span data-ttu-id="9f82b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9f82b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f82b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f82b-129">Request body</span></span>
<span data-ttu-id="9f82b-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f82b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f82b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f82b-131">Response</span></span>
<span data-ttu-id="9f82b-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9f82b-132">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f82b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9f82b-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f82b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f82b-134">Request</span></span>
<span data-ttu-id="9f82b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f82b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="9f82b-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f82b-136">Response</span></span>
<span data-ttu-id="9f82b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9f82b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 688

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
    "displayName": "Display Name value",
    "configurationDeployedUserCount": 14,
    "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
    "configurationDeploymentSummaryPerApp": [
      {
        "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
        "mobileAppIdentifier": {
          "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
          "packageId": "Package Id value"
        },
        "configurationAppliedUserCount": 13
      }
    ],
    "id": "61f2f688-f688-61f2-88f6-f26188f6f261",
    "version": "Version value"
  }
}
```





