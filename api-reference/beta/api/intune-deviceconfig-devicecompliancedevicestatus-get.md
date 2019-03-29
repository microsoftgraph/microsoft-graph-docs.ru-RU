---
title: Get deviceComplianceDeviceStatus
description: Чтение свойств и связей объекта deviceComplianceDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 35ced522b60462777de79519f3bbae28ecf200e2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961457"
---
# <a name="get-devicecompliancedevicestatus"></a><span data-ttu-id="99e5c-103">Get deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="99e5c-103">Get deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="99e5c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99e5c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99e5c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99e5c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99e5c-106">Чтение свойств и связей объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="99e5c-106">Read properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99e5c-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="99e5c-107">Prerequisites</span></span>
<span data-ttu-id="99e5c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99e5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99e5c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99e5c-110">Permission type</span></span>|<span data-ttu-id="99e5c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="99e5c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99e5c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99e5c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="99e5c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="99e5c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="99e5c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99e5c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99e5c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99e5c-115">Not supported.</span></span>|
|<span data-ttu-id="99e5c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99e5c-116">Application</span></span>|<span data-ttu-id="99e5c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99e5c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99e5c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99e5c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="99e5c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="99e5c-119">Optional query parameters</span></span>
<span data-ttu-id="99e5c-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="99e5c-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="99e5c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99e5c-121">Request headers</span></span>
|<span data-ttu-id="99e5c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="99e5c-122">Header</span></span>|<span data-ttu-id="99e5c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="99e5c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99e5c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99e5c-124">Authorization</span></span>|<span data-ttu-id="99e5c-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99e5c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99e5c-126">Accept</span><span class="sxs-lookup"><span data-stu-id="99e5c-126">Accept</span></span>|<span data-ttu-id="99e5c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="99e5c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99e5c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99e5c-128">Request body</span></span>
<span data-ttu-id="99e5c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="99e5c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99e5c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="99e5c-130">Response</span></span>
<span data-ttu-id="99e5c-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="99e5c-131">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99e5c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="99e5c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="99e5c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="99e5c-133">Request</span></span>
<span data-ttu-id="99e5c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99e5c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="99e5c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="99e5c-135">Response</span></span>
<span data-ttu-id="99e5c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="99e5c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




