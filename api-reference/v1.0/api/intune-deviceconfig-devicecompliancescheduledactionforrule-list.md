---
title: List deviceComplianceScheduledActionForRules
description: Перечисление свойств и связей объектов deviceComplianceScheduledActionForRule.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 32c5b75f9d0d2af699a3ed8f41e6294e43e49c12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965238"
---
# <a name="list-devicecompliancescheduledactionforrules"></a><span data-ttu-id="395bf-103">List deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="395bf-103">List deviceComplianceScheduledActionForRules</span></span>

> <span data-ttu-id="395bf-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="395bf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="395bf-105">Перечисление свойств и связей объектов [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="395bf-105">List properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="395bf-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="395bf-106">Prerequisites</span></span>
<span data-ttu-id="395bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="395bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="395bf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="395bf-109">Permission type</span></span>|<span data-ttu-id="395bf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="395bf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="395bf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="395bf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="395bf-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="395bf-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="395bf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="395bf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="395bf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="395bf-114">Not supported.</span></span>|
|<span data-ttu-id="395bf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="395bf-115">Application</span></span>|<span data-ttu-id="395bf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="395bf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="395bf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="395bf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="395bf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="395bf-118">Request headers</span></span>
|<span data-ttu-id="395bf-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="395bf-119">Header</span></span>|<span data-ttu-id="395bf-120">Значение</span><span class="sxs-lookup"><span data-stu-id="395bf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="395bf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="395bf-121">Authorization</span></span>|<span data-ttu-id="395bf-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="395bf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="395bf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="395bf-123">Accept</span></span>|<span data-ttu-id="395bf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="395bf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="395bf-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="395bf-125">Request body</span></span>
<span data-ttu-id="395bf-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="395bf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="395bf-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="395bf-127">Response</span></span>
<span data-ttu-id="395bf-128">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="395bf-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="395bf-129">Пример</span><span class="sxs-lookup"><span data-stu-id="395bf-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="395bf-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="395bf-130">Request</span></span>
<span data-ttu-id="395bf-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="395bf-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

### <a name="response"></a><span data-ttu-id="395bf-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="395bf-132">Response</span></span>
<span data-ttu-id="395bf-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="395bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



