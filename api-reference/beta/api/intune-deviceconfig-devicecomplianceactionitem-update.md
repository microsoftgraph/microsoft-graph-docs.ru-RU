---
title: Update deviceComplianceActionItem
description: Обновление свойств объекта deviceComplianceActionItem.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5f617f6ea5029b7d24e25dcf903db17a177a9a40
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949772"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="8675e-103">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="8675e-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="8675e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8675e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8675e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8675e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8675e-106">Обновление свойств объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="8675e-106">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8675e-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8675e-107">Prerequisites</span></span>
<span data-ttu-id="8675e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8675e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8675e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8675e-110">Permission type</span></span>|<span data-ttu-id="8675e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8675e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8675e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8675e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8675e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8675e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8675e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8675e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8675e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8675e-115">Not supported.</span></span>|
|<span data-ttu-id="8675e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8675e-116">Application</span></span>|<span data-ttu-id="8675e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8675e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8675e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8675e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="8675e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8675e-119">Request headers</span></span>
|<span data-ttu-id="8675e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8675e-120">Header</span></span>|<span data-ttu-id="8675e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8675e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8675e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8675e-122">Authorization</span></span>|<span data-ttu-id="8675e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8675e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8675e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8675e-124">Accept</span></span>|<span data-ttu-id="8675e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8675e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8675e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8675e-126">Request body</span></span>
<span data-ttu-id="8675e-127">В теле запроса добавьте представление объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8675e-127">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="8675e-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span><span class="sxs-lookup"><span data-stu-id="8675e-128">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="8675e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8675e-129">Property</span></span>|<span data-ttu-id="8675e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8675e-130">Type</span></span>|<span data-ttu-id="8675e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8675e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8675e-132">id</span><span class="sxs-lookup"><span data-stu-id="8675e-132">id</span></span>|<span data-ttu-id="8675e-133">Строка</span><span class="sxs-lookup"><span data-stu-id="8675e-133">String</span></span>|<span data-ttu-id="8675e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8675e-134">Key of the entity.</span></span>|
|<span data-ttu-id="8675e-135">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="8675e-135">gracePeriodHours</span></span>|<span data-ttu-id="8675e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="8675e-136">Int32</span></span>|<span data-ttu-id="8675e-137">Время ожидания (в часах) до применения действия.</span><span class="sxs-lookup"><span data-stu-id="8675e-137">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="8675e-138">Допустимые значения: от 0 до 8760</span><span class="sxs-lookup"><span data-stu-id="8675e-138">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="8675e-139">actionType</span><span class="sxs-lookup"><span data-stu-id="8675e-139">actionType</span></span>|[<span data-ttu-id="8675e-140">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="8675e-140">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="8675e-141">Действия, которые необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="8675e-141">What action to take.</span></span> <span data-ttu-id="8675e-142">Возможные значения: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span><span class="sxs-lookup"><span data-stu-id="8675e-142">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="8675e-143">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="8675e-143">notificationTemplateId</span></span>|<span data-ttu-id="8675e-144">String</span><span class="sxs-lookup"><span data-stu-id="8675e-144">String</span></span>|<span data-ttu-id="8675e-145">Используемый шаблон сообщения уведомления</span><span class="sxs-lookup"><span data-stu-id="8675e-145">What notification Message template to use</span></span>|
|<span data-ttu-id="8675e-146">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="8675e-146">notificationMessageCCList</span></span>|<span data-ttu-id="8675e-147">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8675e-147">String collection</span></span>|<span data-ttu-id="8675e-148">Список идентификаторов групп, которым будет отправлена копия этого уведомления.</span><span class="sxs-lookup"><span data-stu-id="8675e-148">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="8675e-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="8675e-149">Response</span></span>
<span data-ttu-id="8675e-150">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8675e-150">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8675e-151">Пример</span><span class="sxs-lookup"><span data-stu-id="8675e-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="8675e-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="8675e-152">Request</span></span>
<span data-ttu-id="8675e-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8675e-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8675e-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="8675e-154">Response</span></span>
<span data-ttu-id="8675e-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8675e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





