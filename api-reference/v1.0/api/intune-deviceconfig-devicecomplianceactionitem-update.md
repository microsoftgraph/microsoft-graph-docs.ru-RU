---
title: Update deviceComplianceActionItem
description: Обновление свойств объекта deviceComplianceActionItem.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c5a80c04ced36a87519217d135257cad640fc29b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861196"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="6f915-103">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="6f915-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="6f915-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6f915-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f915-105">Обновление свойств объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="6f915-105">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f915-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6f915-106">Prerequisites</span></span>
<span data-ttu-id="6f915-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f915-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f915-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f915-109">Permission type</span></span>|<span data-ttu-id="6f915-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f915-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f915-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f915-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6f915-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f915-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f915-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f915-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f915-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f915-114">Not supported.</span></span>|
|<span data-ttu-id="6f915-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f915-115">Application</span></span>|<span data-ttu-id="6f915-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f915-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f915-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f915-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="6f915-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f915-118">Request headers</span></span>
|<span data-ttu-id="6f915-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f915-119">Header</span></span>|<span data-ttu-id="6f915-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6f915-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f915-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f915-121">Authorization</span></span>|<span data-ttu-id="6f915-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6f915-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f915-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6f915-123">Accept</span></span>|<span data-ttu-id="6f915-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6f915-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f915-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f915-125">Request body</span></span>
<span data-ttu-id="6f915-126">В теле запроса добавьте представление объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f915-126">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="6f915-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="6f915-127">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="6f915-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f915-128">Property</span></span>|<span data-ttu-id="6f915-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6f915-129">Type</span></span>|<span data-ttu-id="6f915-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6f915-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f915-131">id</span><span class="sxs-lookup"><span data-stu-id="6f915-131">id</span></span>|<span data-ttu-id="6f915-132">Строка</span><span class="sxs-lookup"><span data-stu-id="6f915-132">String</span></span>|<span data-ttu-id="6f915-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6f915-133">Key of the entity.</span></span>|
|<span data-ttu-id="6f915-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="6f915-134">gracePeriodHours</span></span>|<span data-ttu-id="6f915-135">Int32</span><span class="sxs-lookup"><span data-stu-id="6f915-135">Int32</span></span>|<span data-ttu-id="6f915-136">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="6f915-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="6f915-137">Допустимые значения: от 0 до 8760.</span><span class="sxs-lookup"><span data-stu-id="6f915-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="6f915-138">actionType</span><span class="sxs-lookup"><span data-stu-id="6f915-138">actionType</span></span>|[<span data-ttu-id="6f915-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="6f915-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="6f915-140">Какое действие необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="6f915-140">What action to take.</span></span> <span data-ttu-id="6f915-141">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="6f915-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="6f915-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="6f915-142">notificationTemplateId</span></span>|<span data-ttu-id="6f915-143">String</span><span class="sxs-lookup"><span data-stu-id="6f915-143">String</span></span>|<span data-ttu-id="6f915-144">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="6f915-144">What notification Message template to use</span></span>|
|<span data-ttu-id="6f915-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="6f915-145">notificationMessageCCList</span></span>|<span data-ttu-id="6f915-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6f915-146">String collection</span></span>|<span data-ttu-id="6f915-147">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="6f915-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="6f915-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f915-148">Response</span></span>
<span data-ttu-id="6f915-149">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6f915-149">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f915-150">Пример</span><span class="sxs-lookup"><span data-stu-id="6f915-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f915-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f915-151">Request</span></span>
<span data-ttu-id="6f915-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f915-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
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

### <a name="response"></a><span data-ttu-id="6f915-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f915-153">Response</span></span>
<span data-ttu-id="6f915-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6f915-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



