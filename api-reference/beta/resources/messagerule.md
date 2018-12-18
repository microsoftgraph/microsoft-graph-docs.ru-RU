---
title: Тип ресурса messageRule
description: Правило, которое применяется к сообщениям в папке "Входящие" пользователя.
author: angelgolfer-ms
ms.openlocfilehash: 1824e9a8d840da824efb79eff4b98bac02a8c187
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307730"
---
# <a name="messagerule-resource-type"></a><span data-ttu-id="089a7-103">Тип ресурса messageRule</span><span class="sxs-lookup"><span data-stu-id="089a7-103">messageRule resource type</span></span>

> <span data-ttu-id="089a7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="089a7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="089a7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="089a7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="089a7-106">Правило, которое применяется к сообщениям в папке "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="089a7-106">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="089a7-107">В Outlook можно настроить правила для сообщений в папке "Входящие", согласно которым при соблюдении определенных условий выполняются нужные действия.</span><span class="sxs-lookup"><span data-stu-id="089a7-107">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="089a7-108">Программным способом можно получить доступ к правилам, используя свойство навигации **messageRules** [папки](mailfolder.md) "Входящие".</span><span class="sxs-lookup"><span data-stu-id="089a7-108">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="089a7-109">Каждое правило определено ресурсом **messageRule**, доступные действия правил определяются сложным типом [messageRuleActions](messageruleactions.md), а доступные условия и исключения для правил — сложным типом [messageRulePredicates](messagerulepredicates.md).</span><span class="sxs-lookup"><span data-stu-id="089a7-109">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="089a7-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="089a7-110">Properties</span></span>
| <span data-ttu-id="089a7-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="089a7-111">Property</span></span>     | <span data-ttu-id="089a7-112">Тип</span><span class="sxs-lookup"><span data-stu-id="089a7-112">Type</span></span>   |<span data-ttu-id="089a7-113">Описание</span><span class="sxs-lookup"><span data-stu-id="089a7-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="089a7-114">actions</span><span class="sxs-lookup"><span data-stu-id="089a7-114">actions</span></span> | [<span data-ttu-id="089a7-115">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="089a7-115">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="089a7-116">Действия, которые нужно применить к сообщению при выполнении определенных условий.</span><span class="sxs-lookup"><span data-stu-id="089a7-116">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="089a7-117">conditions</span><span class="sxs-lookup"><span data-stu-id="089a7-117">conditions</span></span> | [<span data-ttu-id="089a7-118">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="089a7-118">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="089a7-119">Условия, при соблюдении которых с указанным правилом выполняются соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="089a7-119">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="089a7-120">displayName</span><span class="sxs-lookup"><span data-stu-id="089a7-120">displayName</span></span> | <span data-ttu-id="089a7-121">Строка</span><span class="sxs-lookup"><span data-stu-id="089a7-121">String</span></span> | <span data-ttu-id="089a7-122">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="089a7-122">The display name of the rule.</span></span> |
| <span data-ttu-id="089a7-123">exceptions</span><span class="sxs-lookup"><span data-stu-id="089a7-123">exceptions</span></span> | [<span data-ttu-id="089a7-124">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="089a7-124">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="089a7-125">Условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="089a7-125">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="089a7-126">hasError</span><span class="sxs-lookup"><span data-stu-id="089a7-126">hasError</span></span> | <span data-ttu-id="089a7-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="089a7-127">Boolean</span></span> | <span data-ttu-id="089a7-128">Указывает, является ли правило ошибкой.</span><span class="sxs-lookup"><span data-stu-id="089a7-128">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="089a7-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="089a7-129">Read-only.</span></span> |
| <span data-ttu-id="089a7-130">id</span><span class="sxs-lookup"><span data-stu-id="089a7-130">id</span></span> |<span data-ttu-id="089a7-131">String</span><span class="sxs-lookup"><span data-stu-id="089a7-131">String</span></span>|<span data-ttu-id="089a7-132">Уникальный идентификатор правила.</span><span class="sxs-lookup"><span data-stu-id="089a7-132">The unique identifier of the rule.</span></span> <span data-ttu-id="089a7-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="089a7-133">Read-only.</span></span>|
| <span data-ttu-id="089a7-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="089a7-134">isEnabled</span></span> | <span data-ttu-id="089a7-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="089a7-135">Boolean</span></span> | <span data-ttu-id="089a7-136">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="089a7-136">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="089a7-137">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="089a7-137">isReadOnly</span></span> | <span data-ttu-id="089a7-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="089a7-138">Boolean</span></span> | <span data-ttu-id="089a7-139">Указывает, доступно ли правило только для чтения и можно ли изменить или удалить его с помощью REST API для правил.</span><span class="sxs-lookup"><span data-stu-id="089a7-139">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="089a7-140">sequence</span><span class="sxs-lookup"><span data-stu-id="089a7-140">sequence</span></span> | <span data-ttu-id="089a7-141">Int32</span><span class="sxs-lookup"><span data-stu-id="089a7-141">Int32</span></span> | <span data-ttu-id="089a7-142">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="089a7-142">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="089a7-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="089a7-143">JSON representation</span></span>
<span data-ttu-id="089a7-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="089a7-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
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

## <a name="methods"></a><span data-ttu-id="089a7-145">Методы</span><span class="sxs-lookup"><span data-stu-id="089a7-145">Methods</span></span>
| <span data-ttu-id="089a7-146">Метод</span><span class="sxs-lookup"><span data-stu-id="089a7-146">Method</span></span>           | <span data-ttu-id="089a7-147">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="089a7-147">Return Type</span></span>    |<span data-ttu-id="089a7-148">Описание</span><span class="sxs-lookup"><span data-stu-id="089a7-148">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="089a7-149">Список правил</span><span class="sxs-lookup"><span data-stu-id="089a7-149">List rules</span></span>](../api/mailfolder-list-messagerules.md) | <span data-ttu-id="089a7-150">Коллекция [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="089a7-150">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="089a7-151">Получает все объекты **messageRule**, определенные для папки "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="089a7-151">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="089a7-152">Получение правила</span><span class="sxs-lookup"><span data-stu-id="089a7-152">Get rule</span></span>](../api/messagerule-get.md) | [<span data-ttu-id="089a7-153">messageRule</span><span class="sxs-lookup"><span data-stu-id="089a7-153">messageRule</span></span>](messagerule.md) |<span data-ttu-id="089a7-154">Считывает свойства и отношения объекта **messageRule**.</span><span class="sxs-lookup"><span data-stu-id="089a7-154">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="089a7-155">Создание</span><span class="sxs-lookup"><span data-stu-id="089a7-155">Create</span></span>](../api/mailfolder-post-messagerules.md) | [<span data-ttu-id="089a7-156">messageRule</span><span class="sxs-lookup"><span data-stu-id="089a7-156">messageRule</span></span>](messagerule.md) |<span data-ttu-id="089a7-157">Создает объект **messageRule**, определяя набор условий и действий.</span><span class="sxs-lookup"><span data-stu-id="089a7-157">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="089a7-158">Обновление</span><span class="sxs-lookup"><span data-stu-id="089a7-158">Update</span></span>](../api/messagerule-update.md) | [<span data-ttu-id="089a7-159">messageRule</span><span class="sxs-lookup"><span data-stu-id="089a7-159">messageRule</span></span>](messagerule.md) |<span data-ttu-id="089a7-160">Изменяет записываемые свойства объекта **messageRule** и сохраняет изменения.</span><span class="sxs-lookup"><span data-stu-id="089a7-160">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="089a7-161">Удаление</span><span class="sxs-lookup"><span data-stu-id="089a7-161">Delete</span></span>](../api/messagerule-delete.md) | <span data-ttu-id="089a7-162">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="089a7-162">None</span></span> |<span data-ttu-id="089a7-163">Удаляет указанный объект **messageRule**.</span><span class="sxs-lookup"><span data-stu-id="089a7-163">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->