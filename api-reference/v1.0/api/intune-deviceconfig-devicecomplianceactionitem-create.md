---
title: Создание объекта deviceComplianceActionItem
description: Создание объекта deviceComplianceActionItem.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0b2102b0242c002c57747ebecf1731fdb325e898
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871010"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="836ab-103">Создание объекта deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="836ab-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="836ab-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="836ab-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="836ab-105">Создание объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="836ab-105">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="836ab-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="836ab-106">Prerequisites</span></span>
<span data-ttu-id="836ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="836ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="836ab-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="836ab-109">Permission type</span></span>|<span data-ttu-id="836ab-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="836ab-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="836ab-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="836ab-111">Delegated (work or school account)</span></span>|<span data-ttu-id="836ab-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="836ab-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="836ab-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="836ab-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="836ab-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="836ab-114">Not supported.</span></span>|
|<span data-ttu-id="836ab-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="836ab-115">Application</span></span>|<span data-ttu-id="836ab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="836ab-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="836ab-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="836ab-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="836ab-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="836ab-118">Request headers</span></span>
|<span data-ttu-id="836ab-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="836ab-119">Header</span></span>|<span data-ttu-id="836ab-120">Значение</span><span class="sxs-lookup"><span data-stu-id="836ab-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="836ab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="836ab-121">Authorization</span></span>|<span data-ttu-id="836ab-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="836ab-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="836ab-123">Accept</span><span class="sxs-lookup"><span data-stu-id="836ab-123">Accept</span></span>|<span data-ttu-id="836ab-124">application/json</span><span class="sxs-lookup"><span data-stu-id="836ab-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="836ab-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="836ab-125">Request body</span></span>
<span data-ttu-id="836ab-126">В тексте запроса добавьте представление объекта deviceComplianceActionItem в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="836ab-126">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="836ab-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="836ab-127">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="836ab-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="836ab-128">Property</span></span>|<span data-ttu-id="836ab-129">Тип</span><span class="sxs-lookup"><span data-stu-id="836ab-129">Type</span></span>|<span data-ttu-id="836ab-130">Описание</span><span class="sxs-lookup"><span data-stu-id="836ab-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="836ab-131">id</span><span class="sxs-lookup"><span data-stu-id="836ab-131">id</span></span>|<span data-ttu-id="836ab-132">Строка</span><span class="sxs-lookup"><span data-stu-id="836ab-132">String</span></span>|<span data-ttu-id="836ab-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="836ab-133">Key of the entity.</span></span>|
|<span data-ttu-id="836ab-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="836ab-134">gracePeriodHours</span></span>|<span data-ttu-id="836ab-135">Int32</span><span class="sxs-lookup"><span data-stu-id="836ab-135">Int32</span></span>|<span data-ttu-id="836ab-136">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="836ab-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="836ab-137">Допустимые значения: от 0 до 8760.</span><span class="sxs-lookup"><span data-stu-id="836ab-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="836ab-138">actionType</span><span class="sxs-lookup"><span data-stu-id="836ab-138">actionType</span></span>|[<span data-ttu-id="836ab-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="836ab-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="836ab-140">Какое действие необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="836ab-140">What action to take.</span></span> <span data-ttu-id="836ab-141">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="836ab-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="836ab-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="836ab-142">notificationTemplateId</span></span>|<span data-ttu-id="836ab-143">String</span><span class="sxs-lookup"><span data-stu-id="836ab-143">String</span></span>|<span data-ttu-id="836ab-144">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="836ab-144">What notification Message template to use</span></span>|
|<span data-ttu-id="836ab-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="836ab-145">notificationMessageCCList</span></span>|<span data-ttu-id="836ab-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="836ab-146">String collection</span></span>|<span data-ttu-id="836ab-147">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="836ab-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="836ab-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="836ab-148">Response</span></span>
<span data-ttu-id="836ab-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="836ab-149">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="836ab-150">Пример</span><span class="sxs-lookup"><span data-stu-id="836ab-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="836ab-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="836ab-151">Request</span></span>
<span data-ttu-id="836ab-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="836ab-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="836ab-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="836ab-153">Response</span></span>
<span data-ttu-id="836ab-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="836ab-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 320

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
```



