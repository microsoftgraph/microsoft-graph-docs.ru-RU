---
title: Get deviceComplianceUserOverview
description: Чтение свойств и связей объекта deviceComplianceUserOverview.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: abaa3315bef477c821f7d00d5abff017f286126c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868910"
---
# <a name="get-devicecomplianceuseroverview"></a><span data-ttu-id="abd39-103">Get deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="abd39-103">Get deviceComplianceUserOverview</span></span>

> <span data-ttu-id="abd39-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="abd39-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abd39-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abd39-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="abd39-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="abd39-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abd39-107">Чтение свойств и связей объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="abd39-107">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="abd39-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="abd39-108">Prerequisites</span></span>
<span data-ttu-id="abd39-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abd39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abd39-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abd39-111">Permission type</span></span>|<span data-ttu-id="abd39-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="abd39-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abd39-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abd39-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abd39-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="abd39-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="abd39-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abd39-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abd39-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abd39-116">Not supported.</span></span>|
|<span data-ttu-id="abd39-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="abd39-117">Application</span></span>|<span data-ttu-id="abd39-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abd39-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abd39-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abd39-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="abd39-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="abd39-120">Optional query parameters</span></span>
<span data-ttu-id="abd39-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="abd39-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="abd39-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abd39-122">Request headers</span></span>
|<span data-ttu-id="abd39-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="abd39-123">Header</span></span>|<span data-ttu-id="abd39-124">Значение</span><span class="sxs-lookup"><span data-stu-id="abd39-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abd39-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="abd39-125">Authorization</span></span>|<span data-ttu-id="abd39-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="abd39-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abd39-127">Accept</span><span class="sxs-lookup"><span data-stu-id="abd39-127">Accept</span></span>|<span data-ttu-id="abd39-128">application/json</span><span class="sxs-lookup"><span data-stu-id="abd39-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abd39-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="abd39-129">Request body</span></span>
<span data-ttu-id="abd39-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="abd39-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abd39-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="abd39-131">Response</span></span>
<span data-ttu-id="abd39-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="abd39-132">If successful, this method returns a `200 OK` response code and [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abd39-133">Пример</span><span class="sxs-lookup"><span data-stu-id="abd39-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="abd39-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="abd39-134">Request</span></span>
<span data-ttu-id="abd39-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="abd39-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="abd39-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="abd39-136">Response</span></span>
<span data-ttu-id="abd39-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="abd39-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





