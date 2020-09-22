---
title: Перечисление объектов deviceComplianceActionItem
description: Список свойств и связей объектов deviceComplianceActionItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 96c3dd4ff0ccdc2be044625b5b569a047b355ab2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052175"
---
# <a name="list-devicecomplianceactionitems"></a><span data-ttu-id="1a748-103">Перечисление объектов deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="1a748-103">List deviceComplianceActionItems</span></span>

<span data-ttu-id="1a748-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a748-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a748-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a748-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a748-106">Список свойств и связей объектов [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="1a748-106">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a748-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1a748-107">Prerequisites</span></span>
<span data-ttu-id="1a748-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a748-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a748-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a748-110">Permission type</span></span>|<span data-ttu-id="1a748-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a748-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a748-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a748-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1a748-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a748-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1a748-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a748-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a748-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a748-115">Not supported.</span></span>|
|<span data-ttu-id="1a748-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a748-116">Application</span></span>|<span data-ttu-id="1a748-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a748-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a748-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a748-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1a748-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1a748-119">Request headers</span></span>
|<span data-ttu-id="1a748-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1a748-120">Header</span></span>|<span data-ttu-id="1a748-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1a748-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a748-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a748-122">Authorization</span></span>|<span data-ttu-id="1a748-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a748-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a748-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1a748-124">Accept</span></span>|<span data-ttu-id="1a748-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1a748-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a748-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1a748-126">Request body</span></span>
<span data-ttu-id="1a748-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1a748-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a748-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a748-128">Response</span></span>
<span data-ttu-id="1a748-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a748-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a748-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1a748-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a748-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a748-131">Request</span></span>
<span data-ttu-id="1a748-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a748-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

### <a name="response"></a><span data-ttu-id="1a748-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a748-133">Response</span></span>
<span data-ttu-id="1a748-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a748-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









