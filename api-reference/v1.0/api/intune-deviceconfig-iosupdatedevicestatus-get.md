---
title: Get iosUpdateDeviceStatus
description: Чтение свойств и связей объекта iosUpdateDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5ec6ef635955b0a2124dcc900a4c2c3131572410
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997584"
---
# <a name="get-iosupdatedevicestatus"></a><span data-ttu-id="45f12-103">Get iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="45f12-103">Get iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="45f12-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45f12-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45f12-105">Чтение свойств и связей объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="45f12-105">Read properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45f12-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="45f12-106">Prerequisites</span></span>
<span data-ttu-id="45f12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45f12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45f12-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45f12-109">Permission type</span></span>|<span data-ttu-id="45f12-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45f12-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45f12-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45f12-111">Delegated (work or school account)</span></span>|<span data-ttu-id="45f12-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="45f12-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="45f12-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45f12-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45f12-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45f12-114">Not supported.</span></span>|
|<span data-ttu-id="45f12-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45f12-115">Application</span></span>|<span data-ttu-id="45f12-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45f12-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45f12-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45f12-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45f12-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="45f12-118">Optional query parameters</span></span>
<span data-ttu-id="45f12-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="45f12-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="45f12-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45f12-120">Request headers</span></span>
|<span data-ttu-id="45f12-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45f12-121">Header</span></span>|<span data-ttu-id="45f12-122">Значение</span><span class="sxs-lookup"><span data-stu-id="45f12-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45f12-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45f12-123">Authorization</span></span>|<span data-ttu-id="45f12-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45f12-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45f12-125">Accept</span><span class="sxs-lookup"><span data-stu-id="45f12-125">Accept</span></span>|<span data-ttu-id="45f12-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45f12-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45f12-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45f12-127">Request body</span></span>
<span data-ttu-id="45f12-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="45f12-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45f12-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="45f12-129">Response</span></span>
<span data-ttu-id="45f12-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="45f12-130">If successful, this method returns a `200 OK` response code and [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45f12-131">Пример</span><span class="sxs-lookup"><span data-stu-id="45f12-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="45f12-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="45f12-132">Request</span></span>
<span data-ttu-id="45f12-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45f12-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="45f12-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="45f12-134">Response</span></span>
<span data-ttu-id="45f12-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45f12-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 646

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
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```



