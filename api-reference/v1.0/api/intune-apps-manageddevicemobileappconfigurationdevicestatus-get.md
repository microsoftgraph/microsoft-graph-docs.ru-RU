---
title: Получение managedDeviceMobileAppConfigurationDeviceStatus
description: Чтение свойства и связи объекта managedDeviceMobileAppConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dccd5f0bc51c80f627120d22a314d77b127b6090
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986112"
---
# <a name="get-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="fe0fe-103">Получение managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="fe0fe-103">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="fe0fe-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fe0fe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe0fe-105">Чтение свойства и связи объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="fe0fe-105">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe0fe-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fe0fe-106">Prerequisites</span></span>
<span data-ttu-id="fe0fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe0fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe0fe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe0fe-109">Permission type</span></span>|<span data-ttu-id="fe0fe-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe0fe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe0fe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe0fe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fe0fe-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe0fe-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fe0fe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe0fe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe0fe-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe0fe-114">Not supported.</span></span>|
|<span data-ttu-id="fe0fe-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe0fe-115">Application</span></span>|<span data-ttu-id="fe0fe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe0fe-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe0fe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe0fe-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe0fe-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fe0fe-118">Optional query parameters</span></span>
<span data-ttu-id="fe0fe-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fe0fe-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fe0fe-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe0fe-120">Request headers</span></span>
|<span data-ttu-id="fe0fe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe0fe-121">Header</span></span>|<span data-ttu-id="fe0fe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fe0fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe0fe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe0fe-123">Authorization</span></span>|<span data-ttu-id="fe0fe-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fe0fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe0fe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fe0fe-125">Accept</span></span>|<span data-ttu-id="fe0fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe0fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe0fe-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fe0fe-127">Request body</span></span>
<span data-ttu-id="fe0fe-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe0fe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe0fe-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe0fe-129">Response</span></span>
<span data-ttu-id="fe0fe-130">Успешно завершена, этот метод возвращает `200 OK` объект [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fe0fe-130">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe0fe-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fe0fe-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe0fe-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe0fe-132">Request</span></span>
<span data-ttu-id="fe0fe-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe0fe-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="fe0fe-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe0fe-134">Response</span></span>
<span data-ttu-id="fe0fe-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fe0fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 531

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
    "id": "477d3651-3651-477d-5136-7d4751367d47",
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



