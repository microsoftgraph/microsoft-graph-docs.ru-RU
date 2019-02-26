---
title: Получение объекта managedAppPolicyDeploymentSummary
description: Чтение свойств и связей объекта managedAppPolicyDeploymentSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5fda5e69925d7541df62a8747d8e0cb55db51a0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250126"
---
# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="028f0-103">Получение объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="028f0-103">Get managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="028f0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="028f0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="028f0-105">Чтение свойств и связей объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="028f0-105">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="028f0-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="028f0-106">Prerequisites</span></span>
<span data-ttu-id="028f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="028f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="028f0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="028f0-109">Permission type</span></span>|<span data-ttu-id="028f0-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="028f0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="028f0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="028f0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="028f0-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="028f0-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="028f0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="028f0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="028f0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="028f0-114">Not supported.</span></span>|
|<span data-ttu-id="028f0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="028f0-115">Application</span></span>|<span data-ttu-id="028f0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="028f0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="028f0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="028f0-117">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="028f0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="028f0-118">Optional query parameters</span></span>
<span data-ttu-id="028f0-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="028f0-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="028f0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="028f0-120">Request headers</span></span>
|<span data-ttu-id="028f0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="028f0-121">Header</span></span>|<span data-ttu-id="028f0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="028f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="028f0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="028f0-123">Authorization</span></span>|<span data-ttu-id="028f0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="028f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="028f0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="028f0-125">Accept</span></span>|<span data-ttu-id="028f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="028f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="028f0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="028f0-127">Request body</span></span>
<span data-ttu-id="028f0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="028f0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="028f0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="028f0-129">Response</span></span>
<span data-ttu-id="028f0-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="028f0-130">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="028f0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="028f0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="028f0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="028f0-132">Request</span></span>
<span data-ttu-id="028f0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="028f0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="028f0-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="028f0-134">Response</span></span>
<span data-ttu-id="028f0-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="028f0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



