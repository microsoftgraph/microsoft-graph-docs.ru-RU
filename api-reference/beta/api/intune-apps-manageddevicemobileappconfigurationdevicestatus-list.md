---
title: Список managedDeviceMobileAppConfigurationDeviceStatuses
description: Свойства списка и связей объектов managedDeviceMobileAppConfigurationDeviceStatus.
author: tfitzmac
ms.openlocfilehash: eebe5ec2da36cad972af87600b6d6776debcbbee
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342968"
---
# <a name="list-manageddevicemobileappconfigurationdevicestatuses"></a><span data-ttu-id="c2e67-103">Список managedDeviceMobileAppConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c2e67-103">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="c2e67-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c2e67-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2e67-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2e67-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2e67-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c2e67-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2e67-107">Свойства списка и связей объектов [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="c2e67-107">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c2e67-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c2e67-108">Prerequisites</span></span>
<span data-ttu-id="c2e67-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2e67-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2e67-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2e67-111">Permission type</span></span>|<span data-ttu-id="c2e67-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2e67-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2e67-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2e67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2e67-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2e67-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c2e67-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2e67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2e67-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2e67-116">Not supported.</span></span>|
|<span data-ttu-id="c2e67-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2e67-117">Application</span></span>|<span data-ttu-id="c2e67-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2e67-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2e67-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2e67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="c2e67-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2e67-120">Request headers</span></span>
|<span data-ttu-id="c2e67-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2e67-121">Header</span></span>|<span data-ttu-id="c2e67-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c2e67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2e67-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2e67-123">Authorization</span></span>|<span data-ttu-id="c2e67-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c2e67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2e67-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c2e67-125">Accept</span></span>|<span data-ttu-id="c2e67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2e67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2e67-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2e67-127">Request body</span></span>
<span data-ttu-id="c2e67-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2e67-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2e67-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2e67-129">Response</span></span>
<span data-ttu-id="c2e67-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c2e67-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2e67-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c2e67-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c2e67-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2e67-132">Request</span></span>
<span data-ttu-id="c2e67-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2e67-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="c2e67-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2e67-134">Response</span></span>
<span data-ttu-id="c2e67-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c2e67-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





