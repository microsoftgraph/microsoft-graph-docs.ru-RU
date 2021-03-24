---
title: Get deviceComplianceUserStatus
description: Чтение свойств и связей объекта deviceComplianceUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b31b1ac08f51aca9ed8e80fe83256f1f0226cb74
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131787"
---
# <a name="get-devicecomplianceuserstatus"></a><span data-ttu-id="a2a1c-103">Get deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="a2a1c-103">Get deviceComplianceUserStatus</span></span>

<span data-ttu-id="a2a1c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2a1c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2a1c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2a1c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2a1c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2a1c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2a1c-107">Чтение свойств и связей объекта [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a2a1c-107">Read properties and relationships of the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2a1c-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a2a1c-108">Prerequisites</span></span>
<span data-ttu-id="a2a1c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2a1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2a1c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2a1c-111">Permission type</span></span>|<span data-ttu-id="a2a1c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2a1c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2a1c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2a1c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2a1c-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2a1c-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2a1c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2a1c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2a1c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2a1c-116">Not supported.</span></span>|
|<span data-ttu-id="a2a1c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="a2a1c-117">Application</span></span>|<span data-ttu-id="a2a1c-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2a1c-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2a1c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2a1c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a2a1c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a2a1c-120">Optional query parameters</span></span>
<span data-ttu-id="a2a1c-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a2a1c-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a2a1c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2a1c-122">Request headers</span></span>
|<span data-ttu-id="a2a1c-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2a1c-123">Header</span></span>|<span data-ttu-id="a2a1c-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a2a1c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2a1c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2a1c-125">Authorization</span></span>|<span data-ttu-id="a2a1c-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2a1c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2a1c-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a2a1c-127">Accept</span></span>|<span data-ttu-id="a2a1c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a2a1c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2a1c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2a1c-129">Request body</span></span>
<span data-ttu-id="a2a1c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2a1c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2a1c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2a1c-131">Response</span></span>
<span data-ttu-id="a2a1c-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a2a1c-132">If successful, this method returns a `200 OK` response code and [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2a1c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a2a1c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2a1c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2a1c-134">Request</span></span>
<span data-ttu-id="a2a1c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2a1c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

### <a name="response"></a><span data-ttu-id="a2a1c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2a1c-136">Response</span></span>
<span data-ttu-id="a2a1c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a2a1c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 369

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
    "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
    "userDisplayName": "User Display Name value",
    "devicesCount": 12,
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```




