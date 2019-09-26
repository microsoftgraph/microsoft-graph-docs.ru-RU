---
title: List deviceComplianceScheduledActionForRules
description: Перечисление свойств и связей объектов deviceComplianceScheduledActionForRule.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8a104b7f9db0b2c57a30f2321c9aeaf312329439
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37175000"
---
# <a name="list-devicecompliancescheduledactionforrules"></a><span data-ttu-id="89b20-103">List deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="89b20-103">List deviceComplianceScheduledActionForRules</span></span>

> <span data-ttu-id="89b20-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89b20-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89b20-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89b20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89b20-106">Перечисление свойств и связей объектов [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span><span class="sxs-lookup"><span data-stu-id="89b20-106">List properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89b20-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="89b20-107">Prerequisites</span></span>
<span data-ttu-id="89b20-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89b20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89b20-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89b20-110">Permission type</span></span>|<span data-ttu-id="89b20-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="89b20-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89b20-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89b20-112">Delegated (work or school account)</span></span>|<span data-ttu-id="89b20-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89b20-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="89b20-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89b20-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89b20-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89b20-115">Not supported.</span></span>|
|<span data-ttu-id="89b20-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89b20-116">Application</span></span>|<span data-ttu-id="89b20-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89b20-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89b20-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89b20-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="89b20-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89b20-119">Request headers</span></span>
|<span data-ttu-id="89b20-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89b20-120">Header</span></span>|<span data-ttu-id="89b20-121">Значение</span><span class="sxs-lookup"><span data-stu-id="89b20-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89b20-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89b20-122">Authorization</span></span>|<span data-ttu-id="89b20-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89b20-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89b20-124">Accept</span><span class="sxs-lookup"><span data-stu-id="89b20-124">Accept</span></span>|<span data-ttu-id="89b20-125">application/json</span><span class="sxs-lookup"><span data-stu-id="89b20-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89b20-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="89b20-126">Request body</span></span>
<span data-ttu-id="89b20-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89b20-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89b20-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="89b20-128">Response</span></span>
<span data-ttu-id="89b20-129">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию объектов [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="89b20-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89b20-130">Пример</span><span class="sxs-lookup"><span data-stu-id="89b20-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="89b20-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="89b20-131">Request</span></span>
<span data-ttu-id="89b20-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89b20-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

### <a name="response"></a><span data-ttu-id="89b20-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="89b20-133">Response</span></span>
<span data-ttu-id="89b20-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89b20-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




