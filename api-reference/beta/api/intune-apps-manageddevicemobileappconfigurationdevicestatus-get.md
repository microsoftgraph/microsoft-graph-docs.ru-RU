---
title: Получение managedDeviceMobileAppConfigurationDeviceStatus
description: Чтение свойств и связей объекта managedDeviceMobileAppConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9cfc8994eac177b1c2e2ac17f9ec8ec24407243
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792225"
---
# <a name="get-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="84b78-103">Получение managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="84b78-103">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="84b78-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84b78-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84b78-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84b78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84b78-106">Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="84b78-106">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84b78-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="84b78-107">Prerequisites</span></span>
<span data-ttu-id="84b78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84b78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84b78-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84b78-110">Permission type</span></span>|<span data-ttu-id="84b78-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="84b78-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84b78-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84b78-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84b78-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="84b78-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="84b78-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84b78-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84b78-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84b78-115">Not supported.</span></span>|
|<span data-ttu-id="84b78-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84b78-116">Application</span></span>|<span data-ttu-id="84b78-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84b78-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84b78-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84b78-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84b78-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="84b78-119">Optional query parameters</span></span>
<span data-ttu-id="84b78-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="84b78-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84b78-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84b78-121">Request headers</span></span>
|<span data-ttu-id="84b78-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84b78-122">Header</span></span>|<span data-ttu-id="84b78-123">Значение</span><span class="sxs-lookup"><span data-stu-id="84b78-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84b78-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84b78-124">Authorization</span></span>|<span data-ttu-id="84b78-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84b78-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84b78-126">Accept</span><span class="sxs-lookup"><span data-stu-id="84b78-126">Accept</span></span>|<span data-ttu-id="84b78-127">application/json</span><span class="sxs-lookup"><span data-stu-id="84b78-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84b78-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84b78-128">Request body</span></span>
<span data-ttu-id="84b78-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84b78-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84b78-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="84b78-130">Response</span></span>
<span data-ttu-id="84b78-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84b78-131">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84b78-132">Пример</span><span class="sxs-lookup"><span data-stu-id="84b78-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="84b78-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="84b78-133">Request</span></span>
<span data-ttu-id="84b78-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84b78-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="84b78-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="84b78-135">Response</span></span>
<span data-ttu-id="84b78-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84b78-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





