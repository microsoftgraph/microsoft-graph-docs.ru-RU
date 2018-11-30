---
title: Get iosUpdateDeviceStatus
description: Чтение свойств и связей объекта iosUpdateDeviceStatus.
ms.openlocfilehash: c3dfa05f05ae0a3d7694c60a93e65529f698db95
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024565"
---
# <a name="get-iosupdatedevicestatus"></a><span data-ttu-id="f64db-103">Get iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="f64db-103">Get iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="f64db-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f64db-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f64db-105">Чтение свойств и связей объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="f64db-105">Read properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f64db-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f64db-106">Prerequisites</span></span>
<span data-ttu-id="f64db-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f64db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f64db-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f64db-109">Permission type</span></span>|<span data-ttu-id="f64db-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f64db-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f64db-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f64db-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f64db-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f64db-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f64db-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f64db-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f64db-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f64db-114">Not supported.</span></span>|
|<span data-ttu-id="f64db-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f64db-115">Application</span></span>|<span data-ttu-id="f64db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f64db-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f64db-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f64db-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f64db-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f64db-118">Optional query parameters</span></span>
<span data-ttu-id="f64db-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f64db-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f64db-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f64db-120">Request headers</span></span>
|<span data-ttu-id="f64db-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f64db-121">Header</span></span>|<span data-ttu-id="f64db-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f64db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f64db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f64db-123">Authorization</span></span>|<span data-ttu-id="f64db-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f64db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f64db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f64db-125">Accept</span></span>|<span data-ttu-id="f64db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f64db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f64db-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f64db-127">Request body</span></span>
<span data-ttu-id="f64db-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f64db-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f64db-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f64db-129">Response</span></span>
<span data-ttu-id="f64db-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f64db-130">If successful, this method returns a `200 OK` response code and [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f64db-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f64db-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f64db-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f64db-132">Request</span></span>
<span data-ttu-id="f64db-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f64db-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="f64db-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="f64db-134">Response</span></span>
<span data-ttu-id="f64db-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f64db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



