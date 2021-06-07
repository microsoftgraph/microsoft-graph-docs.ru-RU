---
title: Получение объекта managedAppPolicyDeploymentSummary
description: Чтение свойств и связей объекта managedAppPolicyDeploymentSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 084fee22b4cde69ef41b9179fc7618b23aa88e5c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752597"
---
# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="367fe-103">Получение объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="367fe-103">Get managedAppPolicyDeploymentSummary</span></span>

<span data-ttu-id="367fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="367fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="367fe-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="367fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="367fe-106">Чтение свойств и связей объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="367fe-106">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="367fe-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="367fe-107">Prerequisites</span></span>
<span data-ttu-id="367fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="367fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="367fe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="367fe-110">Permission type</span></span>|<span data-ttu-id="367fe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="367fe-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="367fe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="367fe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="367fe-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="367fe-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="367fe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="367fe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="367fe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="367fe-115">Not supported.</span></span>|
|<span data-ttu-id="367fe-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="367fe-116">Application</span></span>|<span data-ttu-id="367fe-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="367fe-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="367fe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="367fe-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="367fe-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="367fe-119">Optional query parameters</span></span>
<span data-ttu-id="367fe-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="367fe-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="367fe-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="367fe-121">Request headers</span></span>
|<span data-ttu-id="367fe-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="367fe-122">Header</span></span>|<span data-ttu-id="367fe-123">Значение</span><span class="sxs-lookup"><span data-stu-id="367fe-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="367fe-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="367fe-124">Authorization</span></span>|<span data-ttu-id="367fe-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="367fe-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="367fe-126">Accept</span><span class="sxs-lookup"><span data-stu-id="367fe-126">Accept</span></span>|<span data-ttu-id="367fe-127">application/json</span><span class="sxs-lookup"><span data-stu-id="367fe-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="367fe-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="367fe-128">Request body</span></span>
<span data-ttu-id="367fe-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="367fe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="367fe-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="367fe-130">Response</span></span>
<span data-ttu-id="367fe-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="367fe-131">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="367fe-132">Пример</span><span class="sxs-lookup"><span data-stu-id="367fe-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="367fe-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="367fe-133">Request</span></span>
<span data-ttu-id="367fe-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="367fe-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="367fe-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="367fe-135">Response</span></span>
<span data-ttu-id="367fe-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="367fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




