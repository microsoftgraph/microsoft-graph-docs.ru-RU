---
title: Перечисление объектов deviceComplianceActionItem
description: Список свойств и связей объектов deviceComplianceActionItem.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d3ec9b512fb48114cb58920d109ded1dba13dc77
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813617"
---
# <a name="list-devicecomplianceactionitems"></a><span data-ttu-id="a47d2-103">Перечисление объектов deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="a47d2-103">List deviceComplianceActionItems</span></span>

> <span data-ttu-id="a47d2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a47d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a47d2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a47d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a47d2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a47d2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a47d2-107">Список свойств и связей объектов [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="a47d2-107">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a47d2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a47d2-108">Prerequisites</span></span>
<span data-ttu-id="a47d2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a47d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a47d2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a47d2-111">Permission type</span></span>|<span data-ttu-id="a47d2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a47d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a47d2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a47d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a47d2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a47d2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a47d2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a47d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a47d2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a47d2-116">Not supported.</span></span>|
|<span data-ttu-id="a47d2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a47d2-117">Application</span></span>|<span data-ttu-id="a47d2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a47d2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a47d2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a47d2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a47d2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a47d2-120">Request headers</span></span>
|<span data-ttu-id="a47d2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a47d2-121">Header</span></span>|<span data-ttu-id="a47d2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a47d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a47d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a47d2-123">Authorization</span></span>|<span data-ttu-id="a47d2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a47d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a47d2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a47d2-125">Accept</span></span>|<span data-ttu-id="a47d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a47d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a47d2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a47d2-127">Request body</span></span>
<span data-ttu-id="a47d2-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a47d2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a47d2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a47d2-129">Response</span></span>
<span data-ttu-id="a47d2-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a47d2-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a47d2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a47d2-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a47d2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a47d2-132">Request</span></span>
<span data-ttu-id="a47d2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a47d2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

### <a name="response"></a><span data-ttu-id="a47d2-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a47d2-134">Response</span></span>
<span data-ttu-id="a47d2-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a47d2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





