---
title: Get deviceInstallState
description: Чтение свойств и связей объекта deviceInstallState.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 22c1e5a7f00000f10aa832143eeca8f0b430c571
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354835"
---
# <a name="get-deviceinstallstate"></a><span data-ttu-id="00f56-103">Get deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="00f56-103">Get deviceInstallState</span></span>

> <span data-ttu-id="00f56-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00f56-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00f56-105">Чтение свойств и связей объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="00f56-105">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00f56-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="00f56-106">Prerequisites</span></span>
<span data-ttu-id="00f56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00f56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00f56-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00f56-109">Permission type</span></span>|<span data-ttu-id="00f56-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00f56-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00f56-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00f56-111">Delegated (work or school account)</span></span>|<span data-ttu-id="00f56-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="00f56-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="00f56-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00f56-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00f56-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00f56-114">Not supported.</span></span>|
|<span data-ttu-id="00f56-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00f56-115">Application</span></span>|<span data-ttu-id="00f56-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00f56-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00f56-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00f56-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00f56-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="00f56-118">Optional query parameters</span></span>
<span data-ttu-id="00f56-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="00f56-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00f56-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00f56-120">Request headers</span></span>
|<span data-ttu-id="00f56-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00f56-121">Header</span></span>|<span data-ttu-id="00f56-122">Значение</span><span class="sxs-lookup"><span data-stu-id="00f56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00f56-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00f56-123">Authorization</span></span>|<span data-ttu-id="00f56-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00f56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00f56-125">Accept</span><span class="sxs-lookup"><span data-stu-id="00f56-125">Accept</span></span>|<span data-ttu-id="00f56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00f56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00f56-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00f56-127">Request body</span></span>
<span data-ttu-id="00f56-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00f56-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00f56-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="00f56-129">Response</span></span>
<span data-ttu-id="00f56-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="00f56-130">If successful, this method returns a `200 OK` response code and [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00f56-131">Пример</span><span class="sxs-lookup"><span data-stu-id="00f56-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="00f56-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="00f56-132">Request</span></span>
<span data-ttu-id="00f56-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00f56-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
```

### <a name="response"></a><span data-ttu-id="00f56-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="00f56-134">Response</span></span>
<span data-ttu-id="00f56-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00f56-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




