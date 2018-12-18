---
title: Создание объекта deviceComplianceActionItem
description: Создание объекта deviceComplianceActionItem.
author: tfitzmac
ms.openlocfilehash: a4e0facb0a9d34d840b6ef737c09737c9a6626a4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317978"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="77de1-103">Создание объекта deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="77de1-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="77de1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="77de1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77de1-105">Создание объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="77de1-105">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="77de1-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="77de1-106">Prerequisites</span></span>
<span data-ttu-id="77de1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77de1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77de1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77de1-109">Permission type</span></span>|<span data-ttu-id="77de1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="77de1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77de1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77de1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="77de1-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77de1-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="77de1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77de1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77de1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77de1-114">Not supported.</span></span>|
|<span data-ttu-id="77de1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77de1-115">Application</span></span>|<span data-ttu-id="77de1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77de1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77de1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77de1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="77de1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77de1-118">Request headers</span></span>
|<span data-ttu-id="77de1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="77de1-119">Header</span></span>|<span data-ttu-id="77de1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="77de1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77de1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77de1-121">Authorization</span></span>|<span data-ttu-id="77de1-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="77de1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77de1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="77de1-123">Accept</span></span>|<span data-ttu-id="77de1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="77de1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77de1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77de1-125">Request body</span></span>
<span data-ttu-id="77de1-126">В тексте запроса добавьте представление объекта deviceComplianceActionItem в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77de1-126">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="77de1-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="77de1-127">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="77de1-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="77de1-128">Property</span></span>|<span data-ttu-id="77de1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="77de1-129">Type</span></span>|<span data-ttu-id="77de1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="77de1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77de1-131">id</span><span class="sxs-lookup"><span data-stu-id="77de1-131">id</span></span>|<span data-ttu-id="77de1-132">Строка</span><span class="sxs-lookup"><span data-stu-id="77de1-132">String</span></span>|<span data-ttu-id="77de1-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="77de1-133">Key of the entity.</span></span>|
|<span data-ttu-id="77de1-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="77de1-134">gracePeriodHours</span></span>|<span data-ttu-id="77de1-135">Int32</span><span class="sxs-lookup"><span data-stu-id="77de1-135">Int32</span></span>|<span data-ttu-id="77de1-136">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="77de1-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="77de1-137">Допустимые значения: от 0 до 8760.</span><span class="sxs-lookup"><span data-stu-id="77de1-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="77de1-138">actionType</span><span class="sxs-lookup"><span data-stu-id="77de1-138">actionType</span></span>|[<span data-ttu-id="77de1-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="77de1-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="77de1-140">Какое действие необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="77de1-140">What action to take.</span></span> <span data-ttu-id="77de1-141">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="77de1-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="77de1-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="77de1-142">notificationTemplateId</span></span>|<span data-ttu-id="77de1-143">String</span><span class="sxs-lookup"><span data-stu-id="77de1-143">String</span></span>|<span data-ttu-id="77de1-144">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="77de1-144">What notification Message template to use</span></span>|
|<span data-ttu-id="77de1-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="77de1-145">notificationMessageCCList</span></span>|<span data-ttu-id="77de1-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="77de1-146">String collection</span></span>|<span data-ttu-id="77de1-147">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="77de1-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="77de1-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="77de1-148">Response</span></span>
<span data-ttu-id="77de1-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77de1-149">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77de1-150">Пример</span><span class="sxs-lookup"><span data-stu-id="77de1-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="77de1-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="77de1-151">Request</span></span>
<span data-ttu-id="77de1-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77de1-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="77de1-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="77de1-153">Response</span></span>
<span data-ttu-id="77de1-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="77de1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



