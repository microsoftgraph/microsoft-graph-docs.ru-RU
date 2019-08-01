---
title: Список Манажеддевицемобилеаппконфигуратиондевицестатусес
description: Список свойств и связей объектов managedDeviceMobileAppConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d6223e89e4ee59d2975fc68f55542d108f06abd0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014013"
---
# <a name="list-manageddevicemobileappconfigurationdevicestatuses"></a><span data-ttu-id="9db19-103">Список Манажеддевицемобилеаппконфигуратиондевицестатусес</span><span class="sxs-lookup"><span data-stu-id="9db19-103">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="9db19-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9db19-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9db19-105">Список свойств и связей объектов [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="9db19-105">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9db19-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9db19-106">Prerequisites</span></span>
<span data-ttu-id="9db19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9db19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9db19-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9db19-109">Permission type</span></span>|<span data-ttu-id="9db19-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9db19-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9db19-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9db19-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9db19-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9db19-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9db19-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9db19-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9db19-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9db19-114">Not supported.</span></span>|
|<span data-ttu-id="9db19-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9db19-115">Application</span></span>|<span data-ttu-id="9db19-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9db19-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9db19-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9db19-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="9db19-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9db19-118">Request headers</span></span>
|<span data-ttu-id="9db19-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9db19-119">Header</span></span>|<span data-ttu-id="9db19-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9db19-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9db19-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9db19-121">Authorization</span></span>|<span data-ttu-id="9db19-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9db19-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9db19-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9db19-123">Accept</span></span>|<span data-ttu-id="9db19-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9db19-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9db19-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9db19-125">Request body</span></span>
<span data-ttu-id="9db19-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9db19-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9db19-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="9db19-127">Response</span></span>
<span data-ttu-id="9db19-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9db19-128">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9db19-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9db19-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="9db19-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9db19-130">Request</span></span>
<span data-ttu-id="9db19-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9db19-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="9db19-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9db19-132">Response</span></span>
<span data-ttu-id="9db19-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9db19-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 563

{
  "value": [
    {
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
  ]
}
```



