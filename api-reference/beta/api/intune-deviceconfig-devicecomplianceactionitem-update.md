---
title: Update deviceComplianceActionItem
description: Обновление свойств объекта deviceComplianceActionItem.
ms.openlocfilehash: 0f2d94411c88bf4e7d377150ebd59d3056b1f6c7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075939"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="64a2f-103">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="64a2f-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="64a2f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="64a2f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64a2f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64a2f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64a2f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="64a2f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64a2f-107">Обновление свойств объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="64a2f-107">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="64a2f-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="64a2f-108">Prerequisites</span></span>
<span data-ttu-id="64a2f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64a2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64a2f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64a2f-111">Permission type</span></span>|<span data-ttu-id="64a2f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64a2f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64a2f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64a2f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64a2f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64a2f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64a2f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64a2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64a2f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64a2f-116">Not supported.</span></span>|
|<span data-ttu-id="64a2f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64a2f-117">Application</span></span>|<span data-ttu-id="64a2f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64a2f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64a2f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64a2f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="64a2f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64a2f-120">Request headers</span></span>
|<span data-ttu-id="64a2f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64a2f-121">Header</span></span>|<span data-ttu-id="64a2f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="64a2f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64a2f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="64a2f-123">Authorization</span></span>|<span data-ttu-id="64a2f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="64a2f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64a2f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="64a2f-125">Accept</span></span>|<span data-ttu-id="64a2f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64a2f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64a2f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="64a2f-127">Request body</span></span>
<span data-ttu-id="64a2f-128">В теле запроса добавьте представление объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64a2f-128">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="64a2f-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="64a2f-129">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="64a2f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="64a2f-130">Property</span></span>|<span data-ttu-id="64a2f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="64a2f-131">Type</span></span>|<span data-ttu-id="64a2f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="64a2f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64a2f-133">id</span><span class="sxs-lookup"><span data-stu-id="64a2f-133">id</span></span>|<span data-ttu-id="64a2f-134">String</span><span class="sxs-lookup"><span data-stu-id="64a2f-134">String</span></span>|<span data-ttu-id="64a2f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="64a2f-135">Key of the entity.</span></span>|
|<span data-ttu-id="64a2f-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="64a2f-136">gracePeriodHours</span></span>|<span data-ttu-id="64a2f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="64a2f-137">Int32</span></span>|<span data-ttu-id="64a2f-138">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="64a2f-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="64a2f-139">Допустимые значения: от 0 до 8760.</span><span class="sxs-lookup"><span data-stu-id="64a2f-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="64a2f-140">actionType</span><span class="sxs-lookup"><span data-stu-id="64a2f-140">actionType</span></span>|[<span data-ttu-id="64a2f-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="64a2f-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="64a2f-142">Какое действие необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="64a2f-142">What action to take.</span></span> <span data-ttu-id="64a2f-143">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="64a2f-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="64a2f-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="64a2f-144">notificationTemplateId</span></span>|<span data-ttu-id="64a2f-145">String</span><span class="sxs-lookup"><span data-stu-id="64a2f-145">String</span></span>|<span data-ttu-id="64a2f-146">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="64a2f-146">What notification Message template to use</span></span>|
|<span data-ttu-id="64a2f-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="64a2f-147">notificationMessageCCList</span></span>|<span data-ttu-id="64a2f-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="64a2f-148">String collection</span></span>|<span data-ttu-id="64a2f-149">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="64a2f-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="64a2f-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="64a2f-150">Response</span></span>
<span data-ttu-id="64a2f-151">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="64a2f-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64a2f-152">Пример</span><span class="sxs-lookup"><span data-stu-id="64a2f-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="64a2f-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="64a2f-153">Request</span></span>
<span data-ttu-id="64a2f-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64a2f-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
Content-type: application/json
Content-length: 206

{
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="64a2f-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="64a2f-155">Response</span></span>
<span data-ttu-id="64a2f-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="64a2f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





