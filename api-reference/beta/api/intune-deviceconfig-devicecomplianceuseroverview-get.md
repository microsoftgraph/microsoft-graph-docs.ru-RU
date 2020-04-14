---
title: Get deviceComplianceUserOverview
description: Чтение свойств и связей объекта deviceComplianceUserOverview.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1d006dd45bf1ba3dd02f7504b3b9e6f8be762d7e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433758"
---
# <a name="get-devicecomplianceuseroverview"></a><span data-ttu-id="4a2d5-103">Get deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="4a2d5-103">Get deviceComplianceUserOverview</span></span>

<span data-ttu-id="4a2d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a2d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a2d5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a2d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a2d5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a2d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a2d5-107">Чтение свойств и связей объекта [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="4a2d5-107">Read properties and relationships of the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a2d5-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="4a2d5-108">Prerequisites</span></span>
<span data-ttu-id="4a2d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a2d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a2d5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a2d5-111">Permission type</span></span>|<span data-ttu-id="4a2d5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a2d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a2d5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a2d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a2d5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a2d5-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4a2d5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a2d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a2d5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a2d5-116">Not supported.</span></span>|
|<span data-ttu-id="4a2d5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4a2d5-117">Application</span></span>|<span data-ttu-id="4a2d5-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a2d5-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a2d5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a2d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a2d5-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4a2d5-120">Optional query parameters</span></span>
<span data-ttu-id="4a2d5-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4a2d5-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a2d5-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a2d5-122">Request headers</span></span>
|<span data-ttu-id="4a2d5-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a2d5-123">Header</span></span>|<span data-ttu-id="4a2d5-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4a2d5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a2d5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a2d5-125">Authorization</span></span>|<span data-ttu-id="4a2d5-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a2d5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a2d5-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4a2d5-127">Accept</span></span>|<span data-ttu-id="4a2d5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4a2d5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a2d5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a2d5-129">Request body</span></span>
<span data-ttu-id="4a2d5-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a2d5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a2d5-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a2d5-131">Response</span></span>
<span data-ttu-id="4a2d5-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4a2d5-132">If successful, this method returns a `200 OK` response code and [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a2d5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4a2d5-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a2d5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a2d5-134">Request</span></span>
<span data-ttu-id="4a2d5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a2d5-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

### <a name="response"></a><span data-ttu-id="4a2d5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a2d5-136">Response</span></span>
<span data-ttu-id="4a2d5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a2d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



