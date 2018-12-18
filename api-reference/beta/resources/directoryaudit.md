---
title: Тип ресурса directoryAudit
description: Этот ресурс представляет элементы аудита каталогов и ее коллекцию
author: lleonard-msft
ms.openlocfilehash: 5cbfc1320f721afd71ed3f196bb94a5c716d2c5c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312791"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="6995a-103">Тип ресурса directoryAudit</span><span class="sxs-lookup"><span data-stu-id="6995a-103">directoryAudit resource type</span></span>
<span data-ttu-id="6995a-104">Этот ресурс представляет элементы аудита каталогов и ее коллекцию</span><span class="sxs-lookup"><span data-stu-id="6995a-104">This resource represents the directory Audit items and its collection</span></span>


## <a name="methods"></a><span data-ttu-id="6995a-105">Методы</span><span class="sxs-lookup"><span data-stu-id="6995a-105">Methods</span></span>

| <span data-ttu-id="6995a-106">Метод</span><span class="sxs-lookup"><span data-stu-id="6995a-106">Method</span></span>           | <span data-ttu-id="6995a-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6995a-107">Return Type</span></span>    |<span data-ttu-id="6995a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6995a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6995a-109">Список directoryAudits</span><span class="sxs-lookup"><span data-stu-id="6995a-109">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="6995a-110">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="6995a-110">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="6995a-111">Список элементов аудита каталога в коллекции и их свойства.</span><span class="sxs-lookup"><span data-stu-id="6995a-111">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="6995a-112">Получение directoryAudit</span><span class="sxs-lookup"><span data-stu-id="6995a-112">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="6995a-113">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="6995a-113">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="6995a-114">Получение элемента аудита конкретного каталога и его свойства.</span><span class="sxs-lookup"><span data-stu-id="6995a-114">Get a specific directory audit item and its properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="6995a-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="6995a-115">Properties</span></span>
| <span data-ttu-id="6995a-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="6995a-116">Property</span></span>     | <span data-ttu-id="6995a-117">Тип</span><span class="sxs-lookup"><span data-stu-id="6995a-117">Type</span></span>   |<span data-ttu-id="6995a-118">Описание</span><span class="sxs-lookup"><span data-stu-id="6995a-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6995a-119">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="6995a-119">activityDateTime</span></span>|<span data-ttu-id="6995a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6995a-120">DateTimeOffset</span></span>|<span data-ttu-id="6995a-121">Указывает дату и время выполнения операции.</span><span class="sxs-lookup"><span data-stu-id="6995a-121">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="6995a-122">Тип метки времени — всегда в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6995a-122">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="6995a-123">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6995a-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6995a-124">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="6995a-124">activityDisplayName</span></span>|<span data-ttu-id="6995a-125">String.</span><span class="sxs-lookup"><span data-stu-id="6995a-125">String</span></span>|<span data-ttu-id="6995a-126">Указывает имя действия или имя операции (например:</span><span class="sxs-lookup"><span data-stu-id="6995a-126">Indicates the activity name or the operation name (E.g.</span></span> <span data-ttu-id="6995a-127">«Создание пользователя», «Добавить члена в группу»).</span><span class="sxs-lookup"><span data-stu-id="6995a-127">"Create User", "Add member to group").</span></span> <span data-ttu-id="6995a-128">Список действий вход можно получить [список активности Azure Ad](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span><span class="sxs-lookup"><span data-stu-id="6995a-128">For a list of activities logged,refer to [Azure Ad activity list](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span>|
|<span data-ttu-id="6995a-129">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="6995a-129">additionalDetails</span></span>|<span data-ttu-id="6995a-130">Коллекция [keyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6995a-130">[keyValue](keyvalue.md) collection</span></span>|<span data-ttu-id="6995a-131">Указывает Дополнительные сведения для действия.</span><span class="sxs-lookup"><span data-stu-id="6995a-131">Indicates additional details on the activity.</span></span>|
|<span data-ttu-id="6995a-132">category</span><span class="sxs-lookup"><span data-stu-id="6995a-132">category</span></span>|<span data-ttu-id="6995a-133">String</span><span class="sxs-lookup"><span data-stu-id="6995a-133">String</span></span>|<span data-ttu-id="6995a-134">Показывает, какая категория ресурсов, целевым с помощью этого действия.</span><span class="sxs-lookup"><span data-stu-id="6995a-134">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="6995a-135">(Например: управление пользователей, группы управления и т.д..)</span><span class="sxs-lookup"><span data-stu-id="6995a-135">(For example: User Management, Group Management etc..)</span></span>|
|<span data-ttu-id="6995a-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="6995a-136">correlationId</span></span>|<span data-ttu-id="6995a-137">GUID</span><span class="sxs-lookup"><span data-stu-id="6995a-137">GUID</span></span>|<span data-ttu-id="6995a-138">Указывает уникальный идентификатор, и приводятся рекомендации по их действия, охватывающих различных служб.</span><span class="sxs-lookup"><span data-stu-id="6995a-138">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="6995a-139">Можно использовать для журналов трассировки в службах.</span><span class="sxs-lookup"><span data-stu-id="6995a-139">Can be used to trace logs across services.</span></span>|
|<span data-ttu-id="6995a-140">id</span><span class="sxs-lookup"><span data-stu-id="6995a-140">id</span></span>|<span data-ttu-id="6995a-141">Строка</span><span class="sxs-lookup"><span data-stu-id="6995a-141">String</span></span>| <span data-ttu-id="6995a-142">Указывает уникальный идентификатор для действия.</span><span class="sxs-lookup"><span data-stu-id="6995a-142">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="6995a-143">Это идентификатор GUID.</span><span class="sxs-lookup"><span data-stu-id="6995a-143">This is a GUID.</span></span>|
|<span data-ttu-id="6995a-144">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="6995a-144">initiatedBy</span></span>|[<span data-ttu-id="6995a-145">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="6995a-145">auditActivityInitiator</span></span>](auditactivityinitiator.md)|<span data-ttu-id="6995a-146">Указывает, что сведения о пользователе или приложение инициировал действие.</span><span class="sxs-lookup"><span data-stu-id="6995a-146">Indicates information about the user or app initiated the activity.</span></span>|
|<span data-ttu-id="6995a-147">loggedByService</span><span class="sxs-lookup"><span data-stu-id="6995a-147">loggedByService</span></span>|<span data-ttu-id="6995a-148">String.</span><span class="sxs-lookup"><span data-stu-id="6995a-148">String</span></span>|<span data-ttu-id="6995a-149">Указывает сведения, на котором служба инициировал действие (например: управление средствами самостоятельного создания пароля, основная служба каталогов, B2C, приглашение пользователей, Microsoft Identity Manager, привилегированной управления удостоверениями.</span><span class="sxs-lookup"><span data-stu-id="6995a-149">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>|
|<span data-ttu-id="6995a-150">result</span><span class="sxs-lookup"><span data-stu-id="6995a-150">result</span></span>|<span data-ttu-id="6995a-151">string</span><span class="sxs-lookup"><span data-stu-id="6995a-151">string</span></span>| <span data-ttu-id="6995a-152">Указывает результат операции. Возможные значения: `success`, `failure`, `timeout`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6995a-152">Indicates the result of the activity.Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>||
|<span data-ttu-id="6995a-153">resultReason</span><span class="sxs-lookup"><span data-stu-id="6995a-153">resultReason</span></span>|<span data-ttu-id="6995a-154">String.</span><span class="sxs-lookup"><span data-stu-id="6995a-154">String</span></span>|<span data-ttu-id="6995a-155">Указывает причину сбоя, если результат является «Ошибка» или «время ожидания».</span><span class="sxs-lookup"><span data-stu-id="6995a-155">Indicates the reason for failure if the result is "Failure" or "timeout".</span></span>|
|<span data-ttu-id="6995a-156">targetResources</span><span class="sxs-lookup"><span data-stu-id="6995a-156">targetResources</span></span>|<span data-ttu-id="6995a-157">[targetResource](targetresource.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="6995a-157">[targetResource](targetresource.md) collection</span></span>|<span data-ttu-id="6995a-158">Указывает на данные, на котором был изменен ресурсов из-за загрузки.</span><span class="sxs-lookup"><span data-stu-id="6995a-158">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="6995a-159">Тип ресурса конечного может быть пользователя, устройства, каталог, приложение, роли, группы, политики или другое.</span><span class="sxs-lookup"><span data-stu-id="6995a-159">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>

## <a name="relationships"></a><span data-ttu-id="6995a-160">Связи</span><span class="sxs-lookup"><span data-stu-id="6995a-160">Relationships</span></span>
<span data-ttu-id="6995a-161">Нет</span><span class="sxs-lookup"><span data-stu-id="6995a-161">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6995a-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6995a-162">JSON representation</span></span>

<span data-ttu-id="6995a-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6995a-163">Here is a JSON representation of the resource.</span></span>

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