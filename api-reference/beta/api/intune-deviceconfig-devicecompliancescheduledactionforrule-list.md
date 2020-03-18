---
title: List deviceComplianceScheduledActionForRules
description: Перечисление свойств и связей объектов deviceComplianceScheduledActionForRule.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f90ffb9488938f9edf710d9545ff25c433d59004
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42755275"
---
# <a name="list-devicecompliancescheduledactionforrules"></a><span data-ttu-id="73925-103">List deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="73925-103">List deviceComplianceScheduledActionForRules</span></span>

> <span data-ttu-id="73925-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73925-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73925-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73925-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73925-106">Перечисление свойств и связей объектов [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="73925-106">List properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73925-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="73925-107">Prerequisites</span></span>
<span data-ttu-id="73925-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73925-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73925-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73925-110">Permission type</span></span>|<span data-ttu-id="73925-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="73925-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73925-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73925-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73925-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="73925-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="73925-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73925-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73925-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73925-115">Not supported.</span></span>|
|<span data-ttu-id="73925-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="73925-116">Application</span></span>|<span data-ttu-id="73925-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="73925-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73925-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73925-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="73925-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="73925-119">Request headers</span></span>
|<span data-ttu-id="73925-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73925-120">Header</span></span>|<span data-ttu-id="73925-121">Значение</span><span class="sxs-lookup"><span data-stu-id="73925-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73925-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="73925-122">Authorization</span></span>|<span data-ttu-id="73925-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73925-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73925-124">Accept</span><span class="sxs-lookup"><span data-stu-id="73925-124">Accept</span></span>|<span data-ttu-id="73925-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73925-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73925-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73925-126">Request body</span></span>
<span data-ttu-id="73925-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="73925-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73925-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="73925-128">Response</span></span>
<span data-ttu-id="73925-129">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="73925-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73925-130">Пример</span><span class="sxs-lookup"><span data-stu-id="73925-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="73925-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="73925-131">Request</span></span>
<span data-ttu-id="73925-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73925-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

### <a name="response"></a><span data-ttu-id="73925-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="73925-133">Response</span></span>
<span data-ttu-id="73925-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73925-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




