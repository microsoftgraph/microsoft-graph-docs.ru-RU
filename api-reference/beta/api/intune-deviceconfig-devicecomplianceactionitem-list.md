---
title: Перечисление объектов deviceComplianceActionItem
description: Список свойств и связей объектов deviceComplianceActionItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 444db37fc0b7832990fcdfb90be47627a8b6bfe4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048042"
---
# <a name="list-devicecomplianceactionitems"></a><span data-ttu-id="fb9be-103">Перечисление объектов deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="fb9be-103">List deviceComplianceActionItems</span></span>

<span data-ttu-id="fb9be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb9be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb9be-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb9be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb9be-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb9be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb9be-107">Список свойств и связей объектов [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="fb9be-107">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb9be-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fb9be-108">Prerequisites</span></span>
<span data-ttu-id="fb9be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb9be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb9be-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb9be-111">Permission type</span></span>|<span data-ttu-id="fb9be-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb9be-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb9be-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb9be-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb9be-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb9be-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fb9be-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb9be-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb9be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb9be-116">Not supported.</span></span>|
|<span data-ttu-id="fb9be-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb9be-117">Application</span></span>|<span data-ttu-id="fb9be-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb9be-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb9be-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb9be-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fb9be-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fb9be-120">Request headers</span></span>
|<span data-ttu-id="fb9be-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb9be-121">Header</span></span>|<span data-ttu-id="fb9be-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fb9be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb9be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb9be-123">Authorization</span></span>|<span data-ttu-id="fb9be-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb9be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb9be-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb9be-125">Accept</span></span>|<span data-ttu-id="fb9be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb9be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb9be-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fb9be-127">Request body</span></span>
<span data-ttu-id="fb9be-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb9be-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb9be-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb9be-129">Response</span></span>
<span data-ttu-id="fb9be-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fb9be-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb9be-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fb9be-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb9be-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb9be-132">Request</span></span>
<span data-ttu-id="fb9be-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb9be-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

### <a name="response"></a><span data-ttu-id="fb9be-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb9be-134">Response</span></span>
<span data-ttu-id="fb9be-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb9be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






