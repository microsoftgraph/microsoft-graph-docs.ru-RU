---
title: Get deviceCompliancePolicyDeviceStateSummary
description: Чтение свойств и связей объекта deviceCompliancePolicyDeviceStateSummary.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1306501b6ea303fd3ff816af4ae0102b17b8cae6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812791"
---
# <a name="get-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="7c6e8-103">Get deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="7c6e8-103">Get deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="7c6e8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7c6e8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7c6e8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c6e8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c6e8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7c6e8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7c6e8-107">Чтение свойств и связей объекта [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7c6e8-107">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7c6e8-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7c6e8-108">Prerequisites</span></span>
<span data-ttu-id="7c6e8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c6e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c6e8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c6e8-111">Permission type</span></span>|<span data-ttu-id="7c6e8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c6e8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c6e8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c6e8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c6e8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c6e8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7c6e8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c6e8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c6e8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c6e8-116">Not supported.</span></span>|
|<span data-ttu-id="7c6e8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c6e8-117">Application</span></span>|<span data-ttu-id="7c6e8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c6e8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c6e8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c6e8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7c6e8-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7c6e8-120">Optional query parameters</span></span>
<span data-ttu-id="7c6e8-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7c6e8-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7c6e8-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c6e8-122">Request headers</span></span>
|<span data-ttu-id="7c6e8-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c6e8-123">Header</span></span>|<span data-ttu-id="7c6e8-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7c6e8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c6e8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c6e8-125">Authorization</span></span>|<span data-ttu-id="7c6e8-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7c6e8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c6e8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7c6e8-127">Accept</span></span>|<span data-ttu-id="7c6e8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7c6e8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c6e8-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7c6e8-129">Request body</span></span>
<span data-ttu-id="7c6e8-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7c6e8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c6e8-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c6e8-131">Response</span></span>
<span data-ttu-id="7c6e8-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7c6e8-132">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c6e8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7c6e8-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="7c6e8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c6e8-134">Request</span></span>
<span data-ttu-id="7c6e8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c6e8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

### <a name="response"></a><span data-ttu-id="7c6e8-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c6e8-136">Response</span></span>
<span data-ttu-id="7c6e8-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7c6e8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





