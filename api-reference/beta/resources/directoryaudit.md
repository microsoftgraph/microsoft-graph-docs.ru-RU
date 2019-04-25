---
title: Тип ресурса directoryAudit
description: Этот ресурс представляет элементы аудита каталога и их коллекцию
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1f980208788731206dc58870635644a1f3edc4c7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543228"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="c6b9c-103">Тип ресурса directoryAudit</span><span class="sxs-lookup"><span data-stu-id="c6b9c-103">directoryAudit resource type</span></span>
<span data-ttu-id="c6b9c-104">Этот ресурс представляет элементы аудита каталога и их коллекцию</span><span class="sxs-lookup"><span data-stu-id="c6b9c-104">This resource represents the directory Audit items and its collection</span></span>


## <a name="methods"></a><span data-ttu-id="c6b9c-105">Методы</span><span class="sxs-lookup"><span data-stu-id="c6b9c-105">Methods</span></span>

| <span data-ttu-id="c6b9c-106">Метод</span><span class="sxs-lookup"><span data-stu-id="c6b9c-106">Method</span></span>           | <span data-ttu-id="c6b9c-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c6b9c-107">Return Type</span></span>    |<span data-ttu-id="c6b9c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c6b9c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c6b9c-109">Перечисление directoryAudits</span><span class="sxs-lookup"><span data-stu-id="c6b9c-109">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="c6b9c-110">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="c6b9c-110">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="c6b9c-111">Перечисление элементов аудита каталога в коллекции и их свойства.</span><span class="sxs-lookup"><span data-stu-id="c6b9c-111">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="c6b9c-112">Получение directoryAudit</span><span class="sxs-lookup"><span data-stu-id="c6b9c-112">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="c6b9c-113">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="c6b9c-113">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="c6b9c-114">Получение определенного элемента аудита каталога и его свойств.</span><span class="sxs-lookup"><span data-stu-id="c6b9c-114">Get a specific directory audit item and its properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="c6b9c-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6b9c-115">Properties</span></span>
| <span data-ttu-id="c6b9c-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6b9c-116">Property</span></span>     | <span data-ttu-id="c6b9c-117">Тип</span><span class="sxs-lookup"><span data-stu-id="c6b9c-117">Type</span></span>   |<span data-ttu-id="c6b9c-118">Описание</span><span class="sxs-lookup"><span data-stu-id="c6b9c-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6b9c-119">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="c6b9c-119">activityDateTime</span></span>|<span data-ttu-id="c6b9c-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6b9c-120">DateTimeOffset</span></span>|<span data-ttu-id="c6b9c-121">Указывает дату и время выполнения действия.</span><span class="sxs-lookup"><span data-stu-id="c6b9c-121">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="c6b9c-122">Тип Timestamp всегда представлен в формате времени UTC.</span><span class="sxs-lookup"><span data-stu-id="c6b9c-122">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="c6b9c-123">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c6b9c-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c6b9c-124">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="c6b9c-124">activityDisplayName</span></span>|<span data-ttu-id="c6b9c-125">String</span><span class="sxs-lookup"><span data-stu-id="c6b9c-125">String</span></span>|<span data-ttu-id="c6b9c-126">Указывает имя действия или операции (например,</span><span class="sxs-lookup"><span data-stu-id="c6b9c-126">Indicates the activity name or the operation name (E.g.</span></span> <span data-ttu-id="c6b9c-127">"Создание пользователя", "Добавление участника в группу").</span><span class="sxs-lookup"><span data-stu-id="c6b9c-127">"Create User", "Add member to group").</span></span> <span data-ttu-id="c6b9c-128">Список зарегистрированных действий см. в [списке действий Azure AD](https://docs.microsoft.com/ru-RU/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span><span class="sxs-lookup"><span data-stu-id="c6b9c-128">For a list of activities logged,refer to [Azure Ad activity list](https://docs.microsoft.com/ru-RU/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span>|
|<span data-ttu-id="c6b9c-129">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="c6b9c-129">additionalDetails</span></span>|<span data-ttu-id="c6b9c-130">Коллекция [keyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="c6b9c-130">[keyValue](keyvalue.md) collection</span></span>|<span data-ttu-id="c6b9c-131">Указывает дополнительные сведения о действии.</span><span class="sxs-lookup"><span data-stu-id="c6b9c-131">Indicates additional details on the activity.</span></span>|
|<span data-ttu-id="c6b9c-132">category</span><span class="sxs-lookup"><span data-stu-id="c6b9c-132">category</span></span>|<span data-ttu-id="c6b9c-133">String</span><span class="sxs-lookup"><span data-stu-id="c6b9c-133">String</span></span>|<span data-ttu-id="c6b9c-134">Указывает, для какой категории ресурса предназначено действие.</span><span class="sxs-lookup"><span data-stu-id="c6b9c-134">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="c6b9c-135">(Пример: управление пользователями, управление группами и т. д.)</span><span class="sxs-lookup"><span data-stu-id="c6b9c-135">(For example: User Management, Group Management etc..)</span></span>|
|<span data-ttu-id="c6b9c-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="c6b9c-136">correlationId</span></span>|<span data-ttu-id="c6b9c-137">GUID</span><span class="sxs-lookup"><span data-stu-id="c6b9c-137">GUID</span></span>|<span data-ttu-id="c6b9c-138">Указывает уникальный идентификатор, помогающий соотносить действия, происходящие в различных службах.</span><span class="sxs-lookup"><span data-stu-id="c6b9c-138">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="c6b9c-139">Можно использовать для отслеживания журналов в службах.</span><span class="sxs-lookup"><span data-stu-id="c6b9c-139">Can be used to trace logs across services.</span></span>|
|<span data-ttu-id="c6b9c-140">id</span><span class="sxs-lookup"><span data-stu-id="c6b9c-140">id</span></span>|<span data-ttu-id="c6b9c-141">String</span><span class="sxs-lookup"><span data-stu-id="c6b9c-141">String</span></span>| <span data-ttu-id="c6b9c-142">Указывает уникальный идентификатор для действия.</span><span class="sxs-lookup"><span data-stu-id="c6b9c-142">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="c6b9c-143">Это идентификатор GUID.</span><span class="sxs-lookup"><span data-stu-id="c6b9c-143">This is a GUID.</span></span>|
|<span data-ttu-id="c6b9c-144">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="c6b9c-144">initiatedBy</span></span>|[<span data-ttu-id="c6b9c-145">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="c6b9c-145">auditActivityInitiator</span></span>](auditactivityinitiator.md)|<span data-ttu-id="c6b9c-146">Указывает сведения о пользователе или приложении, запустившем действие.</span><span class="sxs-lookup"><span data-stu-id="c6b9c-146">Indicates information about the user or app initiated the activity.</span></span>|
|<span data-ttu-id="c6b9c-147">loggedByService</span><span class="sxs-lookup"><span data-stu-id="c6b9c-147">loggedByService</span></span>|<span data-ttu-id="c6b9c-148">String</span><span class="sxs-lookup"><span data-stu-id="c6b9c-148">String</span></span>|<span data-ttu-id="c6b9c-149">Указывает, в какой службе запущено действие (например: самостоятельное управление паролями, основной каталог, B2C, приглашенные пользователи, Microsoft Identity Manager, Privileged Identity Management).</span><span class="sxs-lookup"><span data-stu-id="c6b9c-149">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>|
|<span data-ttu-id="c6b9c-150">result</span><span class="sxs-lookup"><span data-stu-id="c6b9c-150">result</span></span>|<span data-ttu-id="c6b9c-151">string</span><span class="sxs-lookup"><span data-stu-id="c6b9c-151">string</span></span>| <span data-ttu-id="c6b9c-152">Указывает результат действия. Возможные значения: `success`, `failure`, `timeout`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c6b9c-152">Indicates the result of the activity.Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>||
|<span data-ttu-id="c6b9c-153">resultReason</span><span class="sxs-lookup"><span data-stu-id="c6b9c-153">resultReason</span></span>|<span data-ttu-id="c6b9c-154">String</span><span class="sxs-lookup"><span data-stu-id="c6b9c-154">String</span></span>|<span data-ttu-id="c6b9c-155">Указывает причину сбоя, если результатом является Failure (Сбой) или timeout (время ожидания).</span><span class="sxs-lookup"><span data-stu-id="c6b9c-155">Indicates the reason for failure if the result is "Failure" or "timeout".</span></span>|
|<span data-ttu-id="c6b9c-156">targetResources</span><span class="sxs-lookup"><span data-stu-id="c6b9c-156">targetResources</span></span>|<span data-ttu-id="c6b9c-157">Коллекция [targetResource](targetresource.md)</span><span class="sxs-lookup"><span data-stu-id="c6b9c-157">[targetResource](targetresource.md) collection</span></span>|<span data-ttu-id="c6b9c-158">Указывает, какой ресурс был изменен в результате действия.</span><span class="sxs-lookup"><span data-stu-id="c6b9c-158">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="c6b9c-159">Возможные типы целевых ресурсов: User, Device, Directory, App, Role, Group, Policy или Other.</span><span class="sxs-lookup"><span data-stu-id="c6b9c-159">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>

## <a name="relationships"></a><span data-ttu-id="c6b9c-160">Связи</span><span class="sxs-lookup"><span data-stu-id="c6b9c-160">Relationships</span></span>
<span data-ttu-id="c6b9c-161">Нет</span><span class="sxs-lookup"><span data-stu-id="c6b9c-161">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c6b9c-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c6b9c-162">JSON representation</span></span>

<span data-ttu-id="c6b9c-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6b9c-163">Here is a JSON representation of the resource.</span></span>

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
