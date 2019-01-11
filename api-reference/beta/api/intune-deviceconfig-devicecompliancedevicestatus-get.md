---
title: Get deviceComplianceDeviceStatus
description: Чтение свойств и связей объекта deviceComplianceDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7afe90c565f34c2fa19ad0adb5228fa0b22ee8ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848008"
---
# <a name="get-devicecompliancedevicestatus"></a><span data-ttu-id="14bb9-103">Get deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="14bb9-103">Get deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="14bb9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="14bb9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14bb9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14bb9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14bb9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="14bb9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14bb9-107">Чтение свойств и связей объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="14bb9-107">Read properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="14bb9-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="14bb9-108">Prerequisites</span></span>
<span data-ttu-id="14bb9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14bb9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14bb9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14bb9-111">Permission type</span></span>|<span data-ttu-id="14bb9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="14bb9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14bb9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14bb9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14bb9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="14bb9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="14bb9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14bb9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14bb9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14bb9-116">Not supported.</span></span>|
|<span data-ttu-id="14bb9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14bb9-117">Application</span></span>|<span data-ttu-id="14bb9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14bb9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14bb9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14bb9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14bb9-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="14bb9-120">Optional query parameters</span></span>
<span data-ttu-id="14bb9-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="14bb9-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="14bb9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14bb9-122">Request headers</span></span>
|<span data-ttu-id="14bb9-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14bb9-123">Header</span></span>|<span data-ttu-id="14bb9-124">Значение</span><span class="sxs-lookup"><span data-stu-id="14bb9-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14bb9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="14bb9-125">Authorization</span></span>|<span data-ttu-id="14bb9-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="14bb9-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14bb9-127">Accept</span><span class="sxs-lookup"><span data-stu-id="14bb9-127">Accept</span></span>|<span data-ttu-id="14bb9-128">application/json</span><span class="sxs-lookup"><span data-stu-id="14bb9-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14bb9-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="14bb9-129">Request body</span></span>
<span data-ttu-id="14bb9-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="14bb9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14bb9-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="14bb9-131">Response</span></span>
<span data-ttu-id="14bb9-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="14bb9-132">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14bb9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="14bb9-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="14bb9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="14bb9-134">Request</span></span>
<span data-ttu-id="14bb9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14bb9-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="14bb9-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="14bb9-136">Response</span></span>
<span data-ttu-id="14bb9-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="14bb9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 532

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
    "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "platform": 8,
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```





