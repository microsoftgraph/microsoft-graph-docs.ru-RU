---
title: Создание объекта deviceComplianceActionItem
description: Создание объекта deviceComplianceActionItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4cb1e72e65c362aafa875a0789cf797fb1f0f7a4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155717"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="7f2a7-103">Создание объекта deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="7f2a7-103">Create deviceComplianceActionItem</span></span>

<span data-ttu-id="7f2a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f2a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f2a7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f2a7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f2a7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f2a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f2a7-107">Создание объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="7f2a7-107">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f2a7-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7f2a7-108">Prerequisites</span></span>
<span data-ttu-id="7f2a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f2a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f2a7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f2a7-111">Permission type</span></span>|<span data-ttu-id="7f2a7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f2a7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f2a7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f2a7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f2a7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f2a7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7f2a7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f2a7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f2a7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f2a7-116">Not supported.</span></span>|
|<span data-ttu-id="7f2a7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7f2a7-117">Application</span></span>|<span data-ttu-id="7f2a7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f2a7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f2a7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f2a7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7f2a7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7f2a7-120">Request headers</span></span>
|<span data-ttu-id="7f2a7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f2a7-121">Header</span></span>|<span data-ttu-id="7f2a7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7f2a7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f2a7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f2a7-123">Authorization</span></span>|<span data-ttu-id="7f2a7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f2a7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f2a7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7f2a7-125">Accept</span></span>|<span data-ttu-id="7f2a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f2a7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f2a7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f2a7-127">Request body</span></span>
<span data-ttu-id="7f2a7-128">В тексте запроса добавьте представление объекта deviceComplianceActionItem в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f2a7-128">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="7f2a7-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="7f2a7-129">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="7f2a7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f2a7-130">Property</span></span>|<span data-ttu-id="7f2a7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7f2a7-131">Type</span></span>|<span data-ttu-id="7f2a7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7f2a7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f2a7-133">id</span><span class="sxs-lookup"><span data-stu-id="7f2a7-133">id</span></span>|<span data-ttu-id="7f2a7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7f2a7-134">String</span></span>|<span data-ttu-id="7f2a7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7f2a7-135">Key of the entity.</span></span>|
|<span data-ttu-id="7f2a7-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="7f2a7-136">gracePeriodHours</span></span>|<span data-ttu-id="7f2a7-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7f2a7-137">Int32</span></span>|<span data-ttu-id="7f2a7-138">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="7f2a7-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="7f2a7-139">Допустимые значения: от 0 до 8760</span><span class="sxs-lookup"><span data-stu-id="7f2a7-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="7f2a7-140">actionType</span><span class="sxs-lookup"><span data-stu-id="7f2a7-140">actionType</span></span>|[<span data-ttu-id="7f2a7-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="7f2a7-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="7f2a7-142">Какие действия необходимо принять.</span><span class="sxs-lookup"><span data-stu-id="7f2a7-142">What action to take.</span></span> <span data-ttu-id="7f2a7-143">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="7f2a7-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="7f2a7-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="7f2a7-144">notificationTemplateId</span></span>|<span data-ttu-id="7f2a7-145">String</span><span class="sxs-lookup"><span data-stu-id="7f2a7-145">String</span></span>|<span data-ttu-id="7f2a7-146">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="7f2a7-146">What notification Message template to use</span></span>|
|<span data-ttu-id="7f2a7-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="7f2a7-147">notificationMessageCCList</span></span>|<span data-ttu-id="7f2a7-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7f2a7-148">String collection</span></span>|<span data-ttu-id="7f2a7-149">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="7f2a7-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="7f2a7-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f2a7-150">Response</span></span>
<span data-ttu-id="7f2a7-151">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f2a7-151">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f2a7-152">Пример</span><span class="sxs-lookup"><span data-stu-id="7f2a7-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f2a7-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f2a7-153">Request</span></span>
<span data-ttu-id="7f2a7-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f2a7-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7f2a7-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f2a7-155">Response</span></span>
<span data-ttu-id="7f2a7-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f2a7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




