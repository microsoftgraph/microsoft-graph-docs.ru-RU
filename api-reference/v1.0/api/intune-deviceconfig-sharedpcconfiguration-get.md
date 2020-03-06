---
title: Get sharedPCConfiguration
description: Чтение свойств и связей объекта sharedPCConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ed5091c48248af42782b50bb324f8e7d2ee46c69
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514244"
---
# <a name="get-sharedpcconfiguration"></a><span data-ttu-id="b907e-103">Get sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="b907e-103">Get sharedPCConfiguration</span></span>

<span data-ttu-id="b907e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b907e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b907e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b907e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b907e-106">Чтение свойств и связей объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b907e-106">Read properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b907e-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b907e-107">Prerequisites</span></span>
<span data-ttu-id="b907e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b907e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b907e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b907e-110">Permission type</span></span>|<span data-ttu-id="b907e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b907e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b907e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b907e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b907e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b907e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b907e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b907e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b907e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b907e-115">Not supported.</span></span>|
|<span data-ttu-id="b907e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b907e-116">Application</span></span>|<span data-ttu-id="b907e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b907e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b907e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b907e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b907e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b907e-119">Optional query parameters</span></span>
<span data-ttu-id="b907e-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b907e-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b907e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b907e-121">Request headers</span></span>
|<span data-ttu-id="b907e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b907e-122">Header</span></span>|<span data-ttu-id="b907e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b907e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b907e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b907e-124">Authorization</span></span>|<span data-ttu-id="b907e-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b907e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b907e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b907e-126">Accept</span></span>|<span data-ttu-id="b907e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b907e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b907e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b907e-128">Request body</span></span>
<span data-ttu-id="b907e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b907e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b907e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b907e-130">Response</span></span>
<span data-ttu-id="b907e-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b907e-131">If successful, this method returns a `200 OK` response code and [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b907e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b907e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b907e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b907e-133">Request</span></span>
<span data-ttu-id="b907e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b907e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b907e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b907e-135">Response</span></span>
<span data-ttu-id="b907e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b907e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1101

{
  "value": {
    "@odata.type": "#microsoft.graph.sharedPCConfiguration",
    "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "accountManagerPolicy": {
      "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
      "accountDeletionPolicy": "diskSpaceThreshold",
      "cacheAccountsAboveDiskFreePercentage": 4,
      "inactiveThresholdDays": 5,
      "removeAccountsBelowDiskFreePercentage": 5
    },
    "allowedAccounts": "domain",
    "allowLocalStorage": true,
    "disableAccountManager": true,
    "disableEduPolicies": true,
    "disablePowerPolicies": true,
    "disableSignInOnResume": true,
    "enabled": true,
    "idleTimeBeforeSleepInSeconds": 12,
    "kioskAppDisplayName": "Kiosk App Display Name value",
    "kioskAppUserModelId": "Kiosk App User Model Id value",
    "maintenanceStartTime": "11:59:24.7240000"
  }
}
```




