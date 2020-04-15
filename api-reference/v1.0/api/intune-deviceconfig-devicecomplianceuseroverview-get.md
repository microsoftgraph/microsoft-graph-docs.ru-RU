---
title: Get deviceComplianceUserOverview
description: Чтение свойств и связей объекта deviceComplianceUserOverview.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cd1c61cb6e5fc30674ea0bbf1899dae88c9b1203
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43399494"
---
# <a name="get-devicecomplianceuseroverview"></a><span data-ttu-id="4917a-103">Get deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="4917a-103">Get deviceComplianceUserOverview</span></span>

<span data-ttu-id="4917a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4917a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4917a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4917a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4917a-106">Чтение свойств и связей объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="4917a-106">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4917a-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4917a-107">Prerequisites</span></span>
<span data-ttu-id="4917a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4917a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4917a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4917a-110">Permission type</span></span>|<span data-ttu-id="4917a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4917a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4917a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4917a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4917a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4917a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4917a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4917a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4917a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4917a-115">Not supported.</span></span>|
|<span data-ttu-id="4917a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4917a-116">Application</span></span>|<span data-ttu-id="4917a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4917a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4917a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4917a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4917a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4917a-119">Optional query parameters</span></span>
<span data-ttu-id="4917a-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4917a-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4917a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4917a-121">Request headers</span></span>
|<span data-ttu-id="4917a-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4917a-122">Header</span></span>|<span data-ttu-id="4917a-123">Значение</span><span class="sxs-lookup"><span data-stu-id="4917a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4917a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4917a-124">Authorization</span></span>|<span data-ttu-id="4917a-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4917a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4917a-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4917a-126">Accept</span></span>|<span data-ttu-id="4917a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4917a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4917a-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4917a-128">Request body</span></span>
<span data-ttu-id="4917a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4917a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4917a-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="4917a-130">Response</span></span>
<span data-ttu-id="4917a-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4917a-131">If successful, this method returns a `200 OK` response code and [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4917a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4917a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4917a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4917a-133">Request</span></span>
<span data-ttu-id="4917a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4917a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="4917a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4917a-135">Response</span></span>
<span data-ttu-id="4917a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4917a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






