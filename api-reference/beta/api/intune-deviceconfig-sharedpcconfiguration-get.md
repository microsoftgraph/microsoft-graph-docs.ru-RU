---
title: Get sharedPCConfiguration
description: Чтение свойств и связей объекта sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e8306be137cdbe7ba5fd61665bd7ec495dcc4332
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964146"
---
# <a name="get-sharedpcconfiguration"></a><span data-ttu-id="a2551-103">Get sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="a2551-103">Get sharedPCConfiguration</span></span>

> <span data-ttu-id="a2551-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a2551-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2551-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2551-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2551-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a2551-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2551-107">Чтение свойств и связей объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2551-107">Read properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2551-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a2551-108">Prerequisites</span></span>
<span data-ttu-id="a2551-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2551-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2551-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2551-111">Permission type</span></span>|<span data-ttu-id="a2551-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2551-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2551-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2551-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2551-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2551-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a2551-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2551-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2551-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2551-116">Not supported.</span></span>|
|<span data-ttu-id="a2551-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2551-117">Application</span></span>|<span data-ttu-id="a2551-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2551-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2551-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2551-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2551-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a2551-120">Optional query parameters</span></span>
<span data-ttu-id="a2551-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a2551-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a2551-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2551-122">Request headers</span></span>
|<span data-ttu-id="a2551-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2551-123">Header</span></span>|<span data-ttu-id="a2551-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a2551-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2551-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2551-125">Authorization</span></span>|<span data-ttu-id="a2551-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a2551-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2551-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a2551-127">Accept</span></span>|<span data-ttu-id="a2551-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a2551-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2551-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a2551-129">Request body</span></span>
<span data-ttu-id="a2551-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2551-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2551-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2551-131">Response</span></span>
<span data-ttu-id="a2551-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a2551-132">If successful, this method returns a `200 OK` response code and [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2551-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a2551-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2551-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2551-134">Request</span></span>
<span data-ttu-id="a2551-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2551-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a2551-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2551-136">Response</span></span>
<span data-ttu-id="a2551-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a2551-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1374

{
  "value": {
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
    "allowedAccounts": "domain",
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
    "maintenanceStartTime": "11:59:24.7240000"
  }
}
```





