---
title: Get deviceComplianceScheduledActionForRule
description: Чтение свойств и связей объекта deviceComplianceScheduledActionForRule.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7e9c152a39f5fcf4908fb44e9e294209b1aa082d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979028"
---
# <a name="get-devicecompliancescheduledactionforrule"></a><span data-ttu-id="0ab40-103">Get deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="0ab40-103">Get deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="0ab40-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0ab40-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ab40-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ab40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ab40-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0ab40-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ab40-107">Чтение свойств и связей объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="0ab40-107">Read properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0ab40-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0ab40-108">Prerequisites</span></span>
<span data-ttu-id="0ab40-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ab40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ab40-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ab40-111">Permission type</span></span>|<span data-ttu-id="0ab40-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ab40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ab40-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ab40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ab40-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ab40-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0ab40-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ab40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ab40-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ab40-116">Not supported.</span></span>|
|<span data-ttu-id="0ab40-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ab40-117">Application</span></span>|<span data-ttu-id="0ab40-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ab40-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ab40-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ab40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ab40-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0ab40-120">Optional query parameters</span></span>
<span data-ttu-id="0ab40-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="0ab40-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0ab40-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ab40-122">Request headers</span></span>
|<span data-ttu-id="0ab40-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ab40-123">Header</span></span>|<span data-ttu-id="0ab40-124">Значение</span><span class="sxs-lookup"><span data-stu-id="0ab40-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ab40-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ab40-125">Authorization</span></span>|<span data-ttu-id="0ab40-126">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0ab40-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ab40-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0ab40-127">Accept</span></span>|<span data-ttu-id="0ab40-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0ab40-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ab40-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0ab40-129">Request body</span></span>
<span data-ttu-id="0ab40-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ab40-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ab40-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ab40-131">Response</span></span>
<span data-ttu-id="0ab40-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0ab40-132">If successful, this method returns a `200 OK` response code and [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ab40-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0ab40-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ab40-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ab40-134">Request</span></span>
<span data-ttu-id="0ab40-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ab40-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

### <a name="response"></a><span data-ttu-id="0ab40-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ab40-136">Response</span></span>
<span data-ttu-id="0ab40-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0ab40-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 188

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
    "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
    "ruleName": "Rule Name value"
  }
}
```





