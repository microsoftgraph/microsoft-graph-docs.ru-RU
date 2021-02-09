---
title: Список deviceManagementAutopilotPolicyStatusDetails
description: Список свойств и связей объектов deviceManagementAutopilotPolicyStatusDetail.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 400d9578704bf4154e356fa8f608dc921effda52
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155666"
---
# <a name="list-devicemanagementautopilotpolicystatusdetails"></a><span data-ttu-id="709a7-103">Список deviceManagementAutopilotPolicyStatusDetails</span><span class="sxs-lookup"><span data-stu-id="709a7-103">List deviceManagementAutopilotPolicyStatusDetails</span></span>

<span data-ttu-id="709a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="709a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="709a7-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="709a7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="709a7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="709a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="709a7-107">Список свойств и связей объектов [deviceManagementAutopilotPolicyStatusDetail.](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)</span><span class="sxs-lookup"><span data-stu-id="709a7-107">List properties and relationships of the [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="709a7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="709a7-108">Prerequisites</span></span>
<span data-ttu-id="709a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="709a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="709a7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="709a7-111">Permission type</span></span>|<span data-ttu-id="709a7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="709a7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="709a7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="709a7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="709a7-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="709a7-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="709a7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="709a7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="709a7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="709a7-116">Not supported.</span></span>|
|<span data-ttu-id="709a7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="709a7-117">Application</span></span>|<span data-ttu-id="709a7-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="709a7-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="709a7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="709a7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="709a7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="709a7-120">Request headers</span></span>
|<span data-ttu-id="709a7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="709a7-121">Header</span></span>|<span data-ttu-id="709a7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="709a7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="709a7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="709a7-123">Authorization</span></span>|<span data-ttu-id="709a7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="709a7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="709a7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="709a7-125">Accept</span></span>|<span data-ttu-id="709a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="709a7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="709a7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="709a7-127">Request body</span></span>
<span data-ttu-id="709a7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="709a7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="709a7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="709a7-129">Response</span></span>
<span data-ttu-id="709a7-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="709a7-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="709a7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="709a7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="709a7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="709a7-132">Request</span></span>
<span data-ttu-id="709a7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="709a7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
```

### <a name="response"></a><span data-ttu-id="709a7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="709a7-134">Response</span></span>
<span data-ttu-id="709a7-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="709a7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 428

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
      "id": "dbe093ee-93ee-dbe0-ee93-e0dbee93e0db",
      "displayName": "Display Name value",
      "policyType": "application",
      "complianceStatus": "compliant",
      "trackedOnEnrollmentStatus": true,
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "errorCode": 9
    }
  ]
}
```




