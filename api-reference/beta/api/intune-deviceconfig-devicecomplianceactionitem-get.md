---
title: Get deviceComplianceActionItem
description: Чтение свойств и связей объекта deviceComplianceActionItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32755e27d7dbd967cb525f53c1ed14c6a7d9f06a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928003"
---
# <a name="get-devicecomplianceactionitem"></a><span data-ttu-id="535ff-103">Get deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="535ff-103">Get deviceComplianceActionItem</span></span>

> <span data-ttu-id="535ff-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="535ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="535ff-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="535ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="535ff-106">Чтение свойств и связей объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="535ff-106">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="535ff-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="535ff-107">Prerequisites</span></span>
<span data-ttu-id="535ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="535ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="535ff-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="535ff-110">Permission type</span></span>|<span data-ttu-id="535ff-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="535ff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="535ff-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="535ff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="535ff-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="535ff-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="535ff-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="535ff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="535ff-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="535ff-115">Not supported.</span></span>|
|<span data-ttu-id="535ff-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="535ff-116">Application</span></span>|<span data-ttu-id="535ff-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="535ff-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="535ff-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="535ff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="535ff-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="535ff-119">Optional query parameters</span></span>
<span data-ttu-id="535ff-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="535ff-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="535ff-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="535ff-121">Request headers</span></span>
|<span data-ttu-id="535ff-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="535ff-122">Header</span></span>|<span data-ttu-id="535ff-123">Значение</span><span class="sxs-lookup"><span data-stu-id="535ff-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="535ff-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="535ff-124">Authorization</span></span>|<span data-ttu-id="535ff-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="535ff-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="535ff-126">Accept</span><span class="sxs-lookup"><span data-stu-id="535ff-126">Accept</span></span>|<span data-ttu-id="535ff-127">application/json</span><span class="sxs-lookup"><span data-stu-id="535ff-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="535ff-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="535ff-128">Request body</span></span>
<span data-ttu-id="535ff-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="535ff-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="535ff-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="535ff-130">Response</span></span>
<span data-ttu-id="535ff-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="535ff-131">If successful, this method returns a `200 OK` response code and [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="535ff-132">Пример</span><span class="sxs-lookup"><span data-stu-id="535ff-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="535ff-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="535ff-133">Request</span></span>
<span data-ttu-id="535ff-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="535ff-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="535ff-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="535ff-135">Response</span></span>
<span data-ttu-id="535ff-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="535ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




