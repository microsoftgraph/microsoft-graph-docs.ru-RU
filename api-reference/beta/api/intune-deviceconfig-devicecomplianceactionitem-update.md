---
title: Update deviceComplianceActionItem
description: Обновление свойств объекта deviceComplianceActionItem.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 77f1292e240d8d8887adff98aa9326685659bb77
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404976"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="98419-103">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="98419-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="98419-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="98419-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="98419-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98419-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98419-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98419-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98419-107">Обновление свойств объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="98419-107">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98419-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="98419-108">Prerequisites</span></span>
<span data-ttu-id="98419-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="98419-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="98419-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98419-111">Permission type</span></span>|<span data-ttu-id="98419-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="98419-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98419-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98419-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98419-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98419-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="98419-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98419-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98419-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98419-116">Not supported.</span></span>|
|<span data-ttu-id="98419-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98419-117">Application</span></span>|<span data-ttu-id="98419-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98419-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98419-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98419-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="98419-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98419-120">Request headers</span></span>
|<span data-ttu-id="98419-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98419-121">Header</span></span>|<span data-ttu-id="98419-122">Значение</span><span class="sxs-lookup"><span data-stu-id="98419-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98419-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="98419-123">Authorization</span></span>|<span data-ttu-id="98419-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="98419-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98419-125">Accept</span><span class="sxs-lookup"><span data-stu-id="98419-125">Accept</span></span>|<span data-ttu-id="98419-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98419-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98419-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="98419-127">Request body</span></span>
<span data-ttu-id="98419-128">В теле запроса добавьте представление объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98419-128">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="98419-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="98419-129">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="98419-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="98419-130">Property</span></span>|<span data-ttu-id="98419-131">Тип</span><span class="sxs-lookup"><span data-stu-id="98419-131">Type</span></span>|<span data-ttu-id="98419-132">Описание</span><span class="sxs-lookup"><span data-stu-id="98419-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98419-133">id</span><span class="sxs-lookup"><span data-stu-id="98419-133">id</span></span>|<span data-ttu-id="98419-134">String</span><span class="sxs-lookup"><span data-stu-id="98419-134">String</span></span>|<span data-ttu-id="98419-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="98419-135">Key of the entity.</span></span>|
|<span data-ttu-id="98419-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="98419-136">gracePeriodHours</span></span>|<span data-ttu-id="98419-137">Int32</span><span class="sxs-lookup"><span data-stu-id="98419-137">Int32</span></span>|<span data-ttu-id="98419-138">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="98419-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="98419-139">Допустимые значения: от 0 до 8760.</span><span class="sxs-lookup"><span data-stu-id="98419-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="98419-140">actionType</span><span class="sxs-lookup"><span data-stu-id="98419-140">actionType</span></span>|[<span data-ttu-id="98419-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="98419-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="98419-142">Какое действие необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="98419-142">What action to take.</span></span> <span data-ttu-id="98419-143">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="98419-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="98419-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="98419-144">notificationTemplateId</span></span>|<span data-ttu-id="98419-145">String</span><span class="sxs-lookup"><span data-stu-id="98419-145">String</span></span>|<span data-ttu-id="98419-146">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="98419-146">What notification Message template to use</span></span>|
|<span data-ttu-id="98419-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="98419-147">notificationMessageCCList</span></span>|<span data-ttu-id="98419-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="98419-148">String collection</span></span>|<span data-ttu-id="98419-149">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="98419-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="98419-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="98419-150">Response</span></span>
<span data-ttu-id="98419-151">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="98419-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98419-152">Пример</span><span class="sxs-lookup"><span data-stu-id="98419-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="98419-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="98419-153">Request</span></span>
<span data-ttu-id="98419-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98419-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="98419-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="98419-155">Response</span></span>
<span data-ttu-id="98419-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="98419-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




