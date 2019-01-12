---
title: Get deviceCompliancePolicyDeviceStateSummary
description: Чтение свойств и связей объекта deviceCompliancePolicyDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c8938749e4ca8fa88d724bdb94d3f7bf440cb620
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959883"
---
# <a name="get-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="3fe54-103">Get deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="3fe54-103">Get deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="3fe54-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3fe54-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3fe54-105">Чтение свойств и связей объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3fe54-105">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3fe54-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3fe54-106">Prerequisites</span></span>
<span data-ttu-id="3fe54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fe54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fe54-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fe54-109">Permission type</span></span>|<span data-ttu-id="3fe54-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fe54-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fe54-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fe54-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3fe54-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fe54-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3fe54-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fe54-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fe54-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fe54-114">Not supported.</span></span>|
|<span data-ttu-id="3fe54-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fe54-115">Application</span></span>|<span data-ttu-id="3fe54-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fe54-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fe54-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fe54-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3fe54-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3fe54-118">Optional query parameters</span></span>
<span data-ttu-id="3fe54-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3fe54-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3fe54-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fe54-120">Request headers</span></span>
|<span data-ttu-id="3fe54-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3fe54-121">Header</span></span>|<span data-ttu-id="3fe54-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3fe54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fe54-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fe54-123">Authorization</span></span>|<span data-ttu-id="3fe54-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3fe54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fe54-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3fe54-125">Accept</span></span>|<span data-ttu-id="3fe54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3fe54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fe54-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3fe54-127">Request body</span></span>
<span data-ttu-id="3fe54-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3fe54-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fe54-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="3fe54-129">Response</span></span>
<span data-ttu-id="3fe54-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3fe54-130">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fe54-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3fe54-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="3fe54-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fe54-132">Request</span></span>
<span data-ttu-id="3fe54-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3fe54-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

### <a name="response"></a><span data-ttu-id="3fe54-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="3fe54-134">Response</span></span>
<span data-ttu-id="3fe54-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3fe54-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
    "inGracePeriodCount": 2,
    "configManagerCount": 2,
    "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
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



