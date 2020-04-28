---
title: Перечисление объектов deviceComplianceActionItem
description: Список свойств и связей объектов deviceComplianceActionItem.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ed667e7860753c11b2b2119fb9cfa9e56ca01aa5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43434247"
---
# <a name="list-devicecomplianceactionitems"></a><span data-ttu-id="c0237-103">Перечисление объектов deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="c0237-103">List deviceComplianceActionItems</span></span>

<span data-ttu-id="c0237-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0237-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0237-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0237-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0237-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0237-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0237-107">Список свойств и связей объектов [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="c0237-107">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c0237-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c0237-108">Prerequisites</span></span>
<span data-ttu-id="c0237-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0237-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0237-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0237-111">Permission type</span></span>|<span data-ttu-id="c0237-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0237-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0237-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0237-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0237-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0237-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c0237-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0237-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0237-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0237-116">Not supported.</span></span>|
|<span data-ttu-id="c0237-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0237-117">Application</span></span>|<span data-ttu-id="c0237-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0237-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0237-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0237-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c0237-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c0237-120">Request headers</span></span>
|<span data-ttu-id="c0237-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c0237-121">Header</span></span>|<span data-ttu-id="c0237-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c0237-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0237-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0237-123">Authorization</span></span>|<span data-ttu-id="c0237-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0237-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0237-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c0237-125">Accept</span></span>|<span data-ttu-id="c0237-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0237-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0237-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c0237-127">Request body</span></span>
<span data-ttu-id="c0237-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0237-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0237-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c0237-129">Response</span></span>
<span data-ttu-id="c0237-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c0237-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0237-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c0237-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0237-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0237-132">Request</span></span>
<span data-ttu-id="c0237-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0237-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

### <a name="response"></a><span data-ttu-id="c0237-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0237-134">Response</span></span>
<span data-ttu-id="c0237-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c0237-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



