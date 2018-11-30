---
title: Get sharedPCConfiguration
description: Чтение свойств и связей объекта sharedPCConfiguration.
ms.openlocfilehash: d0b7350441afd582b64bb2854056f2f0fcdee1b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025425"
---
# <a name="get-sharedpcconfiguration"></a><span data-ttu-id="4795a-103">Get sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="4795a-103">Get sharedPCConfiguration</span></span>

> <span data-ttu-id="4795a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4795a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4795a-105">Чтение свойств и связей объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4795a-105">Read properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4795a-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4795a-106">Prerequisites</span></span>
<span data-ttu-id="4795a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4795a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4795a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4795a-109">Permission type</span></span>|<span data-ttu-id="4795a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4795a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4795a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4795a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4795a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4795a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4795a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4795a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4795a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4795a-114">Not supported.</span></span>|
|<span data-ttu-id="4795a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4795a-115">Application</span></span>|<span data-ttu-id="4795a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4795a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4795a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4795a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4795a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4795a-118">Optional query parameters</span></span>
<span data-ttu-id="4795a-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4795a-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4795a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4795a-120">Request headers</span></span>
|<span data-ttu-id="4795a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4795a-121">Header</span></span>|<span data-ttu-id="4795a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4795a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4795a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4795a-123">Authorization</span></span>|<span data-ttu-id="4795a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4795a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4795a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4795a-125">Accept</span></span>|<span data-ttu-id="4795a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4795a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4795a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4795a-127">Request body</span></span>
<span data-ttu-id="4795a-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4795a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4795a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="4795a-129">Response</span></span>
<span data-ttu-id="4795a-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4795a-130">If successful, this method returns a `200 OK` response code and [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4795a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4795a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4795a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4795a-132">Request</span></span>
<span data-ttu-id="4795a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4795a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="4795a-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="4795a-134">Response</span></span>
<span data-ttu-id="4795a-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4795a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



