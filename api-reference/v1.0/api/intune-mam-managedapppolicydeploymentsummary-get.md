---
title: Получение объекта managedAppPolicyDeploymentSummary
description: Чтение свойств и связей объекта managedAppPolicyDeploymentSummary.
author: tfitzmac
ms.openlocfilehash: 8cff2b8b083ede160c56d499d54980507c38fc85
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312098"
---
# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="2b1bb-103">Получение объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="2b1bb-103">Get managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="2b1bb-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2b1bb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b1bb-105">Чтение свойств и связей объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2b1bb-105">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2b1bb-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2b1bb-106">Prerequisites</span></span>
<span data-ttu-id="2b1bb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b1bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b1bb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b1bb-109">Permission type</span></span>|<span data-ttu-id="2b1bb-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b1bb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b1bb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b1bb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2b1bb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b1bb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="2b1bb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b1bb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b1bb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b1bb-114">Not supported.</span></span>|
|<span data-ttu-id="2b1bb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b1bb-115">Application</span></span>|<span data-ttu-id="2b1bb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b1bb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b1bb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b1bb-117">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="2b1bb-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2b1bb-118">Optional query parameters</span></span>
<span data-ttu-id="2b1bb-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2b1bb-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2b1bb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b1bb-120">Request headers</span></span>
|<span data-ttu-id="2b1bb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b1bb-121">Header</span></span>|<span data-ttu-id="2b1bb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2b1bb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b1bb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b1bb-123">Authorization</span></span>|<span data-ttu-id="2b1bb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2b1bb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b1bb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2b1bb-125">Accept</span></span>|<span data-ttu-id="2b1bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b1bb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b1bb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b1bb-127">Request body</span></span>
<span data-ttu-id="2b1bb-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b1bb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b1bb-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b1bb-129">Response</span></span>
<span data-ttu-id="2b1bb-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2b1bb-130">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b1bb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2b1bb-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="2b1bb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b1bb-132">Request</span></span>
<span data-ttu-id="2b1bb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b1bb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="2b1bb-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b1bb-134">Response</span></span>
<span data-ttu-id="2b1bb-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2b1bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



