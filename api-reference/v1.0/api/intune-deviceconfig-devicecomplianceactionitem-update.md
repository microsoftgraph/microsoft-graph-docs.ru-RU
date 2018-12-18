---
title: Update deviceComplianceActionItem
description: Обновление свойств объекта deviceComplianceActionItem.
author: tfitzmac
ms.openlocfilehash: c3d3124b01bd6c15ff0519baac0920d7e59cc9bd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361833"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="0387e-103">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="0387e-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="0387e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0387e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0387e-105">Обновление свойств объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="0387e-105">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0387e-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0387e-106">Prerequisites</span></span>
<span data-ttu-id="0387e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0387e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0387e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0387e-109">Permission type</span></span>|<span data-ttu-id="0387e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0387e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0387e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0387e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0387e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0387e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0387e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0387e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0387e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0387e-114">Not supported.</span></span>|
|<span data-ttu-id="0387e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0387e-115">Application</span></span>|<span data-ttu-id="0387e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0387e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0387e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0387e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="0387e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0387e-118">Request headers</span></span>
|<span data-ttu-id="0387e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0387e-119">Header</span></span>|<span data-ttu-id="0387e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0387e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0387e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0387e-121">Authorization</span></span>|<span data-ttu-id="0387e-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0387e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0387e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0387e-123">Accept</span></span>|<span data-ttu-id="0387e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0387e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0387e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0387e-125">Request body</span></span>
<span data-ttu-id="0387e-126">В теле запроса добавьте представление объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0387e-126">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="0387e-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="0387e-127">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="0387e-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="0387e-128">Property</span></span>|<span data-ttu-id="0387e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0387e-129">Type</span></span>|<span data-ttu-id="0387e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0387e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0387e-131">id</span><span class="sxs-lookup"><span data-stu-id="0387e-131">id</span></span>|<span data-ttu-id="0387e-132">Строка</span><span class="sxs-lookup"><span data-stu-id="0387e-132">String</span></span>|<span data-ttu-id="0387e-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0387e-133">Key of the entity.</span></span>|
|<span data-ttu-id="0387e-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="0387e-134">gracePeriodHours</span></span>|<span data-ttu-id="0387e-135">Int32</span><span class="sxs-lookup"><span data-stu-id="0387e-135">Int32</span></span>|<span data-ttu-id="0387e-136">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="0387e-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="0387e-137">Допустимые значения: от 0 до 8760.</span><span class="sxs-lookup"><span data-stu-id="0387e-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="0387e-138">actionType</span><span class="sxs-lookup"><span data-stu-id="0387e-138">actionType</span></span>|[<span data-ttu-id="0387e-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="0387e-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="0387e-140">Какое действие необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="0387e-140">What action to take.</span></span> <span data-ttu-id="0387e-141">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="0387e-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="0387e-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="0387e-142">notificationTemplateId</span></span>|<span data-ttu-id="0387e-143">String</span><span class="sxs-lookup"><span data-stu-id="0387e-143">String</span></span>|<span data-ttu-id="0387e-144">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="0387e-144">What notification Message template to use</span></span>|
|<span data-ttu-id="0387e-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="0387e-145">notificationMessageCCList</span></span>|<span data-ttu-id="0387e-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0387e-146">String collection</span></span>|<span data-ttu-id="0387e-147">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="0387e-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="0387e-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="0387e-148">Response</span></span>
<span data-ttu-id="0387e-149">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0387e-149">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0387e-150">Пример</span><span class="sxs-lookup"><span data-stu-id="0387e-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="0387e-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="0387e-151">Request</span></span>
<span data-ttu-id="0387e-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0387e-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0387e-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="0387e-153">Response</span></span>
<span data-ttu-id="0387e-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0387e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



