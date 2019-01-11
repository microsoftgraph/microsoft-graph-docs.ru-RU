---
title: Update deviceComplianceActionItem
description: Обновление свойств объекта deviceComplianceActionItem.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6502980f1bbb5474fd1805ea9d8ec7365befd130
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841974"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="ffe37-103">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="ffe37-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="ffe37-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ffe37-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ffe37-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffe37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ffe37-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ffe37-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffe37-107">Обновление свойств объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="ffe37-107">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ffe37-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ffe37-108">Prerequisites</span></span>
<span data-ttu-id="ffe37-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffe37-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffe37-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffe37-111">Permission type</span></span>|<span data-ttu-id="ffe37-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffe37-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffe37-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffe37-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ffe37-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffe37-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ffe37-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffe37-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffe37-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffe37-116">Not supported.</span></span>|
|<span data-ttu-id="ffe37-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffe37-117">Application</span></span>|<span data-ttu-id="ffe37-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffe37-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffe37-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffe37-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="ffe37-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffe37-120">Request headers</span></span>
|<span data-ttu-id="ffe37-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffe37-121">Header</span></span>|<span data-ttu-id="ffe37-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ffe37-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffe37-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffe37-123">Authorization</span></span>|<span data-ttu-id="ffe37-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ffe37-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffe37-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ffe37-125">Accept</span></span>|<span data-ttu-id="ffe37-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffe37-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffe37-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ffe37-127">Request body</span></span>
<span data-ttu-id="ffe37-128">В теле запроса добавьте представление объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffe37-128">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="ffe37-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="ffe37-129">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="ffe37-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ffe37-130">Property</span></span>|<span data-ttu-id="ffe37-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ffe37-131">Type</span></span>|<span data-ttu-id="ffe37-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ffe37-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffe37-133">id</span><span class="sxs-lookup"><span data-stu-id="ffe37-133">id</span></span>|<span data-ttu-id="ffe37-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ffe37-134">String</span></span>|<span data-ttu-id="ffe37-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ffe37-135">Key of the entity.</span></span>|
|<span data-ttu-id="ffe37-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="ffe37-136">gracePeriodHours</span></span>|<span data-ttu-id="ffe37-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ffe37-137">Int32</span></span>|<span data-ttu-id="ffe37-138">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="ffe37-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="ffe37-139">Допустимые значения: от 0 до 8760.</span><span class="sxs-lookup"><span data-stu-id="ffe37-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="ffe37-140">actionType</span><span class="sxs-lookup"><span data-stu-id="ffe37-140">actionType</span></span>|[<span data-ttu-id="ffe37-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="ffe37-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="ffe37-142">Какое действие необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="ffe37-142">What action to take.</span></span> <span data-ttu-id="ffe37-143">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="ffe37-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="ffe37-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="ffe37-144">notificationTemplateId</span></span>|<span data-ttu-id="ffe37-145">String</span><span class="sxs-lookup"><span data-stu-id="ffe37-145">String</span></span>|<span data-ttu-id="ffe37-146">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="ffe37-146">What notification Message template to use</span></span>|
|<span data-ttu-id="ffe37-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="ffe37-147">notificationMessageCCList</span></span>|<span data-ttu-id="ffe37-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ffe37-148">String collection</span></span>|<span data-ttu-id="ffe37-149">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="ffe37-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="ffe37-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="ffe37-150">Response</span></span>
<span data-ttu-id="ffe37-151">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ffe37-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffe37-152">Пример</span><span class="sxs-lookup"><span data-stu-id="ffe37-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="ffe37-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffe37-153">Request</span></span>
<span data-ttu-id="ffe37-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffe37-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ffe37-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="ffe37-155">Response</span></span>
<span data-ttu-id="ffe37-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ffe37-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





