---
title: Update deviceComplianceActionItem
description: Обновление свойств объекта deviceComplianceActionItem.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 028b8365cd30a39f34dc0cc4dac9867bd122ac07
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979706"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="e5785-103">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="e5785-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="e5785-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5785-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5785-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5785-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5785-106">Обновление свойств объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="e5785-106">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5785-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e5785-107">Prerequisites</span></span>
<span data-ttu-id="e5785-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5785-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5785-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5785-110">Permission type</span></span>|<span data-ttu-id="e5785-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5785-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5785-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5785-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5785-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5785-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e5785-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5785-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5785-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5785-115">Not supported.</span></span>|
|<span data-ttu-id="e5785-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5785-116">Application</span></span>|<span data-ttu-id="e5785-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5785-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5785-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5785-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="e5785-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5785-119">Request headers</span></span>
|<span data-ttu-id="e5785-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5785-120">Header</span></span>|<span data-ttu-id="e5785-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e5785-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5785-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5785-122">Authorization</span></span>|<span data-ttu-id="e5785-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5785-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5785-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e5785-124">Accept</span></span>|<span data-ttu-id="e5785-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e5785-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5785-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5785-126">Request body</span></span>
<span data-ttu-id="e5785-127">В теле запроса добавьте представление объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5785-127">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="e5785-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="e5785-128">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="e5785-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5785-129">Property</span></span>|<span data-ttu-id="e5785-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e5785-130">Type</span></span>|<span data-ttu-id="e5785-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e5785-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5785-132">id</span><span class="sxs-lookup"><span data-stu-id="e5785-132">id</span></span>|<span data-ttu-id="e5785-133">String</span><span class="sxs-lookup"><span data-stu-id="e5785-133">String</span></span>|<span data-ttu-id="e5785-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e5785-134">Key of the entity.</span></span>|
|<span data-ttu-id="e5785-135">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="e5785-135">gracePeriodHours</span></span>|<span data-ttu-id="e5785-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e5785-136">Int32</span></span>|<span data-ttu-id="e5785-137">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="e5785-137">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="e5785-138">Допустимые значения: от 0 до 8760</span><span class="sxs-lookup"><span data-stu-id="e5785-138">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="e5785-139">actionType</span><span class="sxs-lookup"><span data-stu-id="e5785-139">actionType</span></span>|[<span data-ttu-id="e5785-140">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="e5785-140">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="e5785-141">Действия, которые необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="e5785-141">What action to take.</span></span> <span data-ttu-id="e5785-142">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="e5785-142">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="e5785-143">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="e5785-143">notificationTemplateId</span></span>|<span data-ttu-id="e5785-144">String</span><span class="sxs-lookup"><span data-stu-id="e5785-144">String</span></span>|<span data-ttu-id="e5785-145">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="e5785-145">What notification Message template to use</span></span>|
|<span data-ttu-id="e5785-146">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="e5785-146">notificationMessageCCList</span></span>|<span data-ttu-id="e5785-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e5785-147">String collection</span></span>|<span data-ttu-id="e5785-148">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="e5785-148">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="e5785-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5785-149">Response</span></span>
<span data-ttu-id="e5785-150">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e5785-150">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5785-151">Пример</span><span class="sxs-lookup"><span data-stu-id="e5785-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5785-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5785-152">Request</span></span>
<span data-ttu-id="e5785-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5785-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e5785-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5785-154">Response</span></span>
<span data-ttu-id="e5785-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5785-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




