---
title: Получение managedDeviceMobileAppConfigurationDeviceStatus
description: Чтение свойства и связи объекта managedDeviceMobileAppConfigurationDeviceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 861fb5694450c795fc8b74970b41e704e4b9a05d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417555"
---
# <a name="get-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="4dbdc-103">Получение managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="4dbdc-103">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="4dbdc-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4dbdc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4dbdc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dbdc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4dbdc-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4dbdc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dbdc-107">Чтение свойства и связи объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="4dbdc-107">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4dbdc-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="4dbdc-108">Prerequisites</span></span>
<span data-ttu-id="4dbdc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4dbdc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4dbdc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4dbdc-111">Permission type</span></span>|<span data-ttu-id="4dbdc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4dbdc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dbdc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4dbdc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4dbdc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4dbdc-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4dbdc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4dbdc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dbdc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dbdc-116">Not supported.</span></span>|
|<span data-ttu-id="4dbdc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4dbdc-117">Application</span></span>|<span data-ttu-id="4dbdc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dbdc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dbdc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4dbdc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4dbdc-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4dbdc-120">Optional query parameters</span></span>
<span data-ttu-id="4dbdc-121">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4dbdc-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4dbdc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4dbdc-122">Request headers</span></span>
|<span data-ttu-id="4dbdc-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4dbdc-123">Header</span></span>|<span data-ttu-id="4dbdc-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4dbdc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4dbdc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4dbdc-125">Authorization</span></span>|<span data-ttu-id="4dbdc-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4dbdc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4dbdc-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4dbdc-127">Accept</span></span>|<span data-ttu-id="4dbdc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4dbdc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dbdc-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4dbdc-129">Request body</span></span>
<span data-ttu-id="4dbdc-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4dbdc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4dbdc-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dbdc-131">Response</span></span>
<span data-ttu-id="4dbdc-132">Успешно завершена, этот метод возвращает `200 OK` объект [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4dbdc-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dbdc-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4dbdc-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4dbdc-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4dbdc-134">Request</span></span>
<span data-ttu-id="4dbdc-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4dbdc-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="4dbdc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4dbdc-136">Response</span></span>
<span data-ttu-id="4dbdc-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4dbdc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 551

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
    "id": "477d3651-3651-477d-5136-7d4751367d47",
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




