---
title: Update deviceComplianceActionItem
description: Обновление свойств объекта deviceComplianceActionItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26f673b8abdf9bb99d417eb9fbcb7e3565324081
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048066"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="d70b5-103">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="d70b5-103">Update deviceComplianceActionItem</span></span>

<span data-ttu-id="d70b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d70b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d70b5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d70b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d70b5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d70b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d70b5-107">Обновление свойств объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="d70b5-107">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d70b5-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d70b5-108">Prerequisites</span></span>
<span data-ttu-id="d70b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d70b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d70b5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d70b5-111">Permission type</span></span>|<span data-ttu-id="d70b5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d70b5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d70b5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d70b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d70b5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d70b5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d70b5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d70b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d70b5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d70b5-116">Not supported.</span></span>|
|<span data-ttu-id="d70b5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d70b5-117">Application</span></span>|<span data-ttu-id="d70b5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d70b5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d70b5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d70b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="d70b5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d70b5-120">Request headers</span></span>
|<span data-ttu-id="d70b5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d70b5-121">Header</span></span>|<span data-ttu-id="d70b5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d70b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d70b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d70b5-123">Authorization</span></span>|<span data-ttu-id="d70b5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d70b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d70b5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d70b5-125">Accept</span></span>|<span data-ttu-id="d70b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d70b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d70b5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d70b5-127">Request body</span></span>
<span data-ttu-id="d70b5-128">В теле запроса добавьте представление объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d70b5-128">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="d70b5-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="d70b5-129">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="d70b5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d70b5-130">Property</span></span>|<span data-ttu-id="d70b5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d70b5-131">Type</span></span>|<span data-ttu-id="d70b5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d70b5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d70b5-133">id</span><span class="sxs-lookup"><span data-stu-id="d70b5-133">id</span></span>|<span data-ttu-id="d70b5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d70b5-134">String</span></span>|<span data-ttu-id="d70b5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d70b5-135">Key of the entity.</span></span>|
|<span data-ttu-id="d70b5-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="d70b5-136">gracePeriodHours</span></span>|<span data-ttu-id="d70b5-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d70b5-137">Int32</span></span>|<span data-ttu-id="d70b5-138">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="d70b5-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="d70b5-139">Допустимые значения: от 0 до 8760</span><span class="sxs-lookup"><span data-stu-id="d70b5-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="d70b5-140">actionType</span><span class="sxs-lookup"><span data-stu-id="d70b5-140">actionType</span></span>|[<span data-ttu-id="d70b5-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="d70b5-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="d70b5-142">Действия, которые необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="d70b5-142">What action to take.</span></span> <span data-ttu-id="d70b5-143">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="d70b5-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="d70b5-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="d70b5-144">notificationTemplateId</span></span>|<span data-ttu-id="d70b5-145">String</span><span class="sxs-lookup"><span data-stu-id="d70b5-145">String</span></span>|<span data-ttu-id="d70b5-146">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="d70b5-146">What notification Message template to use</span></span>|
|<span data-ttu-id="d70b5-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="d70b5-147">notificationMessageCCList</span></span>|<span data-ttu-id="d70b5-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d70b5-148">String collection</span></span>|<span data-ttu-id="d70b5-149">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="d70b5-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="d70b5-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="d70b5-150">Response</span></span>
<span data-ttu-id="d70b5-151">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d70b5-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d70b5-152">Пример</span><span class="sxs-lookup"><span data-stu-id="d70b5-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="d70b5-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="d70b5-153">Request</span></span>
<span data-ttu-id="d70b5-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d70b5-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
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

### <a name="response"></a><span data-ttu-id="d70b5-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="d70b5-155">Response</span></span>
<span data-ttu-id="d70b5-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d70b5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






