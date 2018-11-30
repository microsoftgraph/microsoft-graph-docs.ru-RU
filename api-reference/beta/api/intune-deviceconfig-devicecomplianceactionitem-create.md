---
title: Создание объекта deviceComplianceActionItem
description: Создание объекта deviceComplianceActionItem.
ms.openlocfilehash: edb99b2fac02b95ebd2634749bdaa8d4acfec781
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079301"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="2f02a-103">Создание объекта deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="2f02a-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="2f02a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2f02a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f02a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f02a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f02a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2f02a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f02a-107">Создание объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="2f02a-107">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f02a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2f02a-108">Prerequisites</span></span>
<span data-ttu-id="2f02a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f02a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f02a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f02a-111">Permission type</span></span>|<span data-ttu-id="2f02a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f02a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f02a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f02a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f02a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f02a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f02a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f02a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f02a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f02a-116">Not supported.</span></span>|
|<span data-ttu-id="2f02a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f02a-117">Application</span></span>|<span data-ttu-id="2f02a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f02a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f02a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f02a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2f02a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f02a-120">Request headers</span></span>
|<span data-ttu-id="2f02a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f02a-121">Header</span></span>|<span data-ttu-id="2f02a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2f02a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f02a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f02a-123">Authorization</span></span>|<span data-ttu-id="2f02a-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2f02a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f02a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2f02a-125">Accept</span></span>|<span data-ttu-id="2f02a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f02a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f02a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f02a-127">Request body</span></span>
<span data-ttu-id="2f02a-128">В тексте запроса добавьте представление объекта deviceComplianceActionItem в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f02a-128">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="2f02a-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="2f02a-129">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="2f02a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f02a-130">Property</span></span>|<span data-ttu-id="2f02a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2f02a-131">Type</span></span>|<span data-ttu-id="2f02a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2f02a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f02a-133">id</span><span class="sxs-lookup"><span data-stu-id="2f02a-133">id</span></span>|<span data-ttu-id="2f02a-134">String</span><span class="sxs-lookup"><span data-stu-id="2f02a-134">String</span></span>|<span data-ttu-id="2f02a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2f02a-135">Key of the entity.</span></span>|
|<span data-ttu-id="2f02a-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="2f02a-136">gracePeriodHours</span></span>|<span data-ttu-id="2f02a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="2f02a-137">Int32</span></span>|<span data-ttu-id="2f02a-138">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="2f02a-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="2f02a-139">Допустимые значения: от 0 до 8760.</span><span class="sxs-lookup"><span data-stu-id="2f02a-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="2f02a-140">actionType</span><span class="sxs-lookup"><span data-stu-id="2f02a-140">actionType</span></span>|[<span data-ttu-id="2f02a-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="2f02a-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="2f02a-142">Какое действие необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="2f02a-142">What action to take.</span></span> <span data-ttu-id="2f02a-143">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="2f02a-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="2f02a-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="2f02a-144">notificationTemplateId</span></span>|<span data-ttu-id="2f02a-145">String</span><span class="sxs-lookup"><span data-stu-id="2f02a-145">String</span></span>|<span data-ttu-id="2f02a-146">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="2f02a-146">What notification Message template to use</span></span>|
|<span data-ttu-id="2f02a-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="2f02a-147">notificationMessageCCList</span></span>|<span data-ttu-id="2f02a-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2f02a-148">String collection</span></span>|<span data-ttu-id="2f02a-149">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="2f02a-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="2f02a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f02a-150">Response</span></span>
<span data-ttu-id="2f02a-151">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f02a-151">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f02a-152">Пример</span><span class="sxs-lookup"><span data-stu-id="2f02a-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f02a-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f02a-153">Request</span></span>
<span data-ttu-id="2f02a-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f02a-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
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

### <a name="response"></a><span data-ttu-id="2f02a-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f02a-155">Response</span></span>
<span data-ttu-id="2f02a-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="2f02a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





