---
title: Получение mobileAppInstallStatus
description: Чтение свойств и связей объекта mobileAppInstallStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b40c8da9172f83840a99c243d50575221f306de3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47977182"
---
# <a name="get-mobileappinstallstatus"></a><span data-ttu-id="13c95-103">Получение mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="13c95-103">Get mobileAppInstallStatus</span></span>

<span data-ttu-id="13c95-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13c95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13c95-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13c95-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13c95-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13c95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13c95-107">Чтение свойств и связей объекта [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) .</span><span class="sxs-lookup"><span data-stu-id="13c95-107">Read properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13c95-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="13c95-108">Prerequisites</span></span>
<span data-ttu-id="13c95-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13c95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13c95-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13c95-111">Permission type</span></span>|<span data-ttu-id="13c95-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="13c95-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13c95-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13c95-113">Delegated (work or school account)</span></span>|<span data-ttu-id="13c95-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="13c95-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="13c95-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13c95-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13c95-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13c95-116">Not supported.</span></span>|
|<span data-ttu-id="13c95-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13c95-117">Application</span></span>|<span data-ttu-id="13c95-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="13c95-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="13c95-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13c95-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13c95-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="13c95-120">Optional query parameters</span></span>
<span data-ttu-id="13c95-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="13c95-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13c95-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13c95-122">Request headers</span></span>
|<span data-ttu-id="13c95-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13c95-123">Header</span></span>|<span data-ttu-id="13c95-124">Значение</span><span class="sxs-lookup"><span data-stu-id="13c95-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13c95-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="13c95-125">Authorization</span></span>|<span data-ttu-id="13c95-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13c95-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13c95-127">Accept</span><span class="sxs-lookup"><span data-stu-id="13c95-127">Accept</span></span>|<span data-ttu-id="13c95-128">application/json</span><span class="sxs-lookup"><span data-stu-id="13c95-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13c95-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="13c95-129">Request body</span></span>
<span data-ttu-id="13c95-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13c95-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13c95-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="13c95-131">Response</span></span>
<span data-ttu-id="13c95-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="13c95-132">If successful, this method returns a `200 OK` response code and [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13c95-133">Пример</span><span class="sxs-lookup"><span data-stu-id="13c95-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="13c95-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="13c95-134">Request</span></span>
<span data-ttu-id="13c95-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13c95-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
```

### <a name="response"></a><span data-ttu-id="13c95-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="13c95-136">Response</span></span>
<span data-ttu-id="13c95-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="13c95-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 651

{
  "value": {
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
}
```






