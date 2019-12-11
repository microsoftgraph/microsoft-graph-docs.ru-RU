---
title: Get deviceComplianceScheduledActionForRule
description: Чтение свойств и связей объекта deviceComplianceScheduledActionForRule.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3001feef6fc78013e7298c5f7b6460efda117543
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949597"
---
# <a name="get-devicecompliancescheduledactionforrule"></a><span data-ttu-id="38e45-103">Get deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="38e45-103">Get deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="38e45-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38e45-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38e45-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38e45-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38e45-106">Чтение свойств и связей объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="38e45-106">Read properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38e45-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="38e45-107">Prerequisites</span></span>
<span data-ttu-id="38e45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38e45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38e45-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38e45-110">Permission type</span></span>|<span data-ttu-id="38e45-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38e45-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38e45-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38e45-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38e45-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38e45-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="38e45-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38e45-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38e45-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38e45-115">Not supported.</span></span>|
|<span data-ttu-id="38e45-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38e45-116">Application</span></span>|<span data-ttu-id="38e45-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38e45-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38e45-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38e45-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38e45-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="38e45-119">Optional query parameters</span></span>
<span data-ttu-id="38e45-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="38e45-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38e45-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38e45-121">Request headers</span></span>
|<span data-ttu-id="38e45-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38e45-122">Header</span></span>|<span data-ttu-id="38e45-123">Значение</span><span class="sxs-lookup"><span data-stu-id="38e45-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38e45-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38e45-124">Authorization</span></span>|<span data-ttu-id="38e45-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38e45-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38e45-126">Accept</span><span class="sxs-lookup"><span data-stu-id="38e45-126">Accept</span></span>|<span data-ttu-id="38e45-127">application/json</span><span class="sxs-lookup"><span data-stu-id="38e45-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38e45-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="38e45-128">Request body</span></span>
<span data-ttu-id="38e45-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="38e45-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38e45-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="38e45-130">Response</span></span>
<span data-ttu-id="38e45-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="38e45-131">If successful, this method returns a `200 OK` response code and [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38e45-132">Пример</span><span class="sxs-lookup"><span data-stu-id="38e45-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="38e45-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="38e45-133">Request</span></span>
<span data-ttu-id="38e45-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38e45-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

### <a name="response"></a><span data-ttu-id="38e45-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="38e45-135">Response</span></span>
<span data-ttu-id="38e45-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38e45-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





