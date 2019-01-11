---
title: Список windowsAutopilotDeviceIdentities
description: Свойства списка и связей объектов windowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a3519dbd27086c8d22ec03f201512f6d15283075
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891352"
---
# <a name="list-windowsautopilotdeviceidentities"></a><span data-ttu-id="553d9-103">Список windowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="553d9-103">List windowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="553d9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="553d9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="553d9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="553d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="553d9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="553d9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="553d9-107">Свойства списка и связей объектов [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="553d9-107">List properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="553d9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="553d9-108">Prerequisites</span></span>
<span data-ttu-id="553d9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="553d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="553d9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="553d9-111">Permission type</span></span>|<span data-ttu-id="553d9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="553d9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="553d9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="553d9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="553d9-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="553d9-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="553d9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="553d9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="553d9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="553d9-116">Not supported.</span></span>|
|<span data-ttu-id="553d9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="553d9-117">Application</span></span>|<span data-ttu-id="553d9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="553d9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="553d9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="553d9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="553d9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="553d9-120">Request headers</span></span>
|<span data-ttu-id="553d9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="553d9-121">Header</span></span>|<span data-ttu-id="553d9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="553d9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="553d9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="553d9-123">Authorization</span></span>|<span data-ttu-id="553d9-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="553d9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="553d9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="553d9-125">Accept</span></span>|<span data-ttu-id="553d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="553d9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="553d9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="553d9-127">Request body</span></span>
<span data-ttu-id="553d9-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="553d9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="553d9-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="553d9-129">Response</span></span>
<span data-ttu-id="553d9-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="553d9-130">If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="553d9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="553d9-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="553d9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="553d9-132">Request</span></span>
<span data-ttu-id="553d9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="553d9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="553d9-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="553d9-134">Response</span></span>
<span data-ttu-id="553d9-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="553d9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 897

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
      "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
      "deploymentProfileAssignmentStatus": "assignedInSync",
      "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
      "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
      "orderIdentifier": "Order Identifier value",
      "purchaseOrderIdentifier": "Purchase Order Identifier value",
      "serialNumber": "Serial Number value",
      "productKey": "Product Key value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "enrollmentState": "enrolled",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "addressableUserName": "Addressable User Name value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





