---
title: Get deviceComplianceScheduledActionForRule
description: Чтение свойств и связей объекта deviceComplianceScheduledActionForRule.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 43745951ea860049a644c54ea0fc71d0333dcbfc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433893"
---
# <a name="get-devicecompliancescheduledactionforrule"></a><span data-ttu-id="ef216-103">Get deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="ef216-103">Get deviceComplianceScheduledActionForRule</span></span>

<span data-ttu-id="ef216-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef216-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef216-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef216-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef216-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef216-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef216-107">Чтение свойств и связей объекта [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="ef216-107">Read properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef216-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ef216-108">Prerequisites</span></span>
<span data-ttu-id="ef216-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef216-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef216-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef216-111">Permission type</span></span>|<span data-ttu-id="ef216-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef216-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef216-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef216-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef216-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef216-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ef216-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef216-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef216-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef216-116">Not supported.</span></span>|
|<span data-ttu-id="ef216-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef216-117">Application</span></span>|<span data-ttu-id="ef216-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef216-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef216-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef216-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ef216-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ef216-120">Optional query parameters</span></span>
<span data-ttu-id="ef216-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ef216-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef216-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef216-122">Request headers</span></span>
|<span data-ttu-id="ef216-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef216-123">Header</span></span>|<span data-ttu-id="ef216-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ef216-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef216-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef216-125">Authorization</span></span>|<span data-ttu-id="ef216-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef216-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef216-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ef216-127">Accept</span></span>|<span data-ttu-id="ef216-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ef216-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef216-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ef216-129">Request body</span></span>
<span data-ttu-id="ef216-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef216-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef216-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef216-131">Response</span></span>
<span data-ttu-id="ef216-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ef216-132">If successful, this method returns a `200 OK` response code and [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef216-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ef216-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef216-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef216-134">Request</span></span>
<span data-ttu-id="ef216-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef216-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

### <a name="response"></a><span data-ttu-id="ef216-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef216-136">Response</span></span>
<span data-ttu-id="ef216-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef216-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



