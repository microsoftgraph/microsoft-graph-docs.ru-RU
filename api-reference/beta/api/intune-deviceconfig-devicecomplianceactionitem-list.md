---
title: Перечисление объектов deviceComplianceActionItem
description: Список свойств и связей объектов deviceComplianceActionItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2e6cc009b308ec4dd1bd1a1bae73b6c27c615204
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37175196"
---
# <a name="list-devicecomplianceactionitems"></a><span data-ttu-id="026f2-103">Перечисление объектов deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="026f2-103">List deviceComplianceActionItems</span></span>

> <span data-ttu-id="026f2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="026f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="026f2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="026f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="026f2-106">Список свойств и связей объектов [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="026f2-106">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="026f2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="026f2-107">Prerequisites</span></span>
<span data-ttu-id="026f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="026f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="026f2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="026f2-110">Permission type</span></span>|<span data-ttu-id="026f2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="026f2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="026f2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="026f2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="026f2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="026f2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="026f2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="026f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="026f2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="026f2-115">Not supported.</span></span>|
|<span data-ttu-id="026f2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="026f2-116">Application</span></span>|<span data-ttu-id="026f2-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="026f2-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="026f2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="026f2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="026f2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="026f2-119">Request headers</span></span>
|<span data-ttu-id="026f2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="026f2-120">Header</span></span>|<span data-ttu-id="026f2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="026f2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="026f2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="026f2-122">Authorization</span></span>|<span data-ttu-id="026f2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="026f2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="026f2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="026f2-124">Accept</span></span>|<span data-ttu-id="026f2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="026f2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="026f2-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="026f2-126">Request body</span></span>
<span data-ttu-id="026f2-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="026f2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="026f2-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="026f2-128">Response</span></span>
<span data-ttu-id="026f2-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="026f2-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="026f2-130">Пример</span><span class="sxs-lookup"><span data-stu-id="026f2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="026f2-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="026f2-131">Request</span></span>
<span data-ttu-id="026f2-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="026f2-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

### <a name="response"></a><span data-ttu-id="026f2-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="026f2-133">Response</span></span>
<span data-ttu-id="026f2-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="026f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




