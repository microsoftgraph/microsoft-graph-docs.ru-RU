---
title: Перечисление объектов deviceConfigurationUserStatus
description: Список свойств и связей объектов deviceConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 80a043a9bd8e90e1c027926fa7bc6ff45b54984d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066826"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="12fc3-103">Перечисление объектов deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="12fc3-103">List deviceConfigurationUserStatuses</span></span>

<span data-ttu-id="12fc3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12fc3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12fc3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12fc3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12fc3-106">Список свойств и связей объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="12fc3-106">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12fc3-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="12fc3-107">Prerequisites</span></span>
<span data-ttu-id="12fc3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12fc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12fc3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12fc3-110">Permission type</span></span>|<span data-ttu-id="12fc3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="12fc3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12fc3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12fc3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12fc3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="12fc3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="12fc3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12fc3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12fc3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12fc3-115">Not supported.</span></span>|
|<span data-ttu-id="12fc3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12fc3-116">Application</span></span>|<span data-ttu-id="12fc3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12fc3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12fc3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12fc3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="12fc3-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="12fc3-119">Request headers</span></span>
|<span data-ttu-id="12fc3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12fc3-120">Header</span></span>|<span data-ttu-id="12fc3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="12fc3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12fc3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="12fc3-122">Authorization</span></span>|<span data-ttu-id="12fc3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12fc3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12fc3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="12fc3-124">Accept</span></span>|<span data-ttu-id="12fc3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12fc3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12fc3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="12fc3-126">Request body</span></span>
<span data-ttu-id="12fc3-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12fc3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12fc3-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="12fc3-128">Response</span></span>
<span data-ttu-id="12fc3-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="12fc3-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12fc3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="12fc3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="12fc3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="12fc3-131">Request</span></span>
<span data-ttu-id="12fc3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12fc3-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="12fc3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="12fc3-133">Response</span></span>
<span data-ttu-id="12fc3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12fc3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
      "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```









