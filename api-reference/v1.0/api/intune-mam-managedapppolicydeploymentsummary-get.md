---
title: Получение объекта managedAppPolicyDeploymentSummary
description: Чтение свойств и связей объекта managedAppPolicyDeploymentSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b7c3112b5ed3d090bbf5fb92719cd05cb3676412
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967764"
---
# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="bb4db-103">Получение объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="bb4db-103">Get managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="bb4db-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb4db-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb4db-105">Чтение свойств и связей объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="bb4db-105">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb4db-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bb4db-106">Prerequisites</span></span>
<span data-ttu-id="bb4db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb4db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb4db-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb4db-109">Permission type</span></span>|<span data-ttu-id="bb4db-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb4db-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb4db-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb4db-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb4db-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bb4db-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bb4db-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb4db-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb4db-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb4db-114">Not supported.</span></span>|
|<span data-ttu-id="bb4db-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb4db-115">Application</span></span>|<span data-ttu-id="bb4db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb4db-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb4db-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb4db-117">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="bb4db-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bb4db-118">Optional query parameters</span></span>
<span data-ttu-id="bb4db-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bb4db-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb4db-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb4db-120">Request headers</span></span>
|<span data-ttu-id="bb4db-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb4db-121">Header</span></span>|<span data-ttu-id="bb4db-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bb4db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb4db-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb4db-123">Authorization</span></span>|<span data-ttu-id="bb4db-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bb4db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb4db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bb4db-125">Accept</span></span>|<span data-ttu-id="bb4db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb4db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb4db-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb4db-127">Request body</span></span>
<span data-ttu-id="bb4db-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb4db-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb4db-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb4db-129">Response</span></span>
<span data-ttu-id="bb4db-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bb4db-130">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb4db-131">Пример</span><span class="sxs-lookup"><span data-stu-id="bb4db-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb4db-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb4db-132">Request</span></span>
<span data-ttu-id="bb4db-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb4db-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="bb4db-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb4db-134">Response</span></span>
<span data-ttu-id="bb4db-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bb4db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



