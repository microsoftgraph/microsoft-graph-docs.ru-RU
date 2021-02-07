---
title: Тип ресурса directoryAudit
description: Представляет элементы аудита каталога и его коллекцию.
author: SarahBar
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 102399d92b8287c7e82a5ae9323c0e827133a50a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131287"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="9c918-103">Тип ресурса directoryAudit</span><span class="sxs-lookup"><span data-stu-id="9c918-103">directoryAudit resource type</span></span>

<span data-ttu-id="9c918-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c918-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c918-105">Представляет элементы аудита каталога и его коллекцию.</span><span class="sxs-lookup"><span data-stu-id="9c918-105">Represents the directory audit items and its collection.</span></span>

## <a name="methods"></a><span data-ttu-id="9c918-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9c918-106">Methods</span></span>

| <span data-ttu-id="9c918-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9c918-107">Method</span></span>           | <span data-ttu-id="9c918-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9c918-108">Return Type</span></span>    |<span data-ttu-id="9c918-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9c918-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c918-110">Перечисление directoryAudits</span><span class="sxs-lookup"><span data-stu-id="9c918-110">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="9c918-111">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="9c918-111">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="9c918-112">Перечисление элементов аудита каталога в коллекции и их свойства.</span><span class="sxs-lookup"><span data-stu-id="9c918-112">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="9c918-113">Получение directoryAudit</span><span class="sxs-lookup"><span data-stu-id="9c918-113">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="9c918-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="9c918-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="9c918-115">Получение определенного элемента аудита каталога и его свойств.</span><span class="sxs-lookup"><span data-stu-id="9c918-115">Get a specific directory audit item and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="9c918-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c918-116">Properties</span></span>

| <span data-ttu-id="9c918-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c918-117">Property</span></span>            | <span data-ttu-id="9c918-118">Тип</span><span class="sxs-lookup"><span data-stu-id="9c918-118">Type</span></span>                                                | <span data-ttu-id="9c918-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9c918-119">Description</span></span>                                                                                                                                                                                                                                                                        |
|:--------------------|:----------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="9c918-120">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="9c918-120">activityDateTime</span></span>    | <span data-ttu-id="9c918-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c918-121">DateTimeOffset</span></span>                                      | <span data-ttu-id="9c918-122">Указывает дату и время выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="9c918-122">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="9c918-123">Тип Timestamp всегда представлен в формате времени UTC.</span><span class="sxs-lookup"><span data-stu-id="9c918-123">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="9c918-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9c918-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>                                                                                          |
| <span data-ttu-id="9c918-125">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="9c918-125">activityDisplayName</span></span> | <span data-ttu-id="9c918-126">String</span><span class="sxs-lookup"><span data-stu-id="9c918-126">String</span></span>                                              | <span data-ttu-id="9c918-127">Указывает имя действия или имя операции (примеры: "Создать пользователя" и "Добавить участника в группу").</span><span class="sxs-lookup"><span data-stu-id="9c918-127">Indicates the activity name or the operation name (examples: "Create User" and "Add member to group").</span></span> <span data-ttu-id="9c918-128">Полный список см. в [списке действий Azure AD.](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list)</span><span class="sxs-lookup"><span data-stu-id="9c918-128">For full list, see [Azure AD activity list](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span> |
| <span data-ttu-id="9c918-129">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="9c918-129">additionalDetails</span></span>   | <span data-ttu-id="9c918-130">Коллекция [keyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9c918-130">[keyValue](keyvalue.md) collection</span></span>                  | <span data-ttu-id="9c918-131">Указывает дополнительные сведения о действии.</span><span class="sxs-lookup"><span data-stu-id="9c918-131">Indicates additional details on the activity.</span></span>                                                                                                                                                                                                                                      |
| <span data-ttu-id="9c918-132">category</span><span class="sxs-lookup"><span data-stu-id="9c918-132">category</span></span>            | <span data-ttu-id="9c918-133">String</span><span class="sxs-lookup"><span data-stu-id="9c918-133">String</span></span>                                              | <span data-ttu-id="9c918-134">Указывает, для какой категории ресурса предназначено действие.</span><span class="sxs-lookup"><span data-stu-id="9c918-134">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="9c918-135">(Пример: управление пользователями, управление группами и т. д.)</span><span class="sxs-lookup"><span data-stu-id="9c918-135">(For example: User Management, Group Management etc..)</span></span>                                                                                                                                                          |
| <span data-ttu-id="9c918-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="9c918-136">correlationId</span></span>       | <span data-ttu-id="9c918-137">GUID</span><span class="sxs-lookup"><span data-stu-id="9c918-137">GUID</span></span>                                                | <span data-ttu-id="9c918-138">Указывает уникальный идентификатор, помогающий соотносить действия, происходящие в различных службах.</span><span class="sxs-lookup"><span data-stu-id="9c918-138">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="9c918-139">Можно использовать для отслеживания журналов в службах.</span><span class="sxs-lookup"><span data-stu-id="9c918-139">Can be used to trace logs across services.</span></span>                                                                                                                                                |
| <span data-ttu-id="9c918-140">id</span><span class="sxs-lookup"><span data-stu-id="9c918-140">id</span></span>                  | <span data-ttu-id="9c918-141">String</span><span class="sxs-lookup"><span data-stu-id="9c918-141">String</span></span>                                              | <span data-ttu-id="9c918-142">Указывает уникальный идентификатор для действия.</span><span class="sxs-lookup"><span data-stu-id="9c918-142">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="9c918-143">Это идентификатор GUID.</span><span class="sxs-lookup"><span data-stu-id="9c918-143">This is a GUID.</span></span>                                                                                                                                                                                                                          |
| <span data-ttu-id="9c918-144">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="9c918-144">initiatedBy</span></span>         | [<span data-ttu-id="9c918-145">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="9c918-145">auditActivityInitiator</span></span>](auditactivityinitiator.md) | <span data-ttu-id="9c918-146">Указывает сведения о пользователе или приложении, запустившем действие.</span><span class="sxs-lookup"><span data-stu-id="9c918-146">Indicates information about the user or app initiated the activity.</span></span>                                                                                                                                                                                                                |
| <span data-ttu-id="9c918-147">loggedByService</span><span class="sxs-lookup"><span data-stu-id="9c918-147">loggedByService</span></span>     | <span data-ttu-id="9c918-148">String</span><span class="sxs-lookup"><span data-stu-id="9c918-148">String</span></span>                                              | <span data-ttu-id="9c918-149">Указывает, в какой службе запущено действие (например: самостоятельное управление паролями, основной каталог, B2C, приглашенные пользователи, Microsoft Identity Manager, Privileged Identity Management).</span><span class="sxs-lookup"><span data-stu-id="9c918-149">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>                                                                      |
| <span data-ttu-id="9c918-150">result</span><span class="sxs-lookup"><span data-stu-id="9c918-150">result</span></span>              | <span data-ttu-id="9c918-151">string</span><span class="sxs-lookup"><span data-stu-id="9c918-151">string</span></span>                                              | <span data-ttu-id="9c918-152">Указывает результат действия.</span><span class="sxs-lookup"><span data-stu-id="9c918-152">Indicates the result of the activity.</span></span> <span data-ttu-id="9c918-153">Возможные значения: `success`, `failure`, `timeout`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="9c918-153">Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>                                                                                                                                                                   |
| <span data-ttu-id="9c918-154">resultReason</span><span class="sxs-lookup"><span data-stu-id="9c918-154">resultReason</span></span>        | <span data-ttu-id="9c918-155">String</span><span class="sxs-lookup"><span data-stu-id="9c918-155">String</span></span>                                              | <span data-ttu-id="9c918-156">Описывает причину "сбоя" или "времени сбоя".</span><span class="sxs-lookup"><span data-stu-id="9c918-156">Describes cause of "failure" or "timeout" results.</span></span>                                                                                                                                                                                                                                 |
| <span data-ttu-id="9c918-157">targetResources</span><span class="sxs-lookup"><span data-stu-id="9c918-157">targetResources</span></span>     | <span data-ttu-id="9c918-158">Коллекция [targetResource](targetresource.md)</span><span class="sxs-lookup"><span data-stu-id="9c918-158">[targetResource](targetresource.md) collection</span></span>      | <span data-ttu-id="9c918-159">Указывает, какой ресурс был изменен в результате действия.</span><span class="sxs-lookup"><span data-stu-id="9c918-159">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="9c918-160">Возможные типы целевых ресурсов: User, Device, Directory, App, Role, Group, Policy или Other.</span><span class="sxs-lookup"><span data-stu-id="9c918-160">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>                                                                                                                   |

## <a name="relationships"></a><span data-ttu-id="9c918-161">Связи</span><span class="sxs-lookup"><span data-stu-id="9c918-161">Relationships</span></span>

<span data-ttu-id="9c918-162">Нет</span><span class="sxs-lookup"><span data-stu-id="9c918-162">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c918-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9c918-163">JSON representation</span></span>

<span data-ttu-id="9c918-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c918-164">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryAudit"
}-->

```json
{
  "activityDateTime": "String (timestamp)",
  "activityDisplayName": "String",
  "additionalDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
  "category": "String",
  "correlationId": "Guid",
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.auditActivityInitiator"},
  "loggedByService": "String",
  "result": "string",
  "resultReason": "String",
  "targetResources": [{"@odata.type": "microsoft.graph.targetResource"}]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryAudit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
