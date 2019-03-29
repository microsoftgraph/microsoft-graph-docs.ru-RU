---
title: Перечисление объектов sharedPCConfiguration
description: Список свойств и связей объектов sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 25d9fa55ea57f2ee4c1bf858e6a6ccc181dd1987
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980161"
---
# <a name="list-sharedpcconfigurations"></a><span data-ttu-id="0b744-103">Перечисление объектов sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b744-103">List sharedPCConfigurations</span></span>

> <span data-ttu-id="0b744-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b744-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b744-105">Список свойств и связей объектов [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0b744-105">List properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b744-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0b744-106">Prerequisites</span></span>
<span data-ttu-id="0b744-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b744-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b744-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b744-109">Permission type</span></span>|<span data-ttu-id="0b744-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b744-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b744-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b744-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0b744-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b744-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0b744-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b744-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b744-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b744-114">Not supported.</span></span>|
|<span data-ttu-id="0b744-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b744-115">Application</span></span>|<span data-ttu-id="0b744-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b744-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b744-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b744-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0b744-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b744-118">Request headers</span></span>
|<span data-ttu-id="0b744-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b744-119">Header</span></span>|<span data-ttu-id="0b744-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0b744-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b744-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b744-121">Authorization</span></span>|<span data-ttu-id="0b744-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b744-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b744-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0b744-123">Accept</span></span>|<span data-ttu-id="0b744-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0b744-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b744-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b744-125">Request body</span></span>
<span data-ttu-id="0b744-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b744-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b744-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b744-127">Response</span></span>
<span data-ttu-id="0b744-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0b744-128">If successful, this method returns a `200 OK` response code and a collection of [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b744-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0b744-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b744-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b744-130">Request</span></span>
<span data-ttu-id="0b744-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b744-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="0b744-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b744-132">Response</span></span>
<span data-ttu-id="0b744-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b744-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



