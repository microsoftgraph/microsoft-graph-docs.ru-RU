---
title: Получение managedDeviceMobileAppConfigurationDeviceStatus
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f763b0a917550127a5cafea2d2362940a6bea356
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43405865"
---
# <a name="get-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="03007-103">Получение managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="03007-103">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>

<span data-ttu-id="03007-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03007-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03007-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03007-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03007-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03007-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03007-107">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="03007-107">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03007-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="03007-108">Prerequisites</span></span>
<span data-ttu-id="03007-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03007-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03007-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03007-111">Permission type</span></span>|<span data-ttu-id="03007-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03007-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03007-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03007-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03007-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="03007-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="03007-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03007-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03007-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03007-116">Not supported.</span></span>|
|<span data-ttu-id="03007-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03007-117">Application</span></span>|<span data-ttu-id="03007-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="03007-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03007-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03007-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="03007-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="03007-120">Optional query parameters</span></span>
<span data-ttu-id="03007-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="03007-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03007-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03007-122">Request headers</span></span>
|<span data-ttu-id="03007-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03007-123">Header</span></span>|<span data-ttu-id="03007-124">Значение</span><span class="sxs-lookup"><span data-stu-id="03007-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03007-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03007-125">Authorization</span></span>|<span data-ttu-id="03007-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03007-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03007-127">Accept</span><span class="sxs-lookup"><span data-stu-id="03007-127">Accept</span></span>|<span data-ttu-id="03007-128">application/json</span><span class="sxs-lookup"><span data-stu-id="03007-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03007-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03007-129">Request body</span></span>
<span data-ttu-id="03007-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03007-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03007-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="03007-131">Response</span></span>
<span data-ttu-id="03007-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03007-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03007-133">Пример</span><span class="sxs-lookup"><span data-stu-id="03007-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="03007-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="03007-134">Request</span></span>
<span data-ttu-id="03007-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03007-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="03007-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="03007-136">Response</span></span>
<span data-ttu-id="03007-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03007-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



