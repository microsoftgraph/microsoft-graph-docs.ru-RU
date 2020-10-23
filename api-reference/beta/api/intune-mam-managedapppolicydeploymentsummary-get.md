---
title: Получение объекта managedAppPolicyDeploymentSummary
description: Чтение свойств и связей объекта managedAppPolicyDeploymentSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f2d7e48d7a835bd4f2c7e37849d6c6ab44c0f550
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701741"
---
# <a name="get-managedapppolicydeploymentsummary"></a><span data-ttu-id="e6aa8-103">Получение объекта managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="e6aa8-103">Get managedAppPolicyDeploymentSummary</span></span>

<span data-ttu-id="e6aa8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6aa8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6aa8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6aa8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6aa8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6aa8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6aa8-107">Чтение свойств и связей объекта [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="e6aa8-107">Read properties and relationships of the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6aa8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e6aa8-108">Prerequisites</span></span>
<span data-ttu-id="e6aa8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6aa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6aa8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6aa8-111">Permission type</span></span>|<span data-ttu-id="e6aa8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6aa8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6aa8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6aa8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6aa8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6aa8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e6aa8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6aa8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6aa8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6aa8-116">Not supported.</span></span>|
|<span data-ttu-id="e6aa8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6aa8-117">Application</span></span>|<span data-ttu-id="e6aa8-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e6aa8-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6aa8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6aa8-119">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="e6aa8-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e6aa8-120">Optional query parameters</span></span>
<span data-ttu-id="e6aa8-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e6aa8-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e6aa8-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6aa8-122">Request headers</span></span>
|<span data-ttu-id="e6aa8-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6aa8-123">Header</span></span>|<span data-ttu-id="e6aa8-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e6aa8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6aa8-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6aa8-125">Authorization</span></span>|<span data-ttu-id="e6aa8-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6aa8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6aa8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e6aa8-127">Accept</span></span>|<span data-ttu-id="e6aa8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e6aa8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6aa8-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e6aa8-129">Request body</span></span>
<span data-ttu-id="e6aa8-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6aa8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6aa8-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6aa8-131">Response</span></span>
<span data-ttu-id="e6aa8-132">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e6aa8-132">If successful, this method returns a `200 OK` response code and [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6aa8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e6aa8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6aa8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6aa8-134">Request</span></span>
<span data-ttu-id="e6aa8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6aa8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
```

### <a name="response"></a><span data-ttu-id="e6aa8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6aa8-136">Response</span></span>
<span data-ttu-id="e6aa8-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6aa8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





