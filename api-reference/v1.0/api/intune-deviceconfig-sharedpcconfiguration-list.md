---
title: Перечисление объектов sharedPCConfiguration
description: Список свойств и связей объектов sharedPCConfiguration.
ms.openlocfilehash: 18cd0562dbb53b796923f76bff5156a306b51962
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024940"
---
# <a name="list-sharedpcconfigurations"></a><span data-ttu-id="ab783-103">Перечисление объектов sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="ab783-103">List sharedPCConfigurations</span></span>

> <span data-ttu-id="ab783-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ab783-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab783-105">Список свойств и связей объектов [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab783-105">List properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab783-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ab783-106">Prerequisites</span></span>
<span data-ttu-id="ab783-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab783-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab783-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab783-109">Permission type</span></span>|<span data-ttu-id="ab783-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab783-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab783-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab783-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ab783-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab783-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ab783-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab783-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab783-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab783-114">Not supported.</span></span>|
|<span data-ttu-id="ab783-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab783-115">Application</span></span>|<span data-ttu-id="ab783-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab783-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab783-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab783-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ab783-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab783-118">Request headers</span></span>
|<span data-ttu-id="ab783-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ab783-119">Header</span></span>|<span data-ttu-id="ab783-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ab783-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab783-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab783-121">Authorization</span></span>|<span data-ttu-id="ab783-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ab783-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab783-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ab783-123">Accept</span></span>|<span data-ttu-id="ab783-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ab783-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab783-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab783-125">Request body</span></span>
<span data-ttu-id="ab783-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab783-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab783-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab783-127">Response</span></span>
<span data-ttu-id="ab783-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ab783-128">If successful, this method returns a `200 OK` response code and a collection of [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab783-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ab783-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab783-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab783-130">Request</span></span>
<span data-ttu-id="ab783-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab783-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ab783-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab783-132">Response</span></span>
<span data-ttu-id="ab783-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ab783-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



