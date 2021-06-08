---
title: Get deviceConfigurationUserStatus
description: Чтение свойств и связей объекта deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d559c38da606d87f9762784fed4c1077fa2be017
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760617"
---
# <a name="get-deviceconfigurationuserstatus"></a><span data-ttu-id="0ee6b-103">Get deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="0ee6b-103">Get deviceConfigurationUserStatus</span></span>

<span data-ttu-id="0ee6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ee6b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0ee6b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ee6b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ee6b-106">Чтение свойств и связей объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="0ee6b-106">Read properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ee6b-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0ee6b-107">Prerequisites</span></span>
<span data-ttu-id="0ee6b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ee6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ee6b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ee6b-110">Permission type</span></span>|<span data-ttu-id="0ee6b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ee6b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ee6b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ee6b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ee6b-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ee6b-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ee6b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ee6b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ee6b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ee6b-115">Not supported.</span></span>|
|<span data-ttu-id="0ee6b-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0ee6b-116">Application</span></span>|<span data-ttu-id="0ee6b-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ee6b-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ee6b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ee6b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ee6b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0ee6b-119">Optional query parameters</span></span>
<span data-ttu-id="0ee6b-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0ee6b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ee6b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ee6b-121">Request headers</span></span>
|<span data-ttu-id="0ee6b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ee6b-122">Header</span></span>|<span data-ttu-id="0ee6b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="0ee6b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ee6b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ee6b-124">Authorization</span></span>|<span data-ttu-id="0ee6b-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ee6b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ee6b-126">Accept</span><span class="sxs-lookup"><span data-stu-id="0ee6b-126">Accept</span></span>|<span data-ttu-id="0ee6b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0ee6b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ee6b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ee6b-128">Request body</span></span>
<span data-ttu-id="0ee6b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ee6b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ee6b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ee6b-130">Response</span></span>
<span data-ttu-id="0ee6b-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0ee6b-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ee6b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0ee6b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ee6b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ee6b-133">Request</span></span>
<span data-ttu-id="0ee6b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ee6b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="0ee6b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ee6b-135">Response</span></span>
<span data-ttu-id="0ee6b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ee6b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




