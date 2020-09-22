---
title: Получение объекта managedAppPolicyDeploymentSummary
description: Чтение свойств и связей объекта managedAppPolicyDeploymentSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0882122571cf1a1413eef25b0bd7e17f1e7e01b5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984994"
---
# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="a7707-103">Получение объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="a7707-103">Get managedAppPolicyDeploymentSummary</span></span>

<span data-ttu-id="a7707-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7707-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7707-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7707-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7707-106">Чтение свойств и связей объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="a7707-106">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7707-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a7707-107">Prerequisites</span></span>
<span data-ttu-id="a7707-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7707-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7707-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7707-110">Permission type</span></span>|<span data-ttu-id="a7707-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7707-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7707-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7707-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a7707-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7707-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a7707-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7707-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7707-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7707-115">Not supported.</span></span>|
|<span data-ttu-id="a7707-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7707-116">Application</span></span>|<span data-ttu-id="a7707-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7707-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7707-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7707-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="a7707-119">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="a7707-119">Optional query parameters</span></span>
<span data-ttu-id="a7707-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a7707-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7707-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7707-121">Request headers</span></span>
|<span data-ttu-id="a7707-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7707-122">Header</span></span>|<span data-ttu-id="a7707-123">Значение</span><span class="sxs-lookup"><span data-stu-id="a7707-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7707-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7707-124">Authorization</span></span>|<span data-ttu-id="a7707-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7707-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7707-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a7707-126">Accept</span></span>|<span data-ttu-id="a7707-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a7707-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7707-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a7707-128">Request body</span></span>
<span data-ttu-id="a7707-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7707-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7707-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7707-130">Response</span></span>
<span data-ttu-id="a7707-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a7707-131">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7707-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a7707-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7707-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7707-133">Request</span></span>
<span data-ttu-id="a7707-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7707-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="a7707-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7707-135">Response</span></span>
<span data-ttu-id="a7707-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7707-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









