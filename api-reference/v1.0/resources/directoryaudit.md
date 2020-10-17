---
title: Тип ресурса directoryAudit
description: Представляет элементы аудита каталога и его коллекцию.
author: SarahBar
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fe49a8561a4081fc6d573d6ca595ceeca9f8bbd0
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582165"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="f65b0-103">Тип ресурса directoryAudit</span><span class="sxs-lookup"><span data-stu-id="f65b0-103">directoryAudit resource type</span></span>

<span data-ttu-id="f65b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f65b0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f65b0-105">Представляет элементы аудита каталога и его коллекцию.</span><span class="sxs-lookup"><span data-stu-id="f65b0-105">Represents the directory audit items and its collection.</span></span>

## <a name="methods"></a><span data-ttu-id="f65b0-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f65b0-106">Methods</span></span>

| <span data-ttu-id="f65b0-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f65b0-107">Method</span></span>           | <span data-ttu-id="f65b0-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f65b0-108">Return Type</span></span>    |<span data-ttu-id="f65b0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f65b0-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f65b0-110">Перечисление directoryAudits</span><span class="sxs-lookup"><span data-stu-id="f65b0-110">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="f65b0-111">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="f65b0-111">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="f65b0-112">Перечисление элементов аудита каталога в коллекции и их свойства.</span><span class="sxs-lookup"><span data-stu-id="f65b0-112">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="f65b0-113">Получение directoryAudit</span><span class="sxs-lookup"><span data-stu-id="f65b0-113">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="f65b0-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="f65b0-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="f65b0-115">Получение определенного элемента аудита каталога и его свойств.</span><span class="sxs-lookup"><span data-stu-id="f65b0-115">Get a specific directory audit item and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="f65b0-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="f65b0-116">Properties</span></span>

| <span data-ttu-id="f65b0-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="f65b0-117">Property</span></span>            | <span data-ttu-id="f65b0-118">Тип</span><span class="sxs-lookup"><span data-stu-id="f65b0-118">Type</span></span>                                                | <span data-ttu-id="f65b0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f65b0-119">Description</span></span>                                                                                                                                                                                                                                                                        |
|:--------------------|:----------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f65b0-120">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="f65b0-120">activityDateTime</span></span>    | <span data-ttu-id="f65b0-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f65b0-121">DateTimeOffset</span></span>                                      | <span data-ttu-id="f65b0-122">Указывает дату и время выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="f65b0-122">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="f65b0-123">Тип Timestamp всегда представлен в формате времени UTC.</span><span class="sxs-lookup"><span data-stu-id="f65b0-123">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="f65b0-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f65b0-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>                                                                                          |
| <span data-ttu-id="f65b0-125">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="f65b0-125">activityDisplayName</span></span> | <span data-ttu-id="f65b0-126">String</span><span class="sxs-lookup"><span data-stu-id="f65b0-126">String</span></span>                                              | <span data-ttu-id="f65b0-127">Указывает имя действия или имя операции (примеры: "Создание пользователя" и "Добавление члена в группу").</span><span class="sxs-lookup"><span data-stu-id="f65b0-127">Indicates the activity name or the operation name (examples: "Create User" and "Add member to group").</span></span> <span data-ttu-id="f65b0-128">Для получения полного списка щелкните [список действий Azure AD](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span><span class="sxs-lookup"><span data-stu-id="f65b0-128">For full list, see [Azure AD activity list](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span> |
| <span data-ttu-id="f65b0-129">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="f65b0-129">additionalDetails</span></span>   | <span data-ttu-id="f65b0-130">Коллекция [keyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f65b0-130">[keyValue](keyvalue.md) collection</span></span>                  | <span data-ttu-id="f65b0-131">Указывает дополнительные сведения о действии.</span><span class="sxs-lookup"><span data-stu-id="f65b0-131">Indicates additional details on the activity.</span></span>                                                                                                                                                                                                                                      |
| <span data-ttu-id="f65b0-132">category</span><span class="sxs-lookup"><span data-stu-id="f65b0-132">category</span></span>            | <span data-ttu-id="f65b0-133">String</span><span class="sxs-lookup"><span data-stu-id="f65b0-133">String</span></span>                                              | <span data-ttu-id="f65b0-134">Указывает, для какой категории ресурса предназначено действие.</span><span class="sxs-lookup"><span data-stu-id="f65b0-134">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="f65b0-135">(Пример: управление пользователями, управление группами и т. д.)</span><span class="sxs-lookup"><span data-stu-id="f65b0-135">(For example: User Management, Group Management etc..)</span></span>                                                                                                                                                          |
| <span data-ttu-id="f65b0-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="f65b0-136">correlationId</span></span>       | <span data-ttu-id="f65b0-137">GUID</span><span class="sxs-lookup"><span data-stu-id="f65b0-137">GUID</span></span>                                                | <span data-ttu-id="f65b0-138">Указывает уникальный идентификатор, помогающий соотносить действия, происходящие в различных службах.</span><span class="sxs-lookup"><span data-stu-id="f65b0-138">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="f65b0-139">Можно использовать для отслеживания журналов в службах.</span><span class="sxs-lookup"><span data-stu-id="f65b0-139">Can be used to trace logs across services.</span></span>                                                                                                                                                |
| <span data-ttu-id="f65b0-140">id</span><span class="sxs-lookup"><span data-stu-id="f65b0-140">id</span></span>                  | <span data-ttu-id="f65b0-141">String</span><span class="sxs-lookup"><span data-stu-id="f65b0-141">String</span></span>                                              | <span data-ttu-id="f65b0-142">Указывает уникальный идентификатор для действия.</span><span class="sxs-lookup"><span data-stu-id="f65b0-142">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="f65b0-143">Это идентификатор GUID.</span><span class="sxs-lookup"><span data-stu-id="f65b0-143">This is a GUID.</span></span>                                                                                                                                                                                                                          |
| <span data-ttu-id="f65b0-144">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="f65b0-144">initiatedBy</span></span>         | [<span data-ttu-id="f65b0-145">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="f65b0-145">auditActivityInitiator</span></span>](auditactivityinitiator.md) | <span data-ttu-id="f65b0-146">Указывает сведения о пользователе или приложении, запустившем действие.</span><span class="sxs-lookup"><span data-stu-id="f65b0-146">Indicates information about the user or app initiated the activity.</span></span>                                                                                                                                                                                                                |
| <span data-ttu-id="f65b0-147">loggedByService</span><span class="sxs-lookup"><span data-stu-id="f65b0-147">loggedByService</span></span>     | <span data-ttu-id="f65b0-148">String</span><span class="sxs-lookup"><span data-stu-id="f65b0-148">String</span></span>                                              | <span data-ttu-id="f65b0-149">Указывает, в какой службе запущено действие (например: самостоятельное управление паролями, основной каталог, B2C, приглашенные пользователи, Microsoft Identity Manager, Privileged Identity Management).</span><span class="sxs-lookup"><span data-stu-id="f65b0-149">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>                                                                      |
| <span data-ttu-id="f65b0-150">result</span><span class="sxs-lookup"><span data-stu-id="f65b0-150">result</span></span>              | <span data-ttu-id="f65b0-151">string</span><span class="sxs-lookup"><span data-stu-id="f65b0-151">string</span></span>                                              | <span data-ttu-id="f65b0-152">Указывает результат действия. Возможные значения: `success`, `failure`, `timeout`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f65b0-152">Indicates the result of the activity.Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>                                                                                                                                                                   |
| <span data-ttu-id="f65b0-153">resultReason</span><span class="sxs-lookup"><span data-stu-id="f65b0-153">resultReason</span></span>        | <span data-ttu-id="f65b0-154">String</span><span class="sxs-lookup"><span data-stu-id="f65b0-154">String</span></span>                                              | <span data-ttu-id="f65b0-155">Описывает причины появления "сбоя" или "время ожидания".</span><span class="sxs-lookup"><span data-stu-id="f65b0-155">Describes cause of "failure" or "timeout" results.</span></span>                                                                                                                                                                                                                                 |
| <span data-ttu-id="f65b0-156">targetResources</span><span class="sxs-lookup"><span data-stu-id="f65b0-156">targetResources</span></span>     | <span data-ttu-id="f65b0-157">Коллекция [targetResource](targetresource.md)</span><span class="sxs-lookup"><span data-stu-id="f65b0-157">[targetResource](targetresource.md) collection</span></span>      | <span data-ttu-id="f65b0-158">Указывает, какой ресурс был изменен в результате действия.</span><span class="sxs-lookup"><span data-stu-id="f65b0-158">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="f65b0-159">Возможные типы целевых ресурсов: User, Device, Directory, App, Role, Group, Policy или Other.</span><span class="sxs-lookup"><span data-stu-id="f65b0-159">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>                                                                                                                   |

## <a name="relationships"></a><span data-ttu-id="f65b0-160">Связи</span><span class="sxs-lookup"><span data-stu-id="f65b0-160">Relationships</span></span>

<span data-ttu-id="f65b0-161">Нет</span><span class="sxs-lookup"><span data-stu-id="f65b0-161">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f65b0-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f65b0-162">JSON representation</span></span>

<span data-ttu-id="f65b0-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f65b0-163">Here is a JSON representation of the resource.</span></span>

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