---
title: Get deviceConfigurationDeviceOverview
description: Чтение свойств и связей объекта deviceConfigurationDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d70b1f0e8c86b55577304d755624f20d2ee8cfca
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43370393"
---
# <a name="get-deviceconfigurationdeviceoverview"></a><span data-ttu-id="5d426-103">Get deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="5d426-103">Get deviceConfigurationDeviceOverview</span></span>

<span data-ttu-id="5d426-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d426-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d426-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d426-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d426-106">Чтение свойств и связей объекта [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="5d426-106">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d426-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5d426-107">Prerequisites</span></span>
<span data-ttu-id="5d426-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d426-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d426-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d426-110">Permission type</span></span>|<span data-ttu-id="5d426-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d426-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d426-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d426-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5d426-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d426-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5d426-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d426-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d426-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d426-115">Not supported.</span></span>|
|<span data-ttu-id="5d426-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d426-116">Application</span></span>|<span data-ttu-id="5d426-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d426-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d426-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d426-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5d426-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5d426-119">Optional query parameters</span></span>
<span data-ttu-id="5d426-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5d426-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d426-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d426-121">Request headers</span></span>
|<span data-ttu-id="5d426-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5d426-122">Header</span></span>|<span data-ttu-id="5d426-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5d426-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d426-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d426-124">Authorization</span></span>|<span data-ttu-id="5d426-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d426-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d426-126">Accept</span><span class="sxs-lookup"><span data-stu-id="5d426-126">Accept</span></span>|<span data-ttu-id="5d426-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5d426-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d426-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5d426-128">Request body</span></span>
<span data-ttu-id="5d426-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5d426-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d426-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5d426-130">Response</span></span>
<span data-ttu-id="5d426-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5d426-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d426-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5d426-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d426-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d426-133">Request</span></span>
<span data-ttu-id="5d426-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d426-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="5d426-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d426-135">Response</span></span>
<span data-ttu-id="5d426-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5d426-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 370

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
    "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```






