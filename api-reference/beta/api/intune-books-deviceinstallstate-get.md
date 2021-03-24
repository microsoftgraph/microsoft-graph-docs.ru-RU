---
title: Get deviceInstallState
description: Чтение свойств и связей объекта deviceInstallState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cdfb3c814f29539feae711440ea9c7e1406c6569
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138733"
---
# <a name="get-deviceinstallstate"></a><span data-ttu-id="5115b-103">Get deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="5115b-103">Get deviceInstallState</span></span>

<span data-ttu-id="5115b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5115b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5115b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5115b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5115b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5115b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5115b-107">Чтение свойств и связей объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="5115b-107">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5115b-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5115b-108">Prerequisites</span></span>
<span data-ttu-id="5115b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5115b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5115b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5115b-111">Permission type</span></span>|<span data-ttu-id="5115b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5115b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5115b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5115b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5115b-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5115b-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5115b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5115b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5115b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5115b-116">Not supported.</span></span>|
|<span data-ttu-id="5115b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5115b-117">Application</span></span>|<span data-ttu-id="5115b-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5115b-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5115b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5115b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5115b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5115b-120">Optional query parameters</span></span>
<span data-ttu-id="5115b-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5115b-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5115b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5115b-122">Request headers</span></span>
|<span data-ttu-id="5115b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5115b-123">Header</span></span>|<span data-ttu-id="5115b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5115b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5115b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5115b-125">Authorization</span></span>|<span data-ttu-id="5115b-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5115b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5115b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5115b-127">Accept</span></span>|<span data-ttu-id="5115b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5115b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5115b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5115b-129">Request body</span></span>
<span data-ttu-id="5115b-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5115b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5115b-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="5115b-131">Response</span></span>
<span data-ttu-id="5115b-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5115b-132">If successful, this method returns a `200 OK` response code and [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5115b-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5115b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5115b-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="5115b-134">Request</span></span>
<span data-ttu-id="5115b-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5115b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
```

### <a name="response"></a><span data-ttu-id="5115b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5115b-136">Response</span></span>
<span data-ttu-id="5115b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5115b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 462

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceInstallState",
    "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
    "deviceName": "Device Name value",
    "deviceId": "Device Id value",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "installState": "installed",
    "errorCode": "Error Code value",
    "osVersion": "Os Version value",
    "osDescription": "Os Description value",
    "userName": "User Name value"
  }
}
```




