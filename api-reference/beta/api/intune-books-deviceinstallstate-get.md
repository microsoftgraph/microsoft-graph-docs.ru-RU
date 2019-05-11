---
title: Get deviceInstallState
description: Чтение свойств и связей объекта deviceInstallState.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2ae555e8fcd3fa173fc545e9b89c7f9e3ae73e49
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934357"
---
# <a name="get-deviceinstallstate"></a><span data-ttu-id="ee6b5-103">Get deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="ee6b5-103">Get deviceInstallState</span></span>

> <span data-ttu-id="ee6b5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee6b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee6b5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee6b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee6b5-106">Чтение свойств и связей объекта [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="ee6b5-106">Read properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee6b5-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ee6b5-107">Prerequisites</span></span>
<span data-ttu-id="ee6b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee6b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee6b5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee6b5-110">Permission type</span></span>|<span data-ttu-id="ee6b5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee6b5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee6b5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee6b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee6b5-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee6b5-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ee6b5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee6b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee6b5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee6b5-115">Not supported.</span></span>|
|<span data-ttu-id="ee6b5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee6b5-116">Application</span></span>|<span data-ttu-id="ee6b5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee6b5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee6b5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee6b5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee6b5-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ee6b5-119">Optional query parameters</span></span>
<span data-ttu-id="ee6b5-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ee6b5-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee6b5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee6b5-121">Request headers</span></span>
|<span data-ttu-id="ee6b5-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee6b5-122">Header</span></span>|<span data-ttu-id="ee6b5-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ee6b5-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee6b5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee6b5-124">Authorization</span></span>|<span data-ttu-id="ee6b5-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee6b5-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee6b5-126">Accept</span><span class="sxs-lookup"><span data-stu-id="ee6b5-126">Accept</span></span>|<span data-ttu-id="ee6b5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ee6b5-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee6b5-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ee6b5-128">Request body</span></span>
<span data-ttu-id="ee6b5-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee6b5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee6b5-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee6b5-130">Response</span></span>
<span data-ttu-id="ee6b5-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceInstallState](../resources/intune-books-deviceinstallstate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ee6b5-131">If successful, this method returns a `200 OK` response code and [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee6b5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ee6b5-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee6b5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee6b5-133">Request</span></span>
<span data-ttu-id="ee6b5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee6b5-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
```

### <a name="response"></a><span data-ttu-id="ee6b5-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee6b5-135">Response</span></span>
<span data-ttu-id="ee6b5-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee6b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




