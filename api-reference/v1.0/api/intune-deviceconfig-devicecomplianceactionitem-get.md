---
title: Get deviceComplianceActionItem
description: Чтение свойств и связей объекта deviceComplianceActionItem.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 23a34f0f3da6023dfb62e270b834549972a72305
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997781"
---
# <a name="get-devicecomplianceactionitem"></a><span data-ttu-id="1b2a7-103">Get deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="1b2a7-103">Get deviceComplianceActionItem</span></span>

> <span data-ttu-id="1b2a7-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b2a7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b2a7-105">Чтение свойств и связей объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="1b2a7-105">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b2a7-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="1b2a7-106">Prerequisites</span></span>
<span data-ttu-id="1b2a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b2a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b2a7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b2a7-109">Permission type</span></span>|<span data-ttu-id="1b2a7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b2a7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b2a7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b2a7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1b2a7-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b2a7-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1b2a7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b2a7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b2a7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b2a7-114">Not supported.</span></span>|
|<span data-ttu-id="1b2a7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b2a7-115">Application</span></span>|<span data-ttu-id="1b2a7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b2a7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b2a7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b2a7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1b2a7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1b2a7-118">Optional query parameters</span></span>
<span data-ttu-id="1b2a7-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1b2a7-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b2a7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b2a7-120">Request headers</span></span>
|<span data-ttu-id="1b2a7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b2a7-121">Header</span></span>|<span data-ttu-id="1b2a7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1b2a7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b2a7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b2a7-123">Authorization</span></span>|<span data-ttu-id="1b2a7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b2a7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b2a7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1b2a7-125">Accept</span></span>|<span data-ttu-id="1b2a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b2a7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b2a7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1b2a7-127">Request body</span></span>
<span data-ttu-id="1b2a7-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1b2a7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b2a7-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b2a7-129">Response</span></span>
<span data-ttu-id="1b2a7-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1b2a7-130">If successful, this method returns a `200 OK` response code and [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b2a7-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1b2a7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b2a7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b2a7-132">Request</span></span>
<span data-ttu-id="1b2a7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b2a7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="1b2a7-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b2a7-134">Response</span></span>
<span data-ttu-id="1b2a7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b2a7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
    "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
    "gracePeriodHours": 0,
    "actionType": "notification",
    "notificationTemplateId": "Notification Template Id value",
    "notificationMessageCCList": [
      "Notification Message CCList value"
    ]
  }
}
```



