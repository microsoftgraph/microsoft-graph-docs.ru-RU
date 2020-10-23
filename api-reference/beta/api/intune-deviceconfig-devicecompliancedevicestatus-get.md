---
title: Get deviceComplianceDeviceStatus
description: Чтение свойств и связей объекта deviceComplianceDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1c36dcaaf557fcf9c15ab3b654cc078f8f7d3fed
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725178"
---
# <a name="get-devicecompliancedevicestatus"></a><span data-ttu-id="0bb07-103">Get deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="0bb07-103">Get deviceComplianceDeviceStatus</span></span>

<span data-ttu-id="0bb07-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bb07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0bb07-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bb07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bb07-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0bb07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bb07-107">Чтение свойств и связей объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="0bb07-107">Read properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bb07-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0bb07-108">Prerequisites</span></span>
<span data-ttu-id="0bb07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bb07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bb07-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0bb07-111">Permission type</span></span>|<span data-ttu-id="0bb07-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0bb07-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bb07-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0bb07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0bb07-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bb07-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0bb07-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0bb07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bb07-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bb07-116">Not supported.</span></span>|
|<span data-ttu-id="0bb07-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0bb07-117">Application</span></span>|<span data-ttu-id="0bb07-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bb07-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bb07-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0bb07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0bb07-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0bb07-120">Optional query parameters</span></span>
<span data-ttu-id="0bb07-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0bb07-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0bb07-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0bb07-122">Request headers</span></span>
|<span data-ttu-id="0bb07-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0bb07-123">Header</span></span>|<span data-ttu-id="0bb07-124">Значение</span><span class="sxs-lookup"><span data-stu-id="0bb07-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bb07-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0bb07-125">Authorization</span></span>|<span data-ttu-id="0bb07-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0bb07-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bb07-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0bb07-127">Accept</span></span>|<span data-ttu-id="0bb07-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0bb07-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bb07-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0bb07-129">Request body</span></span>
<span data-ttu-id="0bb07-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0bb07-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bb07-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="0bb07-131">Response</span></span>
<span data-ttu-id="0bb07-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0bb07-132">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bb07-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0bb07-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bb07-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bb07-134">Request</span></span>
<span data-ttu-id="0bb07-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0bb07-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="0bb07-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bb07-136">Response</span></span>
<span data-ttu-id="0bb07-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0bb07-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





