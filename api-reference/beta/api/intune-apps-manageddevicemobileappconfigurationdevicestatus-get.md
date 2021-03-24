---
title: Get managedDeviceMobileAppConfigurationDeviceStatus
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 720031de811a46a7f580e4e98fd6dbd821812b77
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143600"
---
# <a name="get-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="568d0-103">Get managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="568d0-103">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>

<span data-ttu-id="568d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="568d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="568d0-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="568d0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="568d0-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="568d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="568d0-107">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationDeviceStatus.](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="568d0-107">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="568d0-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="568d0-108">Prerequisites</span></span>
<span data-ttu-id="568d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="568d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="568d0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="568d0-111">Permission type</span></span>|<span data-ttu-id="568d0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="568d0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="568d0-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="568d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="568d0-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="568d0-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="568d0-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="568d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="568d0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="568d0-116">Not supported.</span></span>|
|<span data-ttu-id="568d0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="568d0-117">Application</span></span>|<span data-ttu-id="568d0-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="568d0-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="568d0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="568d0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="568d0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="568d0-120">Optional query parameters</span></span>
<span data-ttu-id="568d0-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="568d0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="568d0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="568d0-122">Request headers</span></span>
|<span data-ttu-id="568d0-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="568d0-123">Header</span></span>|<span data-ttu-id="568d0-124">Значение</span><span class="sxs-lookup"><span data-stu-id="568d0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="568d0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="568d0-125">Authorization</span></span>|<span data-ttu-id="568d0-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="568d0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="568d0-127">Accept</span><span class="sxs-lookup"><span data-stu-id="568d0-127">Accept</span></span>|<span data-ttu-id="568d0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="568d0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="568d0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="568d0-129">Request body</span></span>
<span data-ttu-id="568d0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="568d0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="568d0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="568d0-131">Response</span></span>
<span data-ttu-id="568d0-132">В случае успешной работы этот метод возвращает код ответа и `200 OK` [управляемый объектDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="568d0-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="568d0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="568d0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="568d0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="568d0-134">Request</span></span>
<span data-ttu-id="568d0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="568d0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="568d0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="568d0-136">Response</span></span>
<span data-ttu-id="568d0-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="568d0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




