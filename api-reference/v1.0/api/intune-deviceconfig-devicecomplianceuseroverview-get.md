---
title: Get deviceComplianceUserOverview
description: Чтение свойств и связей объекта deviceComplianceUserOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b6e830edd53b780972fed6d548f3c4f733fbe116
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972021"
---
# <a name="get-devicecomplianceuseroverview"></a><span data-ttu-id="a931b-103">Get deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="a931b-103">Get deviceComplianceUserOverview</span></span>

> <span data-ttu-id="a931b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a931b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a931b-105">Чтение свойств и связей объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="a931b-105">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a931b-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a931b-106">Prerequisites</span></span>
<span data-ttu-id="a931b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a931b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a931b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a931b-109">Permission type</span></span>|<span data-ttu-id="a931b-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a931b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a931b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a931b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a931b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a931b-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a931b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a931b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a931b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a931b-114">Not supported.</span></span>|
|<span data-ttu-id="a931b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a931b-115">Application</span></span>|<span data-ttu-id="a931b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a931b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a931b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a931b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a931b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a931b-118">Optional query parameters</span></span>
<span data-ttu-id="a931b-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a931b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a931b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a931b-120">Request headers</span></span>
|<span data-ttu-id="a931b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a931b-121">Header</span></span>|<span data-ttu-id="a931b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a931b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a931b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a931b-123">Authorization</span></span>|<span data-ttu-id="a931b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a931b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a931b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a931b-125">Accept</span></span>|<span data-ttu-id="a931b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a931b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a931b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a931b-127">Request body</span></span>
<span data-ttu-id="a931b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a931b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a931b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a931b-129">Response</span></span>
<span data-ttu-id="a931b-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a931b-130">If successful, this method returns a `200 OK` response code and [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a931b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a931b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a931b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a931b-132">Request</span></span>
<span data-ttu-id="a931b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a931b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="a931b-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a931b-134">Response</span></span>
<span data-ttu-id="a931b-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a931b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 365

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
    "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
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



