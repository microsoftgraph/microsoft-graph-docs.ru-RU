---
title: Создание объекта deviceComplianceActionItem
description: Создание объекта deviceComplianceActionItem.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dca5374dcb75e93667454389f0104861bb9f1d7c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524479"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="14c73-103">Создание объекта deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="14c73-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="14c73-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14c73-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14c73-105">Создание объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="14c73-105">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14c73-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="14c73-106">Prerequisites</span></span>
<span data-ttu-id="14c73-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14c73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14c73-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14c73-109">Permission type</span></span>|<span data-ttu-id="14c73-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="14c73-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14c73-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14c73-111">Delegated (work or school account)</span></span>|<span data-ttu-id="14c73-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14c73-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14c73-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14c73-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14c73-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14c73-114">Not supported.</span></span>|
|<span data-ttu-id="14c73-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14c73-115">Application</span></span>|<span data-ttu-id="14c73-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14c73-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14c73-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14c73-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="14c73-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14c73-118">Request headers</span></span>
|<span data-ttu-id="14c73-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14c73-119">Header</span></span>|<span data-ttu-id="14c73-120">Значение</span><span class="sxs-lookup"><span data-stu-id="14c73-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14c73-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14c73-121">Authorization</span></span>|<span data-ttu-id="14c73-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14c73-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14c73-123">Accept</span><span class="sxs-lookup"><span data-stu-id="14c73-123">Accept</span></span>|<span data-ttu-id="14c73-124">application/json</span><span class="sxs-lookup"><span data-stu-id="14c73-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14c73-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14c73-125">Request body</span></span>
<span data-ttu-id="14c73-126">В тексте запроса добавьте представление объекта deviceComplianceActionItem в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14c73-126">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="14c73-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта deviceComplianceActionItem.</span><span class="sxs-lookup"><span data-stu-id="14c73-127">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="14c73-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="14c73-128">Property</span></span>|<span data-ttu-id="14c73-129">Тип</span><span class="sxs-lookup"><span data-stu-id="14c73-129">Type</span></span>|<span data-ttu-id="14c73-130">Описание</span><span class="sxs-lookup"><span data-stu-id="14c73-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14c73-131">id</span><span class="sxs-lookup"><span data-stu-id="14c73-131">id</span></span>|<span data-ttu-id="14c73-132">String</span><span class="sxs-lookup"><span data-stu-id="14c73-132">String</span></span>|<span data-ttu-id="14c73-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="14c73-133">Key of the entity.</span></span>|
|<span data-ttu-id="14c73-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="14c73-134">gracePeriodHours</span></span>|<span data-ttu-id="14c73-135">Int32</span><span class="sxs-lookup"><span data-stu-id="14c73-135">Int32</span></span>|<span data-ttu-id="14c73-136">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="14c73-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="14c73-137">Допустимые значения: от 0 до 8760</span><span class="sxs-lookup"><span data-stu-id="14c73-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="14c73-138">actionType</span><span class="sxs-lookup"><span data-stu-id="14c73-138">actionType</span></span>|[<span data-ttu-id="14c73-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="14c73-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="14c73-140">Действия, которые необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="14c73-140">What action to take.</span></span> <span data-ttu-id="14c73-141">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span><span class="sxs-lookup"><span data-stu-id="14c73-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="14c73-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="14c73-142">notificationTemplateId</span></span>|<span data-ttu-id="14c73-143">String</span><span class="sxs-lookup"><span data-stu-id="14c73-143">String</span></span>|<span data-ttu-id="14c73-144">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="14c73-144">What notification Message template to use</span></span>|
|<span data-ttu-id="14c73-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="14c73-145">notificationMessageCCList</span></span>|<span data-ttu-id="14c73-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="14c73-146">String collection</span></span>|<span data-ttu-id="14c73-147">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="14c73-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="14c73-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="14c73-148">Response</span></span>
<span data-ttu-id="14c73-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="14c73-149">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14c73-150">Пример</span><span class="sxs-lookup"><span data-stu-id="14c73-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="14c73-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="14c73-151">Request</span></span>
<span data-ttu-id="14c73-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14c73-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="14c73-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="14c73-153">Response</span></span>
<span data-ttu-id="14c73-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14c73-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



