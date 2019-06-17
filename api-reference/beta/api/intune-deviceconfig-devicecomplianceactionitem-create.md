---
title: Создание объекта deviceComplianceActionItem
description: Создание объекта deviceComplianceActionItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9807dc7dbb09d64ae0af3770155812747cc37cec
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968646"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="74338-103">Создание объекта deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="74338-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="74338-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74338-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74338-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74338-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74338-106">Создание объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="74338-106">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74338-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="74338-107">Prerequisites</span></span>
<span data-ttu-id="74338-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74338-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74338-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74338-110">Permission type</span></span>|<span data-ttu-id="74338-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="74338-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74338-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74338-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74338-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74338-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74338-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74338-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74338-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74338-115">Not supported.</span></span>|
|<span data-ttu-id="74338-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74338-116">Application</span></span>|<span data-ttu-id="74338-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74338-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74338-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74338-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="74338-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74338-119">Request headers</span></span>
|<span data-ttu-id="74338-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="74338-120">Header</span></span>|<span data-ttu-id="74338-121">Значение</span><span class="sxs-lookup"><span data-stu-id="74338-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74338-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74338-122">Authorization</span></span>|<span data-ttu-id="74338-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="74338-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74338-124">Accept</span><span class="sxs-lookup"><span data-stu-id="74338-124">Accept</span></span>|<span data-ttu-id="74338-125">application/json</span><span class="sxs-lookup"><span data-stu-id="74338-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74338-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="74338-126">Request body</span></span>
<span data-ttu-id="74338-127">В тексте запроса добавьте представление объекта deviceComplianceActionItem в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74338-127">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="74338-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="74338-128">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="74338-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="74338-129">Property</span></span>|<span data-ttu-id="74338-130">Тип</span><span class="sxs-lookup"><span data-stu-id="74338-130">Type</span></span>|<span data-ttu-id="74338-131">Описание</span><span class="sxs-lookup"><span data-stu-id="74338-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74338-132">id</span><span class="sxs-lookup"><span data-stu-id="74338-132">id</span></span>|<span data-ttu-id="74338-133">String</span><span class="sxs-lookup"><span data-stu-id="74338-133">String</span></span>|<span data-ttu-id="74338-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="74338-134">Key of the entity.</span></span>|
|<span data-ttu-id="74338-135">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="74338-135">gracePeriodHours</span></span>|<span data-ttu-id="74338-136">Int32</span><span class="sxs-lookup"><span data-stu-id="74338-136">Int32</span></span>|<span data-ttu-id="74338-137">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="74338-137">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="74338-138">Допустимые значения: от 0 до 8760</span><span class="sxs-lookup"><span data-stu-id="74338-138">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="74338-139">actionType</span><span class="sxs-lookup"><span data-stu-id="74338-139">actionType</span></span>|[<span data-ttu-id="74338-140">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="74338-140">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="74338-141">Действия, которые необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="74338-141">What action to take.</span></span> <span data-ttu-id="74338-142">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="74338-142">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="74338-143">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="74338-143">notificationTemplateId</span></span>|<span data-ttu-id="74338-144">String</span><span class="sxs-lookup"><span data-stu-id="74338-144">String</span></span>|<span data-ttu-id="74338-145">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="74338-145">What notification Message template to use</span></span>|
|<span data-ttu-id="74338-146">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="74338-146">notificationMessageCCList</span></span>|<span data-ttu-id="74338-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="74338-147">String collection</span></span>|<span data-ttu-id="74338-148">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="74338-148">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="74338-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="74338-149">Response</span></span>
<span data-ttu-id="74338-150">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="74338-150">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74338-151">Пример</span><span class="sxs-lookup"><span data-stu-id="74338-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="74338-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="74338-152">Request</span></span>
<span data-ttu-id="74338-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="74338-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="74338-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="74338-154">Response</span></span>
<span data-ttu-id="74338-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="74338-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





