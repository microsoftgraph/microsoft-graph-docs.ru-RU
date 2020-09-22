---
title: Get deviceConfigurationUserStatus
description: Чтение свойств и связей объекта deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e940369990249fb5fdc9cef213ebcf9b7f903c78
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066847"
---
# <a name="get-deviceconfigurationuserstatus"></a><span data-ttu-id="bc429-103">Get deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="bc429-103">Get deviceConfigurationUserStatus</span></span>

<span data-ttu-id="bc429-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc429-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc429-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc429-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc429-106">Чтение свойств и связей объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="bc429-106">Read properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc429-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bc429-107">Prerequisites</span></span>
<span data-ttu-id="bc429-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc429-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc429-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc429-110">Permission type</span></span>|<span data-ttu-id="bc429-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc429-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc429-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc429-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bc429-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc429-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bc429-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc429-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc429-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc429-115">Not supported.</span></span>|
|<span data-ttu-id="bc429-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc429-116">Application</span></span>|<span data-ttu-id="bc429-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc429-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc429-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc429-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bc429-119">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="bc429-119">Optional query parameters</span></span>
<span data-ttu-id="bc429-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bc429-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc429-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc429-121">Request headers</span></span>
|<span data-ttu-id="bc429-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc429-122">Header</span></span>|<span data-ttu-id="bc429-123">Значение</span><span class="sxs-lookup"><span data-stu-id="bc429-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc429-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc429-124">Authorization</span></span>|<span data-ttu-id="bc429-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc429-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc429-126">Accept</span><span class="sxs-lookup"><span data-stu-id="bc429-126">Accept</span></span>|<span data-ttu-id="bc429-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bc429-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc429-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bc429-128">Request body</span></span>
<span data-ttu-id="bc429-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc429-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc429-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc429-130">Response</span></span>
<span data-ttu-id="bc429-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bc429-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc429-132">Пример</span><span class="sxs-lookup"><span data-stu-id="bc429-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc429-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc429-133">Request</span></span>
<span data-ttu-id="bc429-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc429-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="bc429-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc429-135">Response</span></span>
<span data-ttu-id="bc429-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc429-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
    "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
    "userDisplayName": "User Display Name value",
    "devicesCount": 12,
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```









