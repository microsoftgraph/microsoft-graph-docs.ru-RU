---
title: Get deviceConfigurationDeviceStatus
description: Чтение свойств и связей объекта deviceConfigurationDeviceStatus.
author: tfitzmac
ms.openlocfilehash: 8bafdda535bd6737454370bd640efc3c9f7869b1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339272"
---
# <a name="get-deviceconfigurationdevicestatus"></a><span data-ttu-id="2e456-103">Get deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="2e456-103">Get deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="2e456-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2e456-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e456-105">Чтение свойств и связей объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="2e456-105">Read properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2e456-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2e456-106">Prerequisites</span></span>
<span data-ttu-id="2e456-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e456-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e456-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e456-109">Permission type</span></span>|<span data-ttu-id="2e456-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e456-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e456-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e456-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2e456-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e456-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2e456-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e456-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e456-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e456-114">Not supported.</span></span>|
|<span data-ttu-id="2e456-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e456-115">Application</span></span>|<span data-ttu-id="2e456-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e456-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e456-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e456-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2e456-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2e456-118">Optional query parameters</span></span>
<span data-ttu-id="2e456-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2e456-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2e456-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e456-120">Request headers</span></span>
|<span data-ttu-id="2e456-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e456-121">Header</span></span>|<span data-ttu-id="2e456-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2e456-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e456-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e456-123">Authorization</span></span>|<span data-ttu-id="2e456-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2e456-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e456-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2e456-125">Accept</span></span>|<span data-ttu-id="2e456-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2e456-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e456-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e456-127">Request body</span></span>
<span data-ttu-id="2e456-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e456-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e456-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e456-129">Response</span></span>
<span data-ttu-id="2e456-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2e456-130">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e456-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2e456-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="2e456-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e456-132">Request</span></span>
<span data-ttu-id="2e456-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e456-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="2e456-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e456-134">Response</span></span>
<span data-ttu-id="2e456-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2e456-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 515

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
    "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
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



