---
title: Тип ресурса messageRule
description: Правило, которое применяется к сообщениям в папке "Входящие" пользователя.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 87f6413b3b7bb38d45a8ba30dc39c3168a2a0d97
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965402"
---
# <a name="messagerule-resource-type"></a><span data-ttu-id="9b293-103">Тип ресурса messageRule</span><span class="sxs-lookup"><span data-stu-id="9b293-103">messageRule resource type</span></span>

<span data-ttu-id="9b293-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b293-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="9b293-105">Правило, которое применяется к сообщениям в папке "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="9b293-105">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="9b293-106">В Outlook можно настроить правила для сообщений в папке "Входящие", согласно которым при соблюдении определенных условий выполняются нужные действия.</span><span class="sxs-lookup"><span data-stu-id="9b293-106">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="9b293-107">Программным способом можно получить доступ к правилам, используя свойство навигации **messageRules** [папки](mailfolder.md) "Входящие".</span><span class="sxs-lookup"><span data-stu-id="9b293-107">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="9b293-108">Каждое правило определено ресурсом **messageRule**, доступные действия правил определяются сложным типом [messageRuleActions](messageruleactions.md), а доступные условия и исключения для правил — сложным типом [messageRulePredicates](messagerulepredicates.md).</span><span class="sxs-lookup"><span data-stu-id="9b293-108">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="9b293-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b293-109">Properties</span></span>
| <span data-ttu-id="9b293-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b293-110">Property</span></span>     | <span data-ttu-id="9b293-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9b293-111">Type</span></span>   |<span data-ttu-id="9b293-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9b293-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9b293-113">actions</span><span class="sxs-lookup"><span data-stu-id="9b293-113">actions</span></span> | [<span data-ttu-id="9b293-114">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="9b293-114">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="9b293-115">Действия, которые нужно применить к сообщению при выполнении определенных условий.</span><span class="sxs-lookup"><span data-stu-id="9b293-115">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="9b293-116">conditions</span><span class="sxs-lookup"><span data-stu-id="9b293-116">conditions</span></span> | [<span data-ttu-id="9b293-117">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="9b293-117">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="9b293-118">Условия, выполнение которых активирует соответствующие действия для указанного правила.</span><span class="sxs-lookup"><span data-stu-id="9b293-118">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="9b293-119">displayName</span><span class="sxs-lookup"><span data-stu-id="9b293-119">displayName</span></span> | <span data-ttu-id="9b293-120">String</span><span class="sxs-lookup"><span data-stu-id="9b293-120">String</span></span> | <span data-ttu-id="9b293-121">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="9b293-121">The display name of the rule.</span></span> |
| <span data-ttu-id="9b293-122">exceptions</span><span class="sxs-lookup"><span data-stu-id="9b293-122">exceptions</span></span> | [<span data-ttu-id="9b293-123">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="9b293-123">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="9b293-124">Условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="9b293-124">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="9b293-125">hasError</span><span class="sxs-lookup"><span data-stu-id="9b293-125">hasError</span></span> | <span data-ttu-id="9b293-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b293-126">Boolean</span></span> | <span data-ttu-id="9b293-127">Указывает, является ли правило ошибкой.</span><span class="sxs-lookup"><span data-stu-id="9b293-127">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="9b293-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b293-128">Read-only.</span></span> |
| <span data-ttu-id="9b293-129">id</span><span class="sxs-lookup"><span data-stu-id="9b293-129">id</span></span> |<span data-ttu-id="9b293-130">String</span><span class="sxs-lookup"><span data-stu-id="9b293-130">String</span></span>|<span data-ttu-id="9b293-131">Уникальный идентификатор правила.</span><span class="sxs-lookup"><span data-stu-id="9b293-131">The unique identifier of the rule.</span></span> <span data-ttu-id="9b293-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b293-132">Read-only.</span></span>|
| <span data-ttu-id="9b293-133">isEnabled</span><span class="sxs-lookup"><span data-stu-id="9b293-133">isEnabled</span></span> | <span data-ttu-id="9b293-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b293-134">Boolean</span></span> | <span data-ttu-id="9b293-135">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="9b293-135">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="9b293-136">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="9b293-136">isReadOnly</span></span> | <span data-ttu-id="9b293-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b293-137">Boolean</span></span> | <span data-ttu-id="9b293-138">Указывает, доступно ли правило только для чтения и можно ли изменить или удалить его с помощью REST API для правил.</span><span class="sxs-lookup"><span data-stu-id="9b293-138">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="9b293-139">sequence</span><span class="sxs-lookup"><span data-stu-id="9b293-139">sequence</span></span> | <span data-ttu-id="9b293-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9b293-140">Int32</span></span> | <span data-ttu-id="9b293-141">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="9b293-141">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="9b293-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b293-142">JSON representation</span></span>
<span data-ttu-id="9b293-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b293-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
   "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.messageRule"
}-->

```json
{
  "actions": {"@odata.type": "microsoft.graph.messageRuleActions"},
  "conditions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "displayName": "String",
  "exceptions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "hasError": "Boolean",
  "id": "String",
  "isEnabled": "Boolean",
  "isReadOnly": "Boolean",
  "sequence": "Int32"
}

```

## <a name="methods"></a><span data-ttu-id="9b293-144">Методы</span><span class="sxs-lookup"><span data-stu-id="9b293-144">Methods</span></span>
| <span data-ttu-id="9b293-145">Метод</span><span class="sxs-lookup"><span data-stu-id="9b293-145">Method</span></span>           | <span data-ttu-id="9b293-146">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9b293-146">Return Type</span></span>    |<span data-ttu-id="9b293-147">Описание</span><span class="sxs-lookup"><span data-stu-id="9b293-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9b293-148">Список правил</span><span class="sxs-lookup"><span data-stu-id="9b293-148">List rules</span></span>](../api/mailfolder-list-messagerules.md) | <span data-ttu-id="9b293-149">Коллекция [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="9b293-149">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="9b293-150">Получает все объекты **messageRule**, определенные для папки "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="9b293-150">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="9b293-151">Получение правила</span><span class="sxs-lookup"><span data-stu-id="9b293-151">Get rule</span></span>](../api/messagerule-get.md) | [<span data-ttu-id="9b293-152">messageRule</span><span class="sxs-lookup"><span data-stu-id="9b293-152">messageRule</span></span>](messagerule.md) |<span data-ttu-id="9b293-153">Считывает свойства и отношения объекта **messageRule**.</span><span class="sxs-lookup"><span data-stu-id="9b293-153">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="9b293-154">Создание</span><span class="sxs-lookup"><span data-stu-id="9b293-154">Create</span></span>](../api/mailfolder-post-messagerules.md) | [<span data-ttu-id="9b293-155">messageRule</span><span class="sxs-lookup"><span data-stu-id="9b293-155">messageRule</span></span>](messagerule.md) |<span data-ttu-id="9b293-156">Создает объект **messageRule**, определяя набор условий и действий.</span><span class="sxs-lookup"><span data-stu-id="9b293-156">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="9b293-157">Обновление</span><span class="sxs-lookup"><span data-stu-id="9b293-157">Update</span></span>](../api/messagerule-update.md) | [<span data-ttu-id="9b293-158">messageRule</span><span class="sxs-lookup"><span data-stu-id="9b293-158">messageRule</span></span>](messagerule.md) |<span data-ttu-id="9b293-159">Изменяет записываемые свойства объекта **messageRule** и сохраняет изменения.</span><span class="sxs-lookup"><span data-stu-id="9b293-159">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|<span data-ttu-id="9b293-160">[удаление](../api/messagerule-delete.md);</span><span class="sxs-lookup"><span data-stu-id="9b293-160">[Delete](../api/messagerule-delete.md)</span></span> | <span data-ttu-id="9b293-161">Нет</span><span class="sxs-lookup"><span data-stu-id="9b293-161">None</span></span> |<span data-ttu-id="9b293-162">Удаляет указанный объект **messageRule**.</span><span class="sxs-lookup"><span data-stu-id="9b293-162">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

