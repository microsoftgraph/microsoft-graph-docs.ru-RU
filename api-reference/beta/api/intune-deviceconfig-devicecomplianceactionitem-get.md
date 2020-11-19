---
title: Get deviceComplianceActionItem
description: Чтение свойств и связей объекта deviceComplianceActionItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 73ce4a69d0949e8e1871dcb66075caf5c4805ec0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49292809"
---
# <a name="get-devicecomplianceactionitem"></a><span data-ttu-id="bda12-103">Get deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="bda12-103">Get deviceComplianceActionItem</span></span>

<span data-ttu-id="bda12-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bda12-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bda12-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bda12-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bda12-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bda12-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bda12-107">Чтение свойств и связей объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="bda12-107">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bda12-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bda12-108">Prerequisites</span></span>
<span data-ttu-id="bda12-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bda12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bda12-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bda12-111">Permission type</span></span>|<span data-ttu-id="bda12-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bda12-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bda12-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bda12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bda12-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bda12-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bda12-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bda12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bda12-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bda12-116">Not supported.</span></span>|
|<span data-ttu-id="bda12-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bda12-117">Application</span></span>|<span data-ttu-id="bda12-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bda12-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bda12-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bda12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bda12-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bda12-120">Optional query parameters</span></span>
<span data-ttu-id="bda12-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bda12-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bda12-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bda12-122">Request headers</span></span>
|<span data-ttu-id="bda12-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bda12-123">Header</span></span>|<span data-ttu-id="bda12-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bda12-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bda12-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bda12-125">Authorization</span></span>|<span data-ttu-id="bda12-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bda12-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bda12-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bda12-127">Accept</span></span>|<span data-ttu-id="bda12-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bda12-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bda12-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bda12-129">Request body</span></span>
<span data-ttu-id="bda12-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bda12-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bda12-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bda12-131">Response</span></span>
<span data-ttu-id="bda12-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bda12-132">If successful, this method returns a `200 OK` response code and [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bda12-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bda12-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="bda12-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bda12-134">Request</span></span>
<span data-ttu-id="bda12-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bda12-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="bda12-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bda12-136">Response</span></span>
<span data-ttu-id="bda12-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bda12-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




