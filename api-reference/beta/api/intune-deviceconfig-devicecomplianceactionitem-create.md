---
title: Создание объекта deviceComplianceActionItem
description: Создание объекта deviceComplianceActionItem.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5e538bd064c2d590eeb743e2c2dea05abc869900
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421582"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="424db-103">Создание объекта deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="424db-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="424db-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="424db-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="424db-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="424db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="424db-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="424db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="424db-107">Создание объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="424db-107">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="424db-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="424db-108">Prerequisites</span></span>
<span data-ttu-id="424db-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="424db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="424db-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="424db-111">Permission type</span></span>|<span data-ttu-id="424db-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="424db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="424db-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="424db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="424db-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="424db-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="424db-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="424db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="424db-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="424db-116">Not supported.</span></span>|
|<span data-ttu-id="424db-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="424db-117">Application</span></span>|<span data-ttu-id="424db-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="424db-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="424db-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="424db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="424db-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="424db-120">Request headers</span></span>
|<span data-ttu-id="424db-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="424db-121">Header</span></span>|<span data-ttu-id="424db-122">Значение</span><span class="sxs-lookup"><span data-stu-id="424db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="424db-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="424db-123">Authorization</span></span>|<span data-ttu-id="424db-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="424db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="424db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="424db-125">Accept</span></span>|<span data-ttu-id="424db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="424db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="424db-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="424db-127">Request body</span></span>
<span data-ttu-id="424db-128">В тексте запроса добавьте представление объекта deviceComplianceActionItem в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="424db-128">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="424db-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="424db-129">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="424db-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="424db-130">Property</span></span>|<span data-ttu-id="424db-131">Тип</span><span class="sxs-lookup"><span data-stu-id="424db-131">Type</span></span>|<span data-ttu-id="424db-132">Описание</span><span class="sxs-lookup"><span data-stu-id="424db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="424db-133">id</span><span class="sxs-lookup"><span data-stu-id="424db-133">id</span></span>|<span data-ttu-id="424db-134">String</span><span class="sxs-lookup"><span data-stu-id="424db-134">String</span></span>|<span data-ttu-id="424db-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="424db-135">Key of the entity.</span></span>|
|<span data-ttu-id="424db-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="424db-136">gracePeriodHours</span></span>|<span data-ttu-id="424db-137">Int32</span><span class="sxs-lookup"><span data-stu-id="424db-137">Int32</span></span>|<span data-ttu-id="424db-138">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="424db-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="424db-139">Допустимые значения: от 0 до 8760.</span><span class="sxs-lookup"><span data-stu-id="424db-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="424db-140">actionType</span><span class="sxs-lookup"><span data-stu-id="424db-140">actionType</span></span>|[<span data-ttu-id="424db-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="424db-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="424db-142">Какое действие необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="424db-142">What action to take.</span></span> <span data-ttu-id="424db-143">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="424db-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="424db-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="424db-144">notificationTemplateId</span></span>|<span data-ttu-id="424db-145">String</span><span class="sxs-lookup"><span data-stu-id="424db-145">String</span></span>|<span data-ttu-id="424db-146">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="424db-146">What notification Message template to use</span></span>|
|<span data-ttu-id="424db-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="424db-147">notificationMessageCCList</span></span>|<span data-ttu-id="424db-148">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="424db-148">String collection</span></span>|<span data-ttu-id="424db-149">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="424db-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="424db-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="424db-150">Response</span></span>
<span data-ttu-id="424db-151">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="424db-151">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="424db-152">Пример</span><span class="sxs-lookup"><span data-stu-id="424db-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="424db-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="424db-153">Request</span></span>
<span data-ttu-id="424db-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="424db-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="424db-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="424db-155">Response</span></span>
<span data-ttu-id="424db-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="424db-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




