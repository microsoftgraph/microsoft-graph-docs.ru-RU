---
title: Список Мобилеаппинсталлстатусес
description: Список свойств и связей объектов mobileAppInstallStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8fa0906e1360793554e74703bb591211042732d9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960680"
---
# <a name="list-mobileappinstallstatuses"></a><span data-ttu-id="a0022-103">Список Мобилеаппинсталлстатусес</span><span class="sxs-lookup"><span data-stu-id="a0022-103">List mobileAppInstallStatuses</span></span>

> <span data-ttu-id="a0022-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0022-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0022-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0022-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0022-106">Список свойств и связей объектов [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="a0022-106">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0022-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a0022-107">Prerequisites</span></span>
<span data-ttu-id="a0022-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0022-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0022-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0022-110">Permission type</span></span>|<span data-ttu-id="a0022-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0022-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0022-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0022-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0022-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0022-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a0022-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0022-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0022-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0022-115">Not supported.</span></span>|
|<span data-ttu-id="a0022-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0022-116">Application</span></span>|<span data-ttu-id="a0022-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0022-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0022-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0022-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="a0022-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0022-119">Request headers</span></span>
|<span data-ttu-id="a0022-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a0022-120">Header</span></span>|<span data-ttu-id="a0022-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a0022-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0022-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a0022-122">Authorization</span></span>|<span data-ttu-id="a0022-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a0022-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0022-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a0022-124">Accept</span></span>|<span data-ttu-id="a0022-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a0022-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0022-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a0022-126">Request body</span></span>
<span data-ttu-id="a0022-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0022-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0022-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0022-128">Response</span></span>
<span data-ttu-id="a0022-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a0022-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0022-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a0022-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0022-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0022-131">Request</span></span>
<span data-ttu-id="a0022-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a0022-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="a0022-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0022-133">Response</span></span>
<span data-ttu-id="a0022-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a0022-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





