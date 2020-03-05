---
title: Список Мобилеаппинсталлстатусес
description: Список свойств и связей объектов mobileAppInstallStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e1fda233cc8783c9b00e8ff9acd2dbe9f8b9d407
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444961"
---
# <a name="list-mobileappinstallstatuses"></a><span data-ttu-id="9b909-103">Список Мобилеаппинсталлстатусес</span><span class="sxs-lookup"><span data-stu-id="9b909-103">List mobileAppInstallStatuses</span></span>

<span data-ttu-id="9b909-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9b909-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b909-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b909-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b909-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b909-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b909-107">Список свойств и связей объектов [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="9b909-107">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b909-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9b909-108">Prerequisites</span></span>
<span data-ttu-id="9b909-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b909-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b909-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b909-111">Permission type</span></span>|<span data-ttu-id="9b909-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b909-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b909-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b909-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b909-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b909-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9b909-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b909-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b909-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b909-116">Not supported.</span></span>|
|<span data-ttu-id="9b909-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b909-117">Application</span></span>|<span data-ttu-id="9b909-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b909-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b909-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b909-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="9b909-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9b909-120">Request headers</span></span>
|<span data-ttu-id="9b909-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b909-121">Header</span></span>|<span data-ttu-id="9b909-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9b909-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b909-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b909-123">Authorization</span></span>|<span data-ttu-id="9b909-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b909-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b909-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9b909-125">Accept</span></span>|<span data-ttu-id="9b909-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b909-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b909-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b909-127">Request body</span></span>
<span data-ttu-id="9b909-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9b909-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b909-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="9b909-129">Response</span></span>
<span data-ttu-id="9b909-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9b909-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b909-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9b909-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b909-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b909-132">Request</span></span>
<span data-ttu-id="9b909-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b909-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="9b909-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b909-134">Response</span></span>
<span data-ttu-id="9b909-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9b909-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





