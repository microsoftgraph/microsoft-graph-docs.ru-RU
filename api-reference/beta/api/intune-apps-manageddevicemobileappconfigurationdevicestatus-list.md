---
title: Список Манажеддевицемобилеаппконфигуратиондевицестатусес
description: Список свойств и связей объектов managedDeviceMobileAppConfigurationDeviceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 99c34f54bafb6b9fc5e0e18a89e1cc8eb82d93af
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37173040"
---
# <a name="list-manageddevicemobileappconfigurationdevicestatuses"></a><span data-ttu-id="ee72d-103">Список Манажеддевицемобилеаппконфигуратиондевицестатусес</span><span class="sxs-lookup"><span data-stu-id="ee72d-103">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="ee72d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee72d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee72d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ee72d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee72d-106">Список свойств и связей объектов [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="ee72d-106">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee72d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ee72d-107">Prerequisites</span></span>
<span data-ttu-id="ee72d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee72d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee72d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee72d-110">Permission type</span></span>|<span data-ttu-id="ee72d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee72d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee72d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee72d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee72d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee72d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ee72d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee72d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee72d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee72d-115">Not supported.</span></span>|
|<span data-ttu-id="ee72d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee72d-116">Application</span></span>|<span data-ttu-id="ee72d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee72d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee72d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee72d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ee72d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee72d-119">Request headers</span></span>
|<span data-ttu-id="ee72d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee72d-120">Header</span></span>|<span data-ttu-id="ee72d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ee72d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee72d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee72d-122">Authorization</span></span>|<span data-ttu-id="ee72d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee72d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee72d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ee72d-124">Accept</span></span>|<span data-ttu-id="ee72d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee72d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee72d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ee72d-126">Request body</span></span>
<span data-ttu-id="ee72d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee72d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee72d-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ee72d-128">Response</span></span>
<span data-ttu-id="ee72d-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee72d-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee72d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ee72d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee72d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee72d-131">Request</span></span>
<span data-ttu-id="ee72d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee72d-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="ee72d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee72d-133">Response</span></span>
<span data-ttu-id="ee72d-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ee72d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 585

{
  "value": [
    {
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
  ]
}
```




