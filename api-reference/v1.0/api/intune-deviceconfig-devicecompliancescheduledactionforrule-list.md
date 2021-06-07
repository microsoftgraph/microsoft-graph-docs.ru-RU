---
title: List deviceComplianceScheduledActionForRules
description: Перечисление свойств и связей объектов deviceComplianceScheduledActionForRule.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6dba306e8a83c9cc3f2f066b96fcfab0a3ae1e84
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756605"
---
# <a name="list-devicecompliancescheduledactionforrules"></a><span data-ttu-id="22d25-103">List deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="22d25-103">List deviceComplianceScheduledActionForRules</span></span>

<span data-ttu-id="22d25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22d25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22d25-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22d25-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22d25-106">Перечисление свойств и связей объектов [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="22d25-106">List properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22d25-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="22d25-107">Prerequisites</span></span>
<span data-ttu-id="22d25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22d25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22d25-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22d25-110">Permission type</span></span>|<span data-ttu-id="22d25-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22d25-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22d25-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22d25-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22d25-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22d25-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22d25-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22d25-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22d25-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22d25-115">Not supported.</span></span>|
|<span data-ttu-id="22d25-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="22d25-116">Application</span></span>|<span data-ttu-id="22d25-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22d25-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22d25-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22d25-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="22d25-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="22d25-119">Request headers</span></span>
|<span data-ttu-id="22d25-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22d25-120">Header</span></span>|<span data-ttu-id="22d25-121">Значение</span><span class="sxs-lookup"><span data-stu-id="22d25-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22d25-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="22d25-122">Authorization</span></span>|<span data-ttu-id="22d25-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22d25-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22d25-124">Accept</span><span class="sxs-lookup"><span data-stu-id="22d25-124">Accept</span></span>|<span data-ttu-id="22d25-125">application/json</span><span class="sxs-lookup"><span data-stu-id="22d25-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22d25-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22d25-126">Request body</span></span>
<span data-ttu-id="22d25-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="22d25-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22d25-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="22d25-128">Response</span></span>
<span data-ttu-id="22d25-129">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="22d25-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22d25-130">Пример</span><span class="sxs-lookup"><span data-stu-id="22d25-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="22d25-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="22d25-131">Request</span></span>
<span data-ttu-id="22d25-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22d25-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

### <a name="response"></a><span data-ttu-id="22d25-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="22d25-133">Response</span></span>
<span data-ttu-id="22d25-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22d25-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 208

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
      "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
      "ruleName": "Rule Name value"
    }
  ]
}
```




