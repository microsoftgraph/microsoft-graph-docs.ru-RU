---
title: Перечисление объектов sharedPCConfiguration
description: Список свойств и связей объектов sharedPCConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 93a96bc786302b27b58251c8e5c9231d0e574dd2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514237"
---
# <a name="list-sharedpcconfigurations"></a><span data-ttu-id="fa4c2-103">Перечисление объектов sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="fa4c2-103">List sharedPCConfigurations</span></span>

<span data-ttu-id="fa4c2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa4c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fa4c2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa4c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa4c2-106">Список свойств и связей объектов [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa4c2-106">List properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa4c2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fa4c2-107">Prerequisites</span></span>
<span data-ttu-id="fa4c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa4c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa4c2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa4c2-110">Permission type</span></span>|<span data-ttu-id="fa4c2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa4c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa4c2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa4c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa4c2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa4c2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fa4c2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa4c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa4c2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa4c2-115">Not supported.</span></span>|
|<span data-ttu-id="fa4c2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa4c2-116">Application</span></span>|<span data-ttu-id="fa4c2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa4c2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa4c2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa4c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fa4c2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fa4c2-119">Request headers</span></span>
|<span data-ttu-id="fa4c2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa4c2-120">Header</span></span>|<span data-ttu-id="fa4c2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fa4c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa4c2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa4c2-122">Authorization</span></span>|<span data-ttu-id="fa4c2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa4c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa4c2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fa4c2-124">Accept</span></span>|<span data-ttu-id="fa4c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa4c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa4c2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa4c2-126">Request body</span></span>
<span data-ttu-id="fa4c2-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa4c2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa4c2-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa4c2-128">Response</span></span>
<span data-ttu-id="fa4c2-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa4c2-129">If successful, this method returns a `200 OK` response code and a collection of [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa4c2-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fa4c2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa4c2-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa4c2-131">Request</span></span>
<span data-ttu-id="fa4c2-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa4c2-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="fa4c2-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa4c2-133">Response</span></span>
<span data-ttu-id="fa4c2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa4c2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1165

{
  "value": [
    {
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
  ]
}
```




