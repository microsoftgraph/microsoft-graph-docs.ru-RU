---
title: тип ресурса cloudPcAuditEvent
description: Представляет объект событий аудита.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: a863ea4128b7383c70bd14f025fcc5ce116dda25
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211345"
---
# <a name="cloudpcauditevent-resource-type"></a><span data-ttu-id="7951e-103">тип ресурса cloudPcAuditEvent</span><span class="sxs-lookup"><span data-stu-id="7951e-103">cloudPcAuditEvent resource type</span></span>

<span data-ttu-id="7951e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7951e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7951e-105">Представляет объект событий аудита.</span><span class="sxs-lookup"><span data-stu-id="7951e-105">Represents the audit event entity.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="7951e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="7951e-106">Methods</span></span>

|<span data-ttu-id="7951e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="7951e-107">Method</span></span>|<span data-ttu-id="7951e-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="7951e-108">Return type</span></span>|<span data-ttu-id="7951e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7951e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7951e-110">Список объектов auditEvent</span><span class="sxs-lookup"><span data-stu-id="7951e-110">List auditEvents</span></span>](../api/virtualendpoint-list-auditevents.md)|<span data-ttu-id="7951e-111">[коллекция cloudPcAuditEvent](../resources/cloudpcauditevent.md)</span><span class="sxs-lookup"><span data-stu-id="7951e-111">[cloudPcAuditEvent](../resources/cloudpcauditevent.md) collection</span></span>|<span data-ttu-id="7951e-112">Список всех [объектов cloudPcAuditEvent](../resources/cloudpcauditevent.md) в клиенте.</span><span class="sxs-lookup"><span data-stu-id="7951e-112">List all the [cloudPcAuditEvent](../resources/cloudpcauditevent.md) objects in a tenant.</span></span>|
|[<span data-ttu-id="7951e-113">Get cloudPcAuditEvent</span><span class="sxs-lookup"><span data-stu-id="7951e-113">Get cloudPcAuditEvent</span></span>](../api/cloudpcauditevent-get.md)|[<span data-ttu-id="7951e-114">cloudPcAuditEvent</span><span class="sxs-lookup"><span data-stu-id="7951e-114">cloudPcAuditEvent</span></span>](../resources/cloudpcauditevent.md)|<span data-ttu-id="7951e-115">Ознакомьтесь с свойствами и отношениями объекта [cloudPcAuditEvent.](../resources/cloudpcauditevent.md)</span><span class="sxs-lookup"><span data-stu-id="7951e-115">Read the properties and relationships of a [cloudPcAuditEvent](../resources/cloudpcauditevent.md) object.</span></span>|
|[<span data-ttu-id="7951e-116">Функция getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="7951e-116">getAuditActivityTypes function</span></span>](../api/cloudpcauditevent-getauditactivitytypes.md)|<span data-ttu-id="7951e-117">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7951e-117">String collection</span></span>|<span data-ttu-id="7951e-118">Получите типы действий аудита.</span><span class="sxs-lookup"><span data-stu-id="7951e-118">Get audit activity types.</span></span>|

## <a name="properties"></a><span data-ttu-id="7951e-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="7951e-119">Properties</span></span>

|<span data-ttu-id="7951e-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="7951e-120">Property</span></span>|<span data-ttu-id="7951e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="7951e-121">Type</span></span>|<span data-ttu-id="7951e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7951e-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7951e-123">id</span><span class="sxs-lookup"><span data-stu-id="7951e-123">id</span></span>|<span data-ttu-id="7951e-124">String</span><span class="sxs-lookup"><span data-stu-id="7951e-124">String</span></span>|<span data-ttu-id="7951e-125">Ключ объекта аудита.</span><span class="sxs-lookup"><span data-stu-id="7951e-125">Key of the audit entity.</span></span> <span data-ttu-id="7951e-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7951e-126">Read-only.</span></span>|
|<span data-ttu-id="7951e-127">displayName</span><span class="sxs-lookup"><span data-stu-id="7951e-127">displayName</span></span>|<span data-ttu-id="7951e-128">String</span><span class="sxs-lookup"><span data-stu-id="7951e-128">String</span></span>|<span data-ttu-id="7951e-129">Отображаемое имя события.</span><span class="sxs-lookup"><span data-stu-id="7951e-129">Event display name.</span></span> <span data-ttu-id="7951e-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7951e-130">Read-only.</span></span>|
|<span data-ttu-id="7951e-131">componentName</span><span class="sxs-lookup"><span data-stu-id="7951e-131">componentName</span></span>|<span data-ttu-id="7951e-132">String</span><span class="sxs-lookup"><span data-stu-id="7951e-132">String</span></span>|<span data-ttu-id="7951e-133">Имя компонента.</span><span class="sxs-lookup"><span data-stu-id="7951e-133">Component name.</span></span> <span data-ttu-id="7951e-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7951e-134">Read-only.</span></span>|
|<span data-ttu-id="7951e-135">actor</span><span class="sxs-lookup"><span data-stu-id="7951e-135">actor</span></span>|[<span data-ttu-id="7951e-136">cloudPcAuditActor</span><span class="sxs-lookup"><span data-stu-id="7951e-136">cloudPcAuditActor</span></span>](../resources/cloudpcauditactor.md)|<span data-ttu-id="7951e-137">Пользователь и приложение Azure AD, связанные с событием аудита.</span><span class="sxs-lookup"><span data-stu-id="7951e-137">Azure AD user and application associated with the audit event.</span></span> <span data-ttu-id="7951e-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7951e-138">Read-only.</span></span>|
|<span data-ttu-id="7951e-139">activity</span><span class="sxs-lookup"><span data-stu-id="7951e-139">activity</span></span>|<span data-ttu-id="7951e-140">String</span><span class="sxs-lookup"><span data-stu-id="7951e-140">String</span></span>|<span data-ttu-id="7951e-141">Понятное имя действия.</span><span class="sxs-lookup"><span data-stu-id="7951e-141">Friendly name of the activity.</span></span><span data-ttu-id="7951e-142">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="7951e-142"> Optional.</span></span>|
|<span data-ttu-id="7951e-143">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="7951e-143">activityDateTime</span></span>|<span data-ttu-id="7951e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7951e-144">DateTimeOffset</span></span>|<span data-ttu-id="7951e-145">Дата и время выполнения действия (в формате UTC).</span><span class="sxs-lookup"><span data-stu-id="7951e-145">The date time in UTC when the activity was performed.</span></span><span data-ttu-id="7951e-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7951e-146"> Read-only.</span></span>|
|<span data-ttu-id="7951e-147">activityType</span><span class="sxs-lookup"><span data-stu-id="7951e-147">activityType</span></span>|<span data-ttu-id="7951e-148">String</span><span class="sxs-lookup"><span data-stu-id="7951e-148">String</span></span>|<span data-ttu-id="7951e-149">Тип выполняемой деятельности.</span><span class="sxs-lookup"><span data-stu-id="7951e-149">The type of activity that was performed.</span></span><span data-ttu-id="7951e-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7951e-150"> Read-only.</span></span>|
|<span data-ttu-id="7951e-151">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="7951e-151">activityOperationType</span></span>|[<span data-ttu-id="7951e-152">cloudPcAuditActivityOperationType</span><span class="sxs-lookup"><span data-stu-id="7951e-152">cloudPcAuditActivityOperationType</span></span>](#cloudpcauditactivityoperationtype-values)|<span data-ttu-id="7951e-153">Тип операции HTTP для действия.</span><span class="sxs-lookup"><span data-stu-id="7951e-153">The HTTP operation type of the activity.</span></span> <span data-ttu-id="7951e-154">Возможные значения включают  `create` `delete` , и `patch` `other` .</span><span class="sxs-lookup"><span data-stu-id="7951e-154">Possible values include `create`, `delete`, `patch` and `other`.</span></span> <span data-ttu-id="7951e-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7951e-155">Read-only.</span></span>|
|<span data-ttu-id="7951e-156">activityResult</span><span class="sxs-lookup"><span data-stu-id="7951e-156">activityResult</span></span>|[<span data-ttu-id="7951e-157">cloudPcAuditActivityResult</span><span class="sxs-lookup"><span data-stu-id="7951e-157">cloudPcAuditActivityResult</span></span>](#cloudpcauditactivityresult-values)|<span data-ttu-id="7951e-158">Результат действия.</span><span class="sxs-lookup"><span data-stu-id="7951e-158">The result of the activity.</span></span><span data-ttu-id="7951e-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7951e-159"> Read-only.</span></span>|
|<span data-ttu-id="7951e-160">correlationId</span><span class="sxs-lookup"><span data-stu-id="7951e-160">correlationId</span></span>|<span data-ttu-id="7951e-161">String</span><span class="sxs-lookup"><span data-stu-id="7951e-161">String</span></span>|<span data-ttu-id="7951e-162">Идентификатор клиентского запроса, используемый для сопоставления действий в системе.</span><span class="sxs-lookup"><span data-stu-id="7951e-162">The client request identifier, used to correlate activity within the system.</span></span><span data-ttu-id="7951e-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7951e-163"> Read-only.</span></span>|
|<span data-ttu-id="7951e-164">resources</span><span class="sxs-lookup"><span data-stu-id="7951e-164">resources</span></span>|<span data-ttu-id="7951e-165">[коллекция cloudPcAuditResource](../resources/cloudpcauditresource.md)</span><span class="sxs-lookup"><span data-stu-id="7951e-165">[cloudPcAuditResource](../resources/cloudpcauditresource.md) collection</span></span>|<span data-ttu-id="7951e-166">Список объектов cloudPcAuditResource.</span><span class="sxs-lookup"><span data-stu-id="7951e-166">List of cloudPcAuditResource objects.</span></span><span data-ttu-id="7951e-167">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7951e-167"> Read-only.</span></span>|
|<span data-ttu-id="7951e-168">category</span><span class="sxs-lookup"><span data-stu-id="7951e-168">category</span></span>|[<span data-ttu-id="7951e-169">cloudPcAuditCategory</span><span class="sxs-lookup"><span data-stu-id="7951e-169">cloudPcAuditCategory</span></span>](#cloudpcauditcategory-values)|<span data-ttu-id="7951e-170">Категория аудита.</span><span class="sxs-lookup"><span data-stu-id="7951e-170">Audit category.</span></span> <span data-ttu-id="7951e-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7951e-171">Read-only.</span></span>|

### <a name="cloudpcauditactivityoperationtype-values"></a><span data-ttu-id="7951e-172">значения cloudPcAuditActivityOperationType</span><span class="sxs-lookup"><span data-stu-id="7951e-172">cloudPcAuditActivityOperationType values</span></span>

|<span data-ttu-id="7951e-173">Member</span><span class="sxs-lookup"><span data-stu-id="7951e-173">Member</span></span>|<span data-ttu-id="7951e-174">Описание</span><span class="sxs-lookup"><span data-stu-id="7951e-174">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7951e-175">create</span><span class="sxs-lookup"><span data-stu-id="7951e-175">create</span></span>|<span data-ttu-id="7951e-176">Создание операции.</span><span class="sxs-lookup"><span data-stu-id="7951e-176">Create operation.</span></span>|
|<span data-ttu-id="7951e-177">delete</span><span class="sxs-lookup"><span data-stu-id="7951e-177">delete</span></span>|<span data-ttu-id="7951e-178">Удаление операции.</span><span class="sxs-lookup"><span data-stu-id="7951e-178">Delete operation.</span></span>|
|<span data-ttu-id="7951e-179">исправление</span><span class="sxs-lookup"><span data-stu-id="7951e-179">patch</span></span>|<span data-ttu-id="7951e-180">Операция исправлений.</span><span class="sxs-lookup"><span data-stu-id="7951e-180">Patch operation.</span></span>|
|<span data-ttu-id="7951e-181">другие</span><span class="sxs-lookup"><span data-stu-id="7951e-181">other</span></span>|<span data-ttu-id="7951e-182">Другая операция.</span><span class="sxs-lookup"><span data-stu-id="7951e-182">Other operation.</span></span>|

### <a name="cloudpcauditactivityresult-values"></a><span data-ttu-id="7951e-183">значения cloudPcAuditActivityResult</span><span class="sxs-lookup"><span data-stu-id="7951e-183">cloudPcAuditActivityResult values</span></span>

|<span data-ttu-id="7951e-184">Member</span><span class="sxs-lookup"><span data-stu-id="7951e-184">Member</span></span>|<span data-ttu-id="7951e-185">Описание</span><span class="sxs-lookup"><span data-stu-id="7951e-185">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7951e-186">success</span><span class="sxs-lookup"><span data-stu-id="7951e-186">success</span></span>|<span data-ttu-id="7951e-187">Операция прошла успешно.</span><span class="sxs-lookup"><span data-stu-id="7951e-187">Operation succeeded.</span></span>|
|<span data-ttu-id="7951e-188">clientError</span><span class="sxs-lookup"><span data-stu-id="7951e-188">clientError</span></span>|<span data-ttu-id="7951e-189">Операция не удалась из-за ошибки клиента.</span><span class="sxs-lookup"><span data-stu-id="7951e-189">Operation failed with client error.</span></span>|
|<span data-ttu-id="7951e-190">сбой</span><span class="sxs-lookup"><span data-stu-id="7951e-190">failure</span></span>|<span data-ttu-id="7951e-191">Не удалось выполнить операцию.</span><span class="sxs-lookup"><span data-stu-id="7951e-191">Operation failed.</span></span>|
|<span data-ttu-id="7951e-192">timeExceeded</span><span class="sxs-lookup"><span data-stu-id="7951e-192">timeExceeded</span></span>|<span data-ttu-id="7951e-193">Операция не справилась с периодией времени.</span><span class="sxs-lookup"><span data-stu-id="7951e-193">Operation failed with timeout.</span></span>|
|<span data-ttu-id="7951e-194">другие</span><span class="sxs-lookup"><span data-stu-id="7951e-194">other</span></span>|<span data-ttu-id="7951e-195">Другой результат.</span><span class="sxs-lookup"><span data-stu-id="7951e-195">Other result.</span></span>|

### <a name="cloudpcauditcategory-values"></a><span data-ttu-id="7951e-196">значения cloudPcAuditCategory</span><span class="sxs-lookup"><span data-stu-id="7951e-196">cloudPcAuditCategory values</span></span>

|<span data-ttu-id="7951e-197">Member</span><span class="sxs-lookup"><span data-stu-id="7951e-197">Member</span></span>|<span data-ttu-id="7951e-198">Описание</span><span class="sxs-lookup"><span data-stu-id="7951e-198">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7951e-199">cloudPC</span><span class="sxs-lookup"><span data-stu-id="7951e-199">cloudPC</span></span>|<span data-ttu-id="7951e-200">Категория облачного КОМПЬЮТЕРА.</span><span class="sxs-lookup"><span data-stu-id="7951e-200">Cloud PC category.</span></span>|
|<span data-ttu-id="7951e-201">другие</span><span class="sxs-lookup"><span data-stu-id="7951e-201">other</span></span> |<span data-ttu-id="7951e-202">Другая категория.</span><span class="sxs-lookup"><span data-stu-id="7951e-202">Other category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7951e-203">Связи</span><span class="sxs-lookup"><span data-stu-id="7951e-203">Relationships</span></span>

<span data-ttu-id="7951e-204">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7951e-204">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7951e-205">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7951e-205">JSON representation</span></span>

<span data-ttu-id="7951e-206">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7951e-206">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcAuditEvent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.cloudPcAuditActor",
    "type": "String",
    "userPermissions": [
      "String"
    ],
    "applicationId": "String",
    "applicationDisplayName": "String",
    "userPrincipalName": "String",
    "servicePrincipalName": "String",
    "ipAddress": "String",
    "userId": "String",
    "userRoleScopeTags": [
      {
        "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo",
        "displayName": "String",
        "roleScopeTagId": "String"
      }
    ],
    "remoteTenantId": "String",
    "remoteUserId": "String"
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.cloudPcAuditResource",
      "displayName": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.cloudPcAuditProperty",
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
