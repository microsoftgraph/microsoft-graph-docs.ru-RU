---
title: Перечисление объектов deviceComplianceActionItem
description: Список свойств и связей объектов deviceComplianceActionItem.
ms.openlocfilehash: 11e87ce644043d4f990c805bc65c7ea833f345b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026729"
---
# <a name="list-devicecomplianceactionitems"></a><span data-ttu-id="650a9-103">Перечисление объектов deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="650a9-103">List deviceComplianceActionItems</span></span>

> <span data-ttu-id="650a9-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="650a9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="650a9-105">Список свойств и связей объектов [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="650a9-105">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="650a9-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="650a9-106">Prerequisites</span></span>
<span data-ttu-id="650a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="650a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="650a9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="650a9-109">Permission type</span></span>|<span data-ttu-id="650a9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="650a9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="650a9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="650a9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="650a9-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="650a9-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="650a9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="650a9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="650a9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="650a9-114">Not supported.</span></span>|
|<span data-ttu-id="650a9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="650a9-115">Application</span></span>|<span data-ttu-id="650a9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="650a9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="650a9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="650a9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="650a9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="650a9-118">Request headers</span></span>
|<span data-ttu-id="650a9-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="650a9-119">Header</span></span>|<span data-ttu-id="650a9-120">Значение</span><span class="sxs-lookup"><span data-stu-id="650a9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="650a9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="650a9-121">Authorization</span></span>|<span data-ttu-id="650a9-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="650a9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="650a9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="650a9-123">Accept</span></span>|<span data-ttu-id="650a9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="650a9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="650a9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="650a9-125">Request body</span></span>
<span data-ttu-id="650a9-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="650a9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="650a9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="650a9-127">Response</span></span>
<span data-ttu-id="650a9-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="650a9-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="650a9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="650a9-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="650a9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="650a9-130">Request</span></span>
<span data-ttu-id="650a9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="650a9-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

### <a name="response"></a><span data-ttu-id="650a9-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="650a9-132">Response</span></span>
<span data-ttu-id="650a9-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="650a9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
      "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
      "gracePeriodHours": 0,
      "actionType": "notification",
      "notificationTemplateId": "Notification Template Id value",
      "notificationMessageCCList": [
        "Notification Message CCList value"
      ]
    }
  ]
}
```



