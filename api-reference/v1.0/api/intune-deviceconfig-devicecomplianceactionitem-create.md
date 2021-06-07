---
title: Создание объекта deviceComplianceActionItem
description: Создание объекта deviceComplianceActionItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3e83ea1386702916a1f14a27e934ea789cca24e7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756675"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="c2071-103">Создание объекта deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="c2071-103">Create deviceComplianceActionItem</span></span>

<span data-ttu-id="c2071-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2071-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2071-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2071-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2071-106">Создание объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="c2071-106">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2071-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c2071-107">Prerequisites</span></span>
<span data-ttu-id="c2071-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2071-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2071-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2071-110">Permission type</span></span>|<span data-ttu-id="c2071-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2071-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2071-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2071-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c2071-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2071-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c2071-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2071-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2071-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2071-115">Not supported.</span></span>|
|<span data-ttu-id="c2071-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c2071-116">Application</span></span>|<span data-ttu-id="c2071-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2071-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2071-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2071-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c2071-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c2071-119">Request headers</span></span>
|<span data-ttu-id="c2071-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2071-120">Header</span></span>|<span data-ttu-id="c2071-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c2071-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2071-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2071-122">Authorization</span></span>|<span data-ttu-id="c2071-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2071-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2071-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c2071-124">Accept</span></span>|<span data-ttu-id="c2071-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c2071-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2071-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2071-126">Request body</span></span>
<span data-ttu-id="c2071-127">В тексте запроса добавьте представление объекта deviceComplianceActionItem в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2071-127">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="c2071-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="c2071-128">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="c2071-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2071-129">Property</span></span>|<span data-ttu-id="c2071-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c2071-130">Type</span></span>|<span data-ttu-id="c2071-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c2071-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2071-132">id</span><span class="sxs-lookup"><span data-stu-id="c2071-132">id</span></span>|<span data-ttu-id="c2071-133">String</span><span class="sxs-lookup"><span data-stu-id="c2071-133">String</span></span>|<span data-ttu-id="c2071-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c2071-134">Key of the entity.</span></span>|
|<span data-ttu-id="c2071-135">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="c2071-135">gracePeriodHours</span></span>|<span data-ttu-id="c2071-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c2071-136">Int32</span></span>|<span data-ttu-id="c2071-137">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="c2071-137">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="c2071-138">Допустимые значения: от 0 до 8760</span><span class="sxs-lookup"><span data-stu-id="c2071-138">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="c2071-139">actionType</span><span class="sxs-lookup"><span data-stu-id="c2071-139">actionType</span></span>|[<span data-ttu-id="c2071-140">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="c2071-140">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="c2071-141">Какие действия необходимо принять.</span><span class="sxs-lookup"><span data-stu-id="c2071-141">What action to take.</span></span> <span data-ttu-id="c2071-142">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="c2071-142">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="c2071-143">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="c2071-143">notificationTemplateId</span></span>|<span data-ttu-id="c2071-144">String</span><span class="sxs-lookup"><span data-stu-id="c2071-144">String</span></span>|<span data-ttu-id="c2071-145">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="c2071-145">What notification Message template to use</span></span>|
|<span data-ttu-id="c2071-146">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="c2071-146">notificationMessageCCList</span></span>|<span data-ttu-id="c2071-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c2071-147">String collection</span></span>|<span data-ttu-id="c2071-148">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="c2071-148">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="c2071-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2071-149">Response</span></span>
<span data-ttu-id="c2071-150">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2071-150">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2071-151">Пример</span><span class="sxs-lookup"><span data-stu-id="c2071-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2071-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2071-152">Request</span></span>
<span data-ttu-id="c2071-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2071-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c2071-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2071-154">Response</span></span>
<span data-ttu-id="c2071-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2071-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




