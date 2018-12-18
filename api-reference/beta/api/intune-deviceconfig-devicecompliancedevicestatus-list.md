---
title: List deviceComplianceDeviceStatuses
description: Перечисление свойств и связей объектов deviceComplianceDeviceStatus.
author: tfitzmac
ms.openlocfilehash: 0cf160e98be194bdbdbde29d3e06e3269db40bbb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330333"
---
# <a name="list-devicecompliancedevicestatuses"></a><span data-ttu-id="9c1fb-103">List deviceComplianceDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="9c1fb-103">List deviceComplianceDeviceStatuses</span></span>

> <span data-ttu-id="9c1fb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9c1fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c1fb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c1fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c1fb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9c1fb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c1fb-107">Перечисление свойств и связей объектов [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="9c1fb-107">List properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9c1fb-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9c1fb-108">Prerequisites</span></span>
<span data-ttu-id="9c1fb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c1fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c1fb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c1fb-111">Permission type</span></span>|<span data-ttu-id="9c1fb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c1fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c1fb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c1fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c1fb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c1fb-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9c1fb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c1fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c1fb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c1fb-116">Not supported.</span></span>|
|<span data-ttu-id="9c1fb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c1fb-117">Application</span></span>|<span data-ttu-id="9c1fb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c1fb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c1fb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c1fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="9c1fb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c1fb-120">Request headers</span></span>
|<span data-ttu-id="9c1fb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9c1fb-121">Header</span></span>|<span data-ttu-id="9c1fb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9c1fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c1fb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c1fb-123">Authorization</span></span>|<span data-ttu-id="9c1fb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9c1fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c1fb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9c1fb-125">Accept</span></span>|<span data-ttu-id="9c1fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c1fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c1fb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c1fb-127">Request body</span></span>
<span data-ttu-id="9c1fb-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c1fb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c1fb-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="9c1fb-129">Response</span></span>
<span data-ttu-id="9c1fb-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9c1fb-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c1fb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9c1fb-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9c1fb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c1fb-132">Request</span></span>
<span data-ttu-id="9c1fb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c1fb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="9c1fb-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9c1fb-134">Response</span></span>
<span data-ttu-id="9c1fb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9c1fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 566

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
      "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
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





