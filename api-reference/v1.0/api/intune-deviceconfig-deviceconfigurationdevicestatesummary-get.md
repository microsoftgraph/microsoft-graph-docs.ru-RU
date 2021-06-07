---
title: Получение объекта deviceConfigurationDeviceStateSummary
description: Чтение свойств и связей объекта deviceConfigurationDeviceStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1073f5cf2a4d661293a16b3c79c9ec09c17efc45
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748315"
---
# <a name="get-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="9403d-103">Получение объекта deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="9403d-103">Get deviceConfigurationDeviceStateSummary</span></span>

<span data-ttu-id="9403d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9403d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9403d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9403d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9403d-106">Чтение свойств и связей объекта [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="9403d-106">Read properties and relationships of the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9403d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9403d-107">Prerequisites</span></span>
<span data-ttu-id="9403d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9403d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9403d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9403d-110">Permission type</span></span>|<span data-ttu-id="9403d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9403d-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9403d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9403d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9403d-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9403d-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9403d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9403d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9403d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9403d-115">Not supported.</span></span>|
|<span data-ttu-id="9403d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9403d-116">Application</span></span>|<span data-ttu-id="9403d-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9403d-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9403d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9403d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9403d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9403d-119">Optional query parameters</span></span>
<span data-ttu-id="9403d-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9403d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9403d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9403d-121">Request headers</span></span>
|<span data-ttu-id="9403d-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9403d-122">Header</span></span>|<span data-ttu-id="9403d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9403d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9403d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9403d-124">Authorization</span></span>|<span data-ttu-id="9403d-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9403d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9403d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9403d-126">Accept</span></span>|<span data-ttu-id="9403d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9403d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9403d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9403d-128">Request body</span></span>
<span data-ttu-id="9403d-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9403d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9403d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9403d-130">Response</span></span>
<span data-ttu-id="9403d-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9403d-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9403d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9403d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9403d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9403d-133">Request</span></span>
<span data-ttu-id="9403d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9403d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurationDeviceStateSummaries
```

### <a name="response"></a><span data-ttu-id="9403d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9403d-135">Response</span></span>
<span data-ttu-id="9403d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9403d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 376

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
    "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
    "unknownDeviceCount": 2,
    "notApplicableDeviceCount": 8,
    "compliantDeviceCount": 4,
    "remediatedDeviceCount": 5,
    "nonCompliantDeviceCount": 7,
    "errorDeviceCount": 0,
    "conflictDeviceCount": 3
  }
}
```




