---
title: Список Мобилеаппинсталлстатусес
description: Список свойств и связей объектов mobileAppInstallStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e306103da5a8eb4203b3654bd5a5eff808e78cbf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47977175"
---
# <a name="list-mobileappinstallstatuses"></a><span data-ttu-id="e98b0-103">Список Мобилеаппинсталлстатусес</span><span class="sxs-lookup"><span data-stu-id="e98b0-103">List mobileAppInstallStatuses</span></span>

<span data-ttu-id="e98b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e98b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e98b0-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e98b0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e98b0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e98b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e98b0-107">Список свойств и связей объектов [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="e98b0-107">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e98b0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e98b0-108">Prerequisites</span></span>
<span data-ttu-id="e98b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e98b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e98b0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e98b0-111">Permission type</span></span>|<span data-ttu-id="e98b0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e98b0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e98b0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e98b0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e98b0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e98b0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e98b0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e98b0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e98b0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e98b0-116">Not supported.</span></span>|
|<span data-ttu-id="e98b0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e98b0-117">Application</span></span>|<span data-ttu-id="e98b0-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e98b0-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e98b0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e98b0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="e98b0-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e98b0-120">Request headers</span></span>
|<span data-ttu-id="e98b0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e98b0-121">Header</span></span>|<span data-ttu-id="e98b0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e98b0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e98b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e98b0-123">Authorization</span></span>|<span data-ttu-id="e98b0-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e98b0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e98b0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e98b0-125">Accept</span></span>|<span data-ttu-id="e98b0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e98b0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e98b0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e98b0-127">Request body</span></span>
<span data-ttu-id="e98b0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e98b0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e98b0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e98b0-129">Response</span></span>
<span data-ttu-id="e98b0-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e98b0-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e98b0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e98b0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e98b0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e98b0-132">Request</span></span>
<span data-ttu-id="e98b0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e98b0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="e98b0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e98b0-134">Response</span></span>
<span data-ttu-id="e98b0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e98b0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 693

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
      "id": "7560ee45-ee45-7560-45ee-607545ee6075",
      "deviceName": "Device Name value",
      "deviceId": "Device Id value",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "mobileAppInstallStatusValue": "failed",
      "installState": "failed",
      "installStateDetail": "dependencyFailedToInstall",
      "errorCode": 9,
      "osVersion": "Os Version value",
      "osDescription": "Os Description value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "displayVersion": "Display Version value"
    }
  ]
}
```






