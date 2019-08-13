---
title: Get iosUpdateDeviceStatus
description: Чтение свойств и связей объекта iosUpdateDeviceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 974130cee3b3f4084e96379b64930f317bb51f12
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36315696"
---
# <a name="get-iosupdatedevicestatus"></a><span data-ttu-id="7a6b1-103">Get iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="7a6b1-103">Get iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="7a6b1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a6b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a6b1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a6b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a6b1-106">Чтение свойств и связей объекта [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="7a6b1-106">Read properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a6b1-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7a6b1-107">Prerequisites</span></span>
<span data-ttu-id="7a6b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a6b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a6b1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a6b1-110">Permission type</span></span>|<span data-ttu-id="7a6b1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a6b1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a6b1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a6b1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7a6b1-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a6b1-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7a6b1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a6b1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a6b1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a6b1-115">Not supported.</span></span>|
|<span data-ttu-id="7a6b1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a6b1-116">Application</span></span>|<span data-ttu-id="7a6b1-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a6b1-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a6b1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a6b1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a6b1-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7a6b1-119">Optional query parameters</span></span>
<span data-ttu-id="7a6b1-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7a6b1-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a6b1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a6b1-121">Request headers</span></span>
|<span data-ttu-id="7a6b1-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a6b1-122">Header</span></span>|<span data-ttu-id="7a6b1-123">Значение</span><span class="sxs-lookup"><span data-stu-id="7a6b1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a6b1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a6b1-124">Authorization</span></span>|<span data-ttu-id="7a6b1-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a6b1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a6b1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="7a6b1-126">Accept</span></span>|<span data-ttu-id="7a6b1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7a6b1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a6b1-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7a6b1-128">Request body</span></span>
<span data-ttu-id="7a6b1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7a6b1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a6b1-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7a6b1-130">Response</span></span>
<span data-ttu-id="7a6b1-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7a6b1-131">If successful, this method returns a `200 OK` response code and [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a6b1-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7a6b1-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a6b1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a6b1-133">Request</span></span>
<span data-ttu-id="7a6b1-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a6b1-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="7a6b1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a6b1-135">Response</span></span>
<span data-ttu-id="7a6b1-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7a6b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






