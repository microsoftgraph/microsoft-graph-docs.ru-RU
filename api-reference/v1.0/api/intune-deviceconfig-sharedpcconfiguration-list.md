---
title: Перечисление объектов sharedPCConfiguration
description: Список свойств и связей объектов sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b97e4cbb7794e6d05082c20de7b7570600a30d01
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814485"
---
# <a name="list-sharedpcconfigurations"></a><span data-ttu-id="97723-103">Перечисление объектов sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="97723-103">List sharedPCConfigurations</span></span>

> <span data-ttu-id="97723-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="97723-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97723-105">Список свойств и связей объектов [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97723-105">List properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="97723-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="97723-106">Prerequisites</span></span>
<span data-ttu-id="97723-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97723-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97723-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97723-109">Permission type</span></span>|<span data-ttu-id="97723-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="97723-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97723-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97723-111">Delegated (work or school account)</span></span>|<span data-ttu-id="97723-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="97723-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="97723-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97723-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97723-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97723-114">Not supported.</span></span>|
|<span data-ttu-id="97723-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97723-115">Application</span></span>|<span data-ttu-id="97723-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97723-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97723-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97723-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="97723-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97723-118">Request headers</span></span>
|<span data-ttu-id="97723-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97723-119">Header</span></span>|<span data-ttu-id="97723-120">Значение</span><span class="sxs-lookup"><span data-stu-id="97723-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97723-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="97723-121">Authorization</span></span>|<span data-ttu-id="97723-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="97723-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97723-123">Accept</span><span class="sxs-lookup"><span data-stu-id="97723-123">Accept</span></span>|<span data-ttu-id="97723-124">application/json</span><span class="sxs-lookup"><span data-stu-id="97723-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97723-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="97723-125">Request body</span></span>
<span data-ttu-id="97723-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="97723-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97723-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="97723-127">Response</span></span>
<span data-ttu-id="97723-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="97723-128">If successful, this method returns a `200 OK` response code and a collection of [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97723-129">Пример</span><span class="sxs-lookup"><span data-stu-id="97723-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="97723-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="97723-130">Request</span></span>
<span data-ttu-id="97723-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97723-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="97723-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="97723-132">Response</span></span>
<span data-ttu-id="97723-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="97723-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



