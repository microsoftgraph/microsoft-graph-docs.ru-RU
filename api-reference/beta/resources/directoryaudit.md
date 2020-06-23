---
title: Тип ресурса directoryAudit
description: Описывает ресурс Директоряудит (Entity) API Microsoft Graph (REST), который помогает выполнять аудит действий с каталогом (клиентом) (бета-версия).
author: SarahBar
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cdaae33fde7c691d83491c6f2f561bd4dabb052e
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845292"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="d3a3b-103">Тип ресурса directoryAudit</span><span class="sxs-lookup"><span data-stu-id="d3a3b-103">directoryAudit resource type</span></span>

<span data-ttu-id="d3a3b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3a3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3a3b-105">Представляет элементы аудита каталога и его коллекцию.</span><span class="sxs-lookup"><span data-stu-id="d3a3b-105">Represents the directory audit items and its collection.</span></span>

## <a name="methods"></a><span data-ttu-id="d3a3b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d3a3b-106">Methods</span></span>

| <span data-ttu-id="d3a3b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d3a3b-107">Method</span></span>           | <span data-ttu-id="d3a3b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d3a3b-108">Return Type</span></span>    |<span data-ttu-id="d3a3b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d3a3b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d3a3b-110">Перечисление directoryAudits</span><span class="sxs-lookup"><span data-stu-id="d3a3b-110">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="d3a3b-111">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="d3a3b-111">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="d3a3b-112">Перечисление элементов аудита каталога в коллекции и их свойства.</span><span class="sxs-lookup"><span data-stu-id="d3a3b-112">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="d3a3b-113">Получение directoryAudit</span><span class="sxs-lookup"><span data-stu-id="d3a3b-113">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="d3a3b-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="d3a3b-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="d3a3b-115">Получение определенного элемента аудита каталога и его свойств.</span><span class="sxs-lookup"><span data-stu-id="d3a3b-115">Get a specific directory audit item and its properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="d3a3b-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3a3b-116">Properties</span></span>
| <span data-ttu-id="d3a3b-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3a3b-117">Property</span></span>            | <span data-ttu-id="d3a3b-118">Тип</span><span class="sxs-lookup"><span data-stu-id="d3a3b-118">Type</span></span>                                                | <span data-ttu-id="d3a3b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d3a3b-119">Description</span></span>                                                                                                                                                                                                                                                            |
|:--------------------|:----------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d3a3b-120">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="d3a3b-120">activityDateTime</span></span>    | <span data-ttu-id="d3a3b-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3a3b-121">DateTimeOffset</span></span>                                      | <span data-ttu-id="d3a3b-122">Указывает дату и время выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="d3a3b-122">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="d3a3b-123">Тип Timestamp всегда представлен в формате времени UTC.</span><span class="sxs-lookup"><span data-stu-id="d3a3b-123">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="d3a3b-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d3a3b-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>                                                                              |
| <span data-ttu-id="d3a3b-125">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="d3a3b-125">activityDisplayName</span></span> | <span data-ttu-id="d3a3b-126">String</span><span class="sxs-lookup"><span data-stu-id="d3a3b-126">String</span></span>                                              | <span data-ttu-id="d3a3b-127">Указывает имя действия или операции (например,</span><span class="sxs-lookup"><span data-stu-id="d3a3b-127">Indicates the activity name or the operation name (E.g.</span></span> <span data-ttu-id="d3a3b-128">"Создание пользователя", "Добавление участника в группу").</span><span class="sxs-lookup"><span data-stu-id="d3a3b-128">"Create User", "Add member to group").</span></span> <span data-ttu-id="d3a3b-129">Список зарегистрированных действий см. в [списке действий Azure AD](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span><span class="sxs-lookup"><span data-stu-id="d3a3b-129">For a list of activities logged,refer to [Azure Ad activity list](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span> |
| <span data-ttu-id="d3a3b-130">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="d3a3b-130">additionalDetails</span></span>   | <span data-ttu-id="d3a3b-131">Коллекция [keyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d3a3b-131">[keyValue](keyvalue.md) collection</span></span>                  | <span data-ttu-id="d3a3b-132">Указывает дополнительные сведения о действии.</span><span class="sxs-lookup"><span data-stu-id="d3a3b-132">Indicates additional details on the activity.</span></span>                                                                                                                                                                                                                          |
| <span data-ttu-id="d3a3b-133">category</span><span class="sxs-lookup"><span data-stu-id="d3a3b-133">category</span></span>            | <span data-ttu-id="d3a3b-134">String</span><span class="sxs-lookup"><span data-stu-id="d3a3b-134">String</span></span>                                              | <span data-ttu-id="d3a3b-135">Указывает, для какой категории ресурса предназначено действие.</span><span class="sxs-lookup"><span data-stu-id="d3a3b-135">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="d3a3b-136">(Пример: управление пользователями, управление группами и т. д.)</span><span class="sxs-lookup"><span data-stu-id="d3a3b-136">(For example: User Management, Group Management etc..)</span></span>                                                                                                                                              |
| <span data-ttu-id="d3a3b-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="d3a3b-137">correlationId</span></span>       | <span data-ttu-id="d3a3b-138">GUID</span><span class="sxs-lookup"><span data-stu-id="d3a3b-138">GUID</span></span>                                                | <span data-ttu-id="d3a3b-139">Указывает уникальный идентификатор, помогающий соотносить действия, происходящие в различных службах.</span><span class="sxs-lookup"><span data-stu-id="d3a3b-139">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="d3a3b-140">Можно использовать для отслеживания журналов в службах.</span><span class="sxs-lookup"><span data-stu-id="d3a3b-140">Can be used to trace logs across services.</span></span>                                                                                                                                    |
| <span data-ttu-id="d3a3b-141">id</span><span class="sxs-lookup"><span data-stu-id="d3a3b-141">id</span></span>                  | <span data-ttu-id="d3a3b-142">Строка</span><span class="sxs-lookup"><span data-stu-id="d3a3b-142">String</span></span>                                              | <span data-ttu-id="d3a3b-143">Указывает уникальный идентификатор для действия.</span><span class="sxs-lookup"><span data-stu-id="d3a3b-143">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="d3a3b-144">Это идентификатор GUID.</span><span class="sxs-lookup"><span data-stu-id="d3a3b-144">This is a GUID.</span></span>                                                                                                                                                                                                              |
| <span data-ttu-id="d3a3b-145">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="d3a3b-145">initiatedBy</span></span>         | [<span data-ttu-id="d3a3b-146">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="d3a3b-146">auditActivityInitiator</span></span>](auditactivityinitiator.md) | <span data-ttu-id="d3a3b-147">Указывает сведения о пользователе или приложении, запустившем действие.</span><span class="sxs-lookup"><span data-stu-id="d3a3b-147">Indicates information about the user or app initiated the activity.</span></span>                                                                                                                                                                                                    |
| <span data-ttu-id="d3a3b-148">loggedByService</span><span class="sxs-lookup"><span data-stu-id="d3a3b-148">loggedByService</span></span>     | <span data-ttu-id="d3a3b-149">String</span><span class="sxs-lookup"><span data-stu-id="d3a3b-149">String</span></span>                                              | <span data-ttu-id="d3a3b-150">Указывает, в какой службе запущено действие (например: самостоятельное управление паролями, основной каталог, B2C, приглашенные пользователи, Microsoft Identity Manager, Privileged Identity Management).</span><span class="sxs-lookup"><span data-stu-id="d3a3b-150">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>                                                          |
| <span data-ttu-id="d3a3b-151">result</span><span class="sxs-lookup"><span data-stu-id="d3a3b-151">result</span></span>              | <span data-ttu-id="d3a3b-152">string</span><span class="sxs-lookup"><span data-stu-id="d3a3b-152">string</span></span>                                              | <span data-ttu-id="d3a3b-153">Указывает результат действия. Возможные значения: `success`, `failure`, `timeout`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d3a3b-153">Indicates the result of the activity.Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>                                                                                                                                                       |
| <span data-ttu-id="d3a3b-154">resultReason</span><span class="sxs-lookup"><span data-stu-id="d3a3b-154">resultReason</span></span>        | <span data-ttu-id="d3a3b-155">String</span><span class="sxs-lookup"><span data-stu-id="d3a3b-155">String</span></span>                                              | <span data-ttu-id="d3a3b-156">Указывает причину сбоя, если результатом является Failure (Сбой) или timeout (время ожидания).</span><span class="sxs-lookup"><span data-stu-id="d3a3b-156">Indicates the reason for failure if the result is "Failure" or "timeout".</span></span>                                                                                                                                                                                              |
| <span data-ttu-id="d3a3b-157">targetResources</span><span class="sxs-lookup"><span data-stu-id="d3a3b-157">targetResources</span></span>     | <span data-ttu-id="d3a3b-158">Коллекция [targetResource](targetresource.md)</span><span class="sxs-lookup"><span data-stu-id="d3a3b-158">[targetResource](targetresource.md) collection</span></span>      | <span data-ttu-id="d3a3b-159">Указывает, какой ресурс был изменен в результате действия.</span><span class="sxs-lookup"><span data-stu-id="d3a3b-159">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="d3a3b-160">Возможные типы целевых ресурсов: User, Device, Directory, App, Role, Group, Policy или Other.</span><span class="sxs-lookup"><span data-stu-id="d3a3b-160">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>                                                                                                       |

## <a name="relationships"></a><span data-ttu-id="d3a3b-161">Связи</span><span class="sxs-lookup"><span data-stu-id="d3a3b-161">Relationships</span></span>
<span data-ttu-id="d3a3b-162">Нет</span><span class="sxs-lookup"><span data-stu-id="d3a3b-162">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d3a3b-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3a3b-163">JSON representation</span></span>

<span data-ttu-id="d3a3b-164">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3a3b-164">Here is a JSON representation of the resource.</span></span>

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
