---
title: Get deviceConfigurationUserStatus
description: Чтение свойств и связей объекта deviceConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6d08e6346d9ecf97141005c306da76f6d3ff23e9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019060"
---
# <a name="get-deviceconfigurationuserstatus"></a><span data-ttu-id="a10c4-103">Get deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="a10c4-103">Get deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="a10c4-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a10c4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a10c4-105">Чтение свойств и связей объекта [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a10c4-105">Read properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a10c4-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a10c4-106">Prerequisites</span></span>
<span data-ttu-id="a10c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a10c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a10c4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a10c4-109">Permission type</span></span>|<span data-ttu-id="a10c4-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a10c4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a10c4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a10c4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a10c4-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a10c4-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a10c4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a10c4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a10c4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a10c4-114">Not supported.</span></span>|
|<span data-ttu-id="a10c4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a10c4-115">Application</span></span>|<span data-ttu-id="a10c4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a10c4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a10c4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a10c4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a10c4-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a10c4-118">Optional query parameters</span></span>
<span data-ttu-id="a10c4-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a10c4-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a10c4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a10c4-120">Request headers</span></span>
|<span data-ttu-id="a10c4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a10c4-121">Header</span></span>|<span data-ttu-id="a10c4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a10c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a10c4-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a10c4-123">Authorization</span></span>|<span data-ttu-id="a10c4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a10c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a10c4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a10c4-125">Accept</span></span>|<span data-ttu-id="a10c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a10c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a10c4-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a10c4-127">Request body</span></span>
<span data-ttu-id="a10c4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a10c4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a10c4-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a10c4-129">Response</span></span>
<span data-ttu-id="a10c4-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a10c4-130">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a10c4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a10c4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a10c4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a10c4-132">Request</span></span>
<span data-ttu-id="a10c4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a10c4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="a10c4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a10c4-134">Response</span></span>
<span data-ttu-id="a10c4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a10c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
    "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
    "userDisplayName": "User Display Name value",
    "devicesCount": 12,
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```



