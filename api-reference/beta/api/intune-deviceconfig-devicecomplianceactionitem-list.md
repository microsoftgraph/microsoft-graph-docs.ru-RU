---
title: Перечисление объектов deviceComplianceActionItem
description: Список свойств и связей объектов deviceComplianceActionItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ae0166800700245f895042bd47fcae413db323e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36310908"
---
# <a name="list-devicecomplianceactionitems"></a><span data-ttu-id="f6934-103">Перечисление объектов deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="f6934-103">List deviceComplianceActionItems</span></span>

> <span data-ttu-id="f6934-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6934-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6934-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f6934-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6934-106">Список свойств и связей объектов [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="f6934-106">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6934-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f6934-107">Prerequisites</span></span>
<span data-ttu-id="f6934-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6934-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6934-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6934-110">Permission type</span></span>|<span data-ttu-id="f6934-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6934-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6934-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6934-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6934-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6934-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f6934-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6934-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6934-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6934-115">Not supported.</span></span>|
|<span data-ttu-id="f6934-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6934-116">Application</span></span>|<span data-ttu-id="f6934-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6934-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6934-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6934-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f6934-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6934-119">Request headers</span></span>
|<span data-ttu-id="f6934-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6934-120">Header</span></span>|<span data-ttu-id="f6934-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f6934-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6934-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6934-122">Authorization</span></span>|<span data-ttu-id="f6934-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6934-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6934-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f6934-124">Accept</span></span>|<span data-ttu-id="f6934-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f6934-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6934-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6934-126">Request body</span></span>
<span data-ttu-id="f6934-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6934-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6934-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6934-128">Response</span></span>
<span data-ttu-id="f6934-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6934-129">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6934-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f6934-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6934-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6934-131">Request</span></span>
<span data-ttu-id="f6934-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6934-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

### <a name="response"></a><span data-ttu-id="f6934-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6934-133">Response</span></span>
<span data-ttu-id="f6934-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6934-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






