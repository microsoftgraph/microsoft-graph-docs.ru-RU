---
title: Get iosUpdateDeviceStatus
description: Чтение свойств и связей объекта iosUpdateDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 792ae2c758f7571fead0104a4957cc6a9c36a570
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137387"
---
# <a name="get-iosupdatedevicestatus"></a><span data-ttu-id="8de82-103">Get iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="8de82-103">Get iosUpdateDeviceStatus</span></span>

<span data-ttu-id="8de82-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8de82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8de82-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8de82-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8de82-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8de82-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8de82-107">Чтение свойств и связей объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="8de82-107">Read properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8de82-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8de82-108">Prerequisites</span></span>
<span data-ttu-id="8de82-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8de82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8de82-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8de82-111">Permission type</span></span>|<span data-ttu-id="8de82-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8de82-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8de82-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8de82-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8de82-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8de82-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8de82-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8de82-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8de82-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8de82-116">Not supported.</span></span>|
|<span data-ttu-id="8de82-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8de82-117">Application</span></span>|<span data-ttu-id="8de82-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8de82-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8de82-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8de82-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8de82-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8de82-120">Optional query parameters</span></span>
<span data-ttu-id="8de82-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8de82-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8de82-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8de82-122">Request headers</span></span>
|<span data-ttu-id="8de82-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8de82-123">Header</span></span>|<span data-ttu-id="8de82-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8de82-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8de82-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8de82-125">Authorization</span></span>|<span data-ttu-id="8de82-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8de82-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8de82-127">Accept</span><span class="sxs-lookup"><span data-stu-id="8de82-127">Accept</span></span>|<span data-ttu-id="8de82-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8de82-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8de82-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8de82-129">Request body</span></span>
<span data-ttu-id="8de82-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8de82-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8de82-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8de82-131">Response</span></span>
<span data-ttu-id="8de82-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8de82-132">If successful, this method returns a `200 OK` response code and [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8de82-133">Пример</span><span class="sxs-lookup"><span data-stu-id="8de82-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8de82-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="8de82-134">Request</span></span>
<span data-ttu-id="8de82-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8de82-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="8de82-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8de82-136">Response</span></span>
<span data-ttu-id="8de82-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8de82-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 666

{
  "value": {
    "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
    "id": "63a79499-9499-63a7-9994-a7639994a763",
    "installStatus": "available",
    "osVersion": "Os Version value",
    "deviceId": "Device Id value",
    "userId": "User Id value",
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




