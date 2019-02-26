---
title: Update deviceComplianceActionItem
description: Обновление свойств объекта deviceComplianceActionItem.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5da502820ccf13b0494a6914811db698ff8abc65
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254025"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="daf09-103">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="daf09-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="daf09-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="daf09-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="daf09-105">Обновление свойств объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="daf09-105">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="daf09-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="daf09-106">Prerequisites</span></span>
<span data-ttu-id="daf09-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="daf09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="daf09-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="daf09-109">Permission type</span></span>|<span data-ttu-id="daf09-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="daf09-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="daf09-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="daf09-111">Delegated (work or school account)</span></span>|<span data-ttu-id="daf09-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daf09-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="daf09-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="daf09-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="daf09-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="daf09-114">Not supported.</span></span>|
|<span data-ttu-id="daf09-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="daf09-115">Application</span></span>|<span data-ttu-id="daf09-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="daf09-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="daf09-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="daf09-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="daf09-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="daf09-118">Request headers</span></span>
|<span data-ttu-id="daf09-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="daf09-119">Header</span></span>|<span data-ttu-id="daf09-120">Значение</span><span class="sxs-lookup"><span data-stu-id="daf09-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="daf09-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="daf09-121">Authorization</span></span>|<span data-ttu-id="daf09-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="daf09-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="daf09-123">Accept</span><span class="sxs-lookup"><span data-stu-id="daf09-123">Accept</span></span>|<span data-ttu-id="daf09-124">application/json</span><span class="sxs-lookup"><span data-stu-id="daf09-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="daf09-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="daf09-125">Request body</span></span>
<span data-ttu-id="daf09-126">В теле запроса добавьте представление объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="daf09-126">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="daf09-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="daf09-127">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="daf09-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="daf09-128">Property</span></span>|<span data-ttu-id="daf09-129">Тип</span><span class="sxs-lookup"><span data-stu-id="daf09-129">Type</span></span>|<span data-ttu-id="daf09-130">Описание</span><span class="sxs-lookup"><span data-stu-id="daf09-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daf09-131">id</span><span class="sxs-lookup"><span data-stu-id="daf09-131">id</span></span>|<span data-ttu-id="daf09-132">Строка</span><span class="sxs-lookup"><span data-stu-id="daf09-132">String</span></span>|<span data-ttu-id="daf09-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="daf09-133">Key of the entity.</span></span>|
|<span data-ttu-id="daf09-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="daf09-134">gracePeriodHours</span></span>|<span data-ttu-id="daf09-135">Int32</span><span class="sxs-lookup"><span data-stu-id="daf09-135">Int32</span></span>|<span data-ttu-id="daf09-136">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="daf09-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="daf09-137">Допустимые значения: от 0 до 8760.</span><span class="sxs-lookup"><span data-stu-id="daf09-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="daf09-138">actionType</span><span class="sxs-lookup"><span data-stu-id="daf09-138">actionType</span></span>|[<span data-ttu-id="daf09-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="daf09-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="daf09-140">Действия, которые необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="daf09-140">What action to take.</span></span> <span data-ttu-id="daf09-141">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="daf09-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="daf09-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="daf09-142">notificationTemplateId</span></span>|<span data-ttu-id="daf09-143">String</span><span class="sxs-lookup"><span data-stu-id="daf09-143">String</span></span>|<span data-ttu-id="daf09-144">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="daf09-144">What notification Message template to use</span></span>|
|<span data-ttu-id="daf09-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="daf09-145">notificationMessageCCList</span></span>|<span data-ttu-id="daf09-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="daf09-146">String collection</span></span>|<span data-ttu-id="daf09-147">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="daf09-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="daf09-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="daf09-148">Response</span></span>
<span data-ttu-id="daf09-149">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="daf09-149">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daf09-150">Пример</span><span class="sxs-lookup"><span data-stu-id="daf09-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="daf09-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="daf09-151">Request</span></span>
<span data-ttu-id="daf09-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="daf09-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="daf09-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="daf09-153">Response</span></span>
<span data-ttu-id="daf09-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="daf09-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



