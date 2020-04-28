---
title: Get deviceComplianceActionItem
description: Чтение свойств и связей объекта deviceComplianceActionItem.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4271364c4f890ad8c95f8efa5d4d6ea894ac375d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43434254"
---
# <a name="get-devicecomplianceactionitem"></a><span data-ttu-id="7a7af-103">Get deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="7a7af-103">Get deviceComplianceActionItem</span></span>

<span data-ttu-id="7a7af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a7af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a7af-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a7af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a7af-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a7af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a7af-107">Чтение свойств и связей объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="7a7af-107">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a7af-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="7a7af-108">Prerequisites</span></span>
<span data-ttu-id="7a7af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a7af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a7af-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a7af-111">Permission type</span></span>|<span data-ttu-id="7a7af-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a7af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a7af-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a7af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a7af-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a7af-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7a7af-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a7af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a7af-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a7af-116">Not supported.</span></span>|
|<span data-ttu-id="7a7af-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a7af-117">Application</span></span>|<span data-ttu-id="7a7af-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a7af-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a7af-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a7af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a7af-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7a7af-120">Optional query parameters</span></span>
<span data-ttu-id="7a7af-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7a7af-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a7af-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a7af-122">Request headers</span></span>
|<span data-ttu-id="7a7af-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a7af-123">Header</span></span>|<span data-ttu-id="7a7af-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7a7af-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a7af-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a7af-125">Authorization</span></span>|<span data-ttu-id="7a7af-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a7af-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a7af-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7a7af-127">Accept</span></span>|<span data-ttu-id="7a7af-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7a7af-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a7af-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7a7af-129">Request body</span></span>
<span data-ttu-id="7a7af-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7a7af-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a7af-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7a7af-131">Response</span></span>
<span data-ttu-id="7a7af-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7a7af-132">If successful, this method returns a `200 OK` response code and [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a7af-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7a7af-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a7af-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a7af-134">Request</span></span>
<span data-ttu-id="7a7af-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a7af-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="7a7af-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a7af-136">Response</span></span>
<span data-ttu-id="7a7af-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7a7af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



