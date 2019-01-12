---
title: Тип ресурса auditEvent
description: Класс, содержащий свойства события аудита.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 445ed776de946c3b557e387164f81dcf4ee16ab2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940969"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="fc905-103">Тип ресурса auditEvent</span><span class="sxs-lookup"><span data-stu-id="fc905-103">auditEvent resource type</span></span>

> <span data-ttu-id="fc905-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fc905-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc905-105">Класс, содержащий свойства события аудита.</span><span class="sxs-lookup"><span data-stu-id="fc905-105">A class containing the properties for Audit Event.</span></span>
## <a name="methods"></a><span data-ttu-id="fc905-106">Методы</span><span class="sxs-lookup"><span data-stu-id="fc905-106">Methods</span></span>
|<span data-ttu-id="fc905-107">Метод</span><span class="sxs-lookup"><span data-stu-id="fc905-107">Method</span></span>|<span data-ttu-id="fc905-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fc905-108">Return Type</span></span>|<span data-ttu-id="fc905-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fc905-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fc905-110">Список объектов auditEvent</span><span class="sxs-lookup"><span data-stu-id="fc905-110">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="fc905-111">Коллекция [auditEvent](../resources/intune-auditing-auditevent.md)</span><span class="sxs-lookup"><span data-stu-id="fc905-111">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="fc905-112">Список свойств и связей объектов [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="fc905-112">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="fc905-113">Получение объекта auditEvent</span><span class="sxs-lookup"><span data-stu-id="fc905-113">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="fc905-114">auditEvent</span><span class="sxs-lookup"><span data-stu-id="fc905-114">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="fc905-115">Чтение свойств и связей объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="fc905-115">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="fc905-116">Создание объекта auditEvent</span><span class="sxs-lookup"><span data-stu-id="fc905-116">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="fc905-117">auditEvent</span><span class="sxs-lookup"><span data-stu-id="fc905-117">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="fc905-118">Создание объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="fc905-118">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="fc905-119">Удаление объекта auditEvent</span><span class="sxs-lookup"><span data-stu-id="fc905-119">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="fc905-120">Нет</span><span class="sxs-lookup"><span data-stu-id="fc905-120">None</span></span>|<span data-ttu-id="fc905-121">Удаляет объект [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="fc905-121">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="fc905-122">Обновление объекта auditEvent</span><span class="sxs-lookup"><span data-stu-id="fc905-122">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="fc905-123">auditEvent</span><span class="sxs-lookup"><span data-stu-id="fc905-123">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="fc905-124">Обновление свойств объекта [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="fc905-124">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="fc905-125">Функция getAuditCategories</span><span class="sxs-lookup"><span data-stu-id="fc905-125">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="fc905-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fc905-126">String collection</span></span>|<span data-ttu-id="fc905-127">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fc905-127">Not yet documented</span></span>|
|[<span data-ttu-id="fc905-128">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="fc905-128">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="fc905-129">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fc905-129">String collection</span></span>|<span data-ttu-id="fc905-130">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fc905-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="fc905-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc905-131">Properties</span></span>
|<span data-ttu-id="fc905-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc905-132">Property</span></span>|<span data-ttu-id="fc905-133">Тип</span><span class="sxs-lookup"><span data-stu-id="fc905-133">Type</span></span>|<span data-ttu-id="fc905-134">Описание</span><span class="sxs-lookup"><span data-stu-id="fc905-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc905-135">id</span><span class="sxs-lookup"><span data-stu-id="fc905-135">id</span></span>|<span data-ttu-id="fc905-136">String</span><span class="sxs-lookup"><span data-stu-id="fc905-136">String</span></span>|<span data-ttu-id="fc905-137">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fc905-137">Key of the entity.</span></span>|
|<span data-ttu-id="fc905-138">displayName</span><span class="sxs-lookup"><span data-stu-id="fc905-138">displayName</span></span>|<span data-ttu-id="fc905-139">String</span><span class="sxs-lookup"><span data-stu-id="fc905-139">String</span></span>|<span data-ttu-id="fc905-140">Отображаемое имя события.</span><span class="sxs-lookup"><span data-stu-id="fc905-140">Event display name.</span></span>|
|<span data-ttu-id="fc905-141">componentName</span><span class="sxs-lookup"><span data-stu-id="fc905-141">componentName</span></span>|<span data-ttu-id="fc905-142">String</span><span class="sxs-lookup"><span data-stu-id="fc905-142">String</span></span>|<span data-ttu-id="fc905-143">Имя компонента.</span><span class="sxs-lookup"><span data-stu-id="fc905-143">Component name.</span></span>|
|<span data-ttu-id="fc905-144">actor</span><span class="sxs-lookup"><span data-stu-id="fc905-144">actor</span></span>|[<span data-ttu-id="fc905-145">auditActor</span><span class="sxs-lookup"><span data-stu-id="fc905-145">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="fc905-146">Пользователь AAD и приложение, связанные с событием аудита.</span><span class="sxs-lookup"><span data-stu-id="fc905-146">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="fc905-147">activity</span><span class="sxs-lookup"><span data-stu-id="fc905-147">activity</span></span>|<span data-ttu-id="fc905-148">String</span><span class="sxs-lookup"><span data-stu-id="fc905-148">String</span></span>|<span data-ttu-id="fc905-149">Понятное имя действия.</span><span class="sxs-lookup"><span data-stu-id="fc905-149">Friendly name of the activity.</span></span>|
|<span data-ttu-id="fc905-150">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="fc905-150">activityDateTime</span></span>|<span data-ttu-id="fc905-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc905-151">DateTimeOffset</span></span>|<span data-ttu-id="fc905-152">Дата и время выполнения действия (в формате UTC).</span><span class="sxs-lookup"><span data-stu-id="fc905-152">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="fc905-153">activityType</span><span class="sxs-lookup"><span data-stu-id="fc905-153">activityType</span></span>|<span data-ttu-id="fc905-154">String</span><span class="sxs-lookup"><span data-stu-id="fc905-154">String</span></span>|<span data-ttu-id="fc905-155">Тип выполненного действия.</span><span class="sxs-lookup"><span data-stu-id="fc905-155">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="fc905-156">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="fc905-156">activityOperationType</span></span>|<span data-ttu-id="fc905-157">String</span><span class="sxs-lookup"><span data-stu-id="fc905-157">String</span></span>|<span data-ttu-id="fc905-158">Тип операции HTTP для действия.</span><span class="sxs-lookup"><span data-stu-id="fc905-158">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="fc905-159">activityResult</span><span class="sxs-lookup"><span data-stu-id="fc905-159">activityResult</span></span>|<span data-ttu-id="fc905-160">String</span><span class="sxs-lookup"><span data-stu-id="fc905-160">String</span></span>|<span data-ttu-id="fc905-161">Результат действия.</span><span class="sxs-lookup"><span data-stu-id="fc905-161">The result of the activity.</span></span>|
|<span data-ttu-id="fc905-162">correlationId</span><span class="sxs-lookup"><span data-stu-id="fc905-162">correlationId</span></span>|<span data-ttu-id="fc905-163">Guid</span><span class="sxs-lookup"><span data-stu-id="fc905-163">Guid</span></span>|<span data-ttu-id="fc905-164">Идентификатор клиентского запроса, используемый для согласования действий в системе.</span><span class="sxs-lookup"><span data-stu-id="fc905-164">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="fc905-165">resources</span><span class="sxs-lookup"><span data-stu-id="fc905-165">resources</span></span>|<span data-ttu-id="fc905-166">Коллекция [auditResource](../resources/intune-auditing-auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="fc905-166">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="fc905-167">Изменяемые ресурсы.</span><span class="sxs-lookup"><span data-stu-id="fc905-167">Resources being modified.</span></span>|
|<span data-ttu-id="fc905-168">category</span><span class="sxs-lookup"><span data-stu-id="fc905-168">category</span></span>|<span data-ttu-id="fc905-169">String</span><span class="sxs-lookup"><span data-stu-id="fc905-169">String</span></span>|<span data-ttu-id="fc905-170">Категория аудита.</span><span class="sxs-lookup"><span data-stu-id="fc905-170">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc905-171">Связи</span><span class="sxs-lookup"><span data-stu-id="fc905-171">Relationships</span></span>
<span data-ttu-id="fc905-172">Нет</span><span class="sxs-lookup"><span data-stu-id="fc905-172">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fc905-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc905-173">JSON Representation</span></span>
<span data-ttu-id="fc905-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc905-174">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "String",
    "userPermissions": [
      "String"
    ],
    "applicationId": "String",
    "applicationDisplayName": "String",
    "userPrincipalName": "String",
    "servicePrincipalName": "String",
    "ipAddress": "String",
    "userId": "String"
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "Guid",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "String",
          "oldValue": "String",
          "newValue": "String"
        }
      ],
      "type": "String",
      "resourceId": "String"
    }
  ],
  "category": "String"
}
```



