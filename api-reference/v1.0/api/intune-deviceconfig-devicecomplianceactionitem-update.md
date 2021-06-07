---
title: Update deviceComplianceActionItem
description: Обновление свойств объекта deviceComplianceActionItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eb7c4c3c35b0bf75a6ed84805029a15cea9aff33
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756654"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="25d10-103">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="25d10-103">Update deviceComplianceActionItem</span></span>

<span data-ttu-id="25d10-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25d10-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25d10-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25d10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25d10-106">Обновление свойств объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="25d10-106">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25d10-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="25d10-107">Prerequisites</span></span>
<span data-ttu-id="25d10-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25d10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25d10-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25d10-110">Permission type</span></span>|<span data-ttu-id="25d10-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25d10-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25d10-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25d10-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25d10-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25d10-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="25d10-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25d10-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25d10-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25d10-115">Not supported.</span></span>|
|<span data-ttu-id="25d10-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="25d10-116">Application</span></span>|<span data-ttu-id="25d10-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25d10-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="25d10-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25d10-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="25d10-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="25d10-119">Request headers</span></span>
|<span data-ttu-id="25d10-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25d10-120">Header</span></span>|<span data-ttu-id="25d10-121">Значение</span><span class="sxs-lookup"><span data-stu-id="25d10-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25d10-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="25d10-122">Authorization</span></span>|<span data-ttu-id="25d10-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25d10-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25d10-124">Accept</span><span class="sxs-lookup"><span data-stu-id="25d10-124">Accept</span></span>|<span data-ttu-id="25d10-125">application/json</span><span class="sxs-lookup"><span data-stu-id="25d10-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25d10-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25d10-126">Request body</span></span>
<span data-ttu-id="25d10-127">В теле запроса добавьте представление объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25d10-127">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="25d10-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="25d10-128">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="25d10-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="25d10-129">Property</span></span>|<span data-ttu-id="25d10-130">Тип</span><span class="sxs-lookup"><span data-stu-id="25d10-130">Type</span></span>|<span data-ttu-id="25d10-131">Описание</span><span class="sxs-lookup"><span data-stu-id="25d10-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25d10-132">id</span><span class="sxs-lookup"><span data-stu-id="25d10-132">id</span></span>|<span data-ttu-id="25d10-133">String</span><span class="sxs-lookup"><span data-stu-id="25d10-133">String</span></span>|<span data-ttu-id="25d10-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="25d10-134">Key of the entity.</span></span>|
|<span data-ttu-id="25d10-135">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="25d10-135">gracePeriodHours</span></span>|<span data-ttu-id="25d10-136">Int32</span><span class="sxs-lookup"><span data-stu-id="25d10-136">Int32</span></span>|<span data-ttu-id="25d10-137">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="25d10-137">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="25d10-138">Допустимые значения: от 0 до 8760</span><span class="sxs-lookup"><span data-stu-id="25d10-138">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="25d10-139">actionType</span><span class="sxs-lookup"><span data-stu-id="25d10-139">actionType</span></span>|[<span data-ttu-id="25d10-140">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="25d10-140">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="25d10-141">Какие действия необходимо принять.</span><span class="sxs-lookup"><span data-stu-id="25d10-141">What action to take.</span></span> <span data-ttu-id="25d10-142">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="25d10-142">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="25d10-143">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="25d10-143">notificationTemplateId</span></span>|<span data-ttu-id="25d10-144">String</span><span class="sxs-lookup"><span data-stu-id="25d10-144">String</span></span>|<span data-ttu-id="25d10-145">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="25d10-145">What notification Message template to use</span></span>|
|<span data-ttu-id="25d10-146">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="25d10-146">notificationMessageCCList</span></span>|<span data-ttu-id="25d10-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="25d10-147">String collection</span></span>|<span data-ttu-id="25d10-148">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="25d10-148">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="25d10-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="25d10-149">Response</span></span>
<span data-ttu-id="25d10-150">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="25d10-150">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25d10-151">Пример</span><span class="sxs-lookup"><span data-stu-id="25d10-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="25d10-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="25d10-152">Request</span></span>
<span data-ttu-id="25d10-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25d10-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="25d10-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="25d10-154">Response</span></span>
<span data-ttu-id="25d10-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25d10-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




