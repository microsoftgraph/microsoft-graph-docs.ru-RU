---
title: Перечисление объектов sharedPCConfiguration
description: Список свойств и связей объектов sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dec4a087d5d769d4f1fe88fb35924d7320d3b898
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804685"
---
# <a name="list-sharedpcconfigurations"></a><span data-ttu-id="85920-103">Перечисление объектов sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="85920-103">List sharedPCConfigurations</span></span>

> <span data-ttu-id="85920-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85920-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85920-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85920-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85920-106">Список свойств и связей объектов [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85920-106">List properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85920-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="85920-107">Prerequisites</span></span>
<span data-ttu-id="85920-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85920-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85920-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85920-110">Permission type</span></span>|<span data-ttu-id="85920-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85920-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85920-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85920-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85920-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="85920-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="85920-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85920-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85920-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85920-115">Not supported.</span></span>|
|<span data-ttu-id="85920-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85920-116">Application</span></span>|<span data-ttu-id="85920-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85920-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85920-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85920-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="85920-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85920-119">Request headers</span></span>
|<span data-ttu-id="85920-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85920-120">Header</span></span>|<span data-ttu-id="85920-121">Значение</span><span class="sxs-lookup"><span data-stu-id="85920-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85920-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85920-122">Authorization</span></span>|<span data-ttu-id="85920-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85920-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85920-124">Accept</span><span class="sxs-lookup"><span data-stu-id="85920-124">Accept</span></span>|<span data-ttu-id="85920-125">application/json</span><span class="sxs-lookup"><span data-stu-id="85920-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85920-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85920-126">Request body</span></span>
<span data-ttu-id="85920-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85920-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85920-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="85920-128">Response</span></span>
<span data-ttu-id="85920-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85920-129">If successful, this method returns a `200 OK` response code and a collection of [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85920-130">Пример</span><span class="sxs-lookup"><span data-stu-id="85920-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="85920-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="85920-131">Request</span></span>
<span data-ttu-id="85920-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85920-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="85920-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="85920-133">Response</span></span>
<span data-ttu-id="85920-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85920-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1492

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sharedPCConfiguration",
      "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
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
      "allowedAccounts": "guest",
      "localStorage": "enabled",
      "allowLocalStorage": true,
      "setAccountManager": "enabled",
      "disableAccountManager": true,
      "setEduPolicies": "enabled",
      "disableEduPolicies": true,
      "setPowerPolicies": "enabled",
      "disablePowerPolicies": true,
      "signInOnResume": "enabled",
      "disableSignInOnResume": true,
      "enabled": true,
      "idleTimeBeforeSleepInSeconds": 12,
      "kioskAppDisplayName": "Kiosk App Display Name value",
      "kioskAppUserModelId": "Kiosk App User Model Id value",
      "maintenanceStartTime": "11:59:24.7240000",
      "fastFirstSignIn": "enabled"
    }
  ]
}
```





