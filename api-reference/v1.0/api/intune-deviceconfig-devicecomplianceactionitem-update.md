---
title: Update deviceComplianceActionItem
description: Обновление свойств объекта deviceComplianceActionItem.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 112a9f77af4ea5daba53253002a239d93fc374b6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515149"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="9404a-103">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="9404a-103">Update deviceComplianceActionItem</span></span>

<span data-ttu-id="9404a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9404a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9404a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9404a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9404a-106">Обновление свойств объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="9404a-106">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9404a-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9404a-107">Prerequisites</span></span>
<span data-ttu-id="9404a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9404a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9404a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9404a-110">Permission type</span></span>|<span data-ttu-id="9404a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9404a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9404a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9404a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9404a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9404a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9404a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9404a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9404a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9404a-115">Not supported.</span></span>|
|<span data-ttu-id="9404a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9404a-116">Application</span></span>|<span data-ttu-id="9404a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9404a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9404a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9404a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="9404a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9404a-119">Request headers</span></span>
|<span data-ttu-id="9404a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9404a-120">Header</span></span>|<span data-ttu-id="9404a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9404a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9404a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9404a-122">Authorization</span></span>|<span data-ttu-id="9404a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9404a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9404a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9404a-124">Accept</span></span>|<span data-ttu-id="9404a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9404a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9404a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9404a-126">Request body</span></span>
<span data-ttu-id="9404a-127">В теле запроса добавьте представление объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9404a-127">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="9404a-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="9404a-128">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="9404a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9404a-129">Property</span></span>|<span data-ttu-id="9404a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9404a-130">Type</span></span>|<span data-ttu-id="9404a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9404a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9404a-132">id</span><span class="sxs-lookup"><span data-stu-id="9404a-132">id</span></span>|<span data-ttu-id="9404a-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9404a-133">String</span></span>|<span data-ttu-id="9404a-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9404a-134">Key of the entity.</span></span>|
|<span data-ttu-id="9404a-135">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="9404a-135">gracePeriodHours</span></span>|<span data-ttu-id="9404a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="9404a-136">Int32</span></span>|<span data-ttu-id="9404a-137">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="9404a-137">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="9404a-138">Допустимые значения: от 0 до 8760</span><span class="sxs-lookup"><span data-stu-id="9404a-138">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="9404a-139">actionType</span><span class="sxs-lookup"><span data-stu-id="9404a-139">actionType</span></span>|[<span data-ttu-id="9404a-140">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="9404a-140">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="9404a-141">Действия, которые необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="9404a-141">What action to take.</span></span> <span data-ttu-id="9404a-142">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="9404a-142">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="9404a-143">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="9404a-143">notificationTemplateId</span></span>|<span data-ttu-id="9404a-144">String</span><span class="sxs-lookup"><span data-stu-id="9404a-144">String</span></span>|<span data-ttu-id="9404a-145">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="9404a-145">What notification Message template to use</span></span>|
|<span data-ttu-id="9404a-146">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="9404a-146">notificationMessageCCList</span></span>|<span data-ttu-id="9404a-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9404a-147">String collection</span></span>|<span data-ttu-id="9404a-148">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="9404a-148">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="9404a-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="9404a-149">Response</span></span>
<span data-ttu-id="9404a-150">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9404a-150">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9404a-151">Пример</span><span class="sxs-lookup"><span data-stu-id="9404a-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="9404a-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="9404a-152">Request</span></span>
<span data-ttu-id="9404a-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9404a-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9404a-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="9404a-154">Response</span></span>
<span data-ttu-id="9404a-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9404a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




