---
title: Get deviceComplianceUserOverview
description: Чтение свойств и связей объекта deviceComplianceUserOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 87e1a86c89ccbc7186d6ba7c323131a36dae2857
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968948"
---
# <a name="get-devicecomplianceuseroverview"></a><span data-ttu-id="49d23-103">Get deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="49d23-103">Get deviceComplianceUserOverview</span></span>

> <span data-ttu-id="49d23-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="49d23-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49d23-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49d23-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49d23-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="49d23-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49d23-107">Чтение свойств и связей объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="49d23-107">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="49d23-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="49d23-108">Prerequisites</span></span>
<span data-ttu-id="49d23-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49d23-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49d23-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49d23-111">Permission type</span></span>|<span data-ttu-id="49d23-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="49d23-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49d23-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49d23-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49d23-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="49d23-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="49d23-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49d23-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49d23-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49d23-116">Not supported.</span></span>|
|<span data-ttu-id="49d23-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49d23-117">Application</span></span>|<span data-ttu-id="49d23-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49d23-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49d23-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49d23-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49d23-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="49d23-120">Optional query parameters</span></span>
<span data-ttu-id="49d23-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="49d23-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="49d23-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49d23-122">Request headers</span></span>
|<span data-ttu-id="49d23-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="49d23-123">Header</span></span>|<span data-ttu-id="49d23-124">Значение</span><span class="sxs-lookup"><span data-stu-id="49d23-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49d23-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="49d23-125">Authorization</span></span>|<span data-ttu-id="49d23-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="49d23-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49d23-127">Accept</span><span class="sxs-lookup"><span data-stu-id="49d23-127">Accept</span></span>|<span data-ttu-id="49d23-128">application/json</span><span class="sxs-lookup"><span data-stu-id="49d23-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49d23-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="49d23-129">Request body</span></span>
<span data-ttu-id="49d23-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49d23-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49d23-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="49d23-131">Response</span></span>
<span data-ttu-id="49d23-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="49d23-132">If successful, this method returns a `200 OK` response code and [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49d23-133">Пример</span><span class="sxs-lookup"><span data-stu-id="49d23-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="49d23-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="49d23-134">Request</span></span>
<span data-ttu-id="49d23-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49d23-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="49d23-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="49d23-136">Response</span></span>
<span data-ttu-id="49d23-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="49d23-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
    "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```





