---
title: Тип ресурса messageRule
description: Правило, которое применяется к сообщениям в папке "Входящие" пользователя.
ms.openlocfilehash: beada909a5b4abc1d91a40cf1674916f3d3c04ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027684"
---
# <a name="messagerule-resource-type"></a><span data-ttu-id="4ef84-103">Тип ресурса messageRule</span><span class="sxs-lookup"><span data-stu-id="4ef84-103">messageRule resource type</span></span>


<span data-ttu-id="4ef84-104">Правило, которое применяется к сообщениям в папке "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ef84-104">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="4ef84-105">В Outlook можно настроить правила для сообщений в папке "Входящие", согласно которым при соблюдении определенных условий выполняются нужные действия.</span><span class="sxs-lookup"><span data-stu-id="4ef84-105">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="4ef84-106">Программным способом можно получить доступ к правилам, используя свойство навигации **messageRules** [папки](mailfolder.md) "Входящие".</span><span class="sxs-lookup"><span data-stu-id="4ef84-106">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="4ef84-107">Каждое правило определено ресурсом **messageRule**, доступные действия правил определяются сложным типом [messageRuleActions](messageruleactions.md), а доступные условия и исключения для правил — сложным типом [messageRulePredicates](messagerulepredicates.md).</span><span class="sxs-lookup"><span data-stu-id="4ef84-107">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="4ef84-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ef84-108">Properties</span></span>
| <span data-ttu-id="4ef84-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ef84-109">Property</span></span>     | <span data-ttu-id="4ef84-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4ef84-110">Type</span></span>   |<span data-ttu-id="4ef84-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4ef84-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4ef84-112">actions</span><span class="sxs-lookup"><span data-stu-id="4ef84-112">actions</span></span> | [<span data-ttu-id="4ef84-113">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="4ef84-113">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="4ef84-114">Действия, которые нужно применить к сообщению при выполнении определенных условий.</span><span class="sxs-lookup"><span data-stu-id="4ef84-114">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="4ef84-115">conditions</span><span class="sxs-lookup"><span data-stu-id="4ef84-115">conditions</span></span> | [<span data-ttu-id="4ef84-116">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="4ef84-116">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="4ef84-117">Условия, при соблюдении которых с указанным правилом выполняются соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="4ef84-117">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="4ef84-118">displayName</span><span class="sxs-lookup"><span data-stu-id="4ef84-118">displayName</span></span> | <span data-ttu-id="4ef84-119">String</span><span class="sxs-lookup"><span data-stu-id="4ef84-119">String</span></span> | <span data-ttu-id="4ef84-120">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="4ef84-120">The display name of the rule.</span></span> |
| <span data-ttu-id="4ef84-121">exceptions</span><span class="sxs-lookup"><span data-stu-id="4ef84-121">exceptions</span></span> | [<span data-ttu-id="4ef84-122">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="4ef84-122">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="4ef84-123">Условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="4ef84-123">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="4ef84-124">hasError</span><span class="sxs-lookup"><span data-stu-id="4ef84-124">hasError</span></span> | <span data-ttu-id="4ef84-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ef84-125">Boolean</span></span> | <span data-ttu-id="4ef84-126">Указывает, является ли правило ошибкой.</span><span class="sxs-lookup"><span data-stu-id="4ef84-126">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="4ef84-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ef84-127">Read-only.</span></span> |
| <span data-ttu-id="4ef84-128">id</span><span class="sxs-lookup"><span data-stu-id="4ef84-128">id</span></span> |<span data-ttu-id="4ef84-129">String</span><span class="sxs-lookup"><span data-stu-id="4ef84-129">String</span></span>|<span data-ttu-id="4ef84-130">Уникальный идентификатор правила.</span><span class="sxs-lookup"><span data-stu-id="4ef84-130">The unique identifier of the rule.</span></span> <span data-ttu-id="4ef84-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ef84-131">Read-only.</span></span>|
| <span data-ttu-id="4ef84-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="4ef84-132">isEnabled</span></span> | <span data-ttu-id="4ef84-133">Логический</span><span class="sxs-lookup"><span data-stu-id="4ef84-133">Boolean</span></span> | <span data-ttu-id="4ef84-134">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="4ef84-134">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="4ef84-135">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="4ef84-135">isReadOnly</span></span> | <span data-ttu-id="4ef84-136">Логический</span><span class="sxs-lookup"><span data-stu-id="4ef84-136">Boolean</span></span> | <span data-ttu-id="4ef84-137">Указывает, доступно ли правило только для чтения и можно ли изменить или удалить его с помощью REST API для правил.</span><span class="sxs-lookup"><span data-stu-id="4ef84-137">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="4ef84-138">sequence</span><span class="sxs-lookup"><span data-stu-id="4ef84-138">sequence</span></span> | <span data-ttu-id="4ef84-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4ef84-139">Int32</span></span> | <span data-ttu-id="4ef84-140">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="4ef84-140">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="4ef84-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ef84-141">JSON representation</span></span>
<span data-ttu-id="4ef84-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ef84-142">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="4ef84-143">Методы</span><span class="sxs-lookup"><span data-stu-id="4ef84-143">Methods</span></span>
| <span data-ttu-id="4ef84-144">Метод</span><span class="sxs-lookup"><span data-stu-id="4ef84-144">Method</span></span>           | <span data-ttu-id="4ef84-145">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4ef84-145">Return Type</span></span>    |<span data-ttu-id="4ef84-146">Описание</span><span class="sxs-lookup"><span data-stu-id="4ef84-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4ef84-147">Список правил</span><span class="sxs-lookup"><span data-stu-id="4ef84-147">List rules</span></span>](../api/mailfolder-list-messagerules.md) | <span data-ttu-id="4ef84-148">Коллекция [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="4ef84-148">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="4ef84-149">Получает все объекты **messageRule**, определенные для папки "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="4ef84-149">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="4ef84-150">Получение правила</span><span class="sxs-lookup"><span data-stu-id="4ef84-150">Get rule</span></span>](../api/messagerule-get.md) | [<span data-ttu-id="4ef84-151">messageRule</span><span class="sxs-lookup"><span data-stu-id="4ef84-151">messageRule</span></span>](messagerule.md) |<span data-ttu-id="4ef84-152">Считывает свойства и отношения объекта **messageRule**.</span><span class="sxs-lookup"><span data-stu-id="4ef84-152">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="4ef84-153">Создание</span><span class="sxs-lookup"><span data-stu-id="4ef84-153">Create</span></span>](../api/mailfolder-post-messagerules.md) | [<span data-ttu-id="4ef84-154">messageRule</span><span class="sxs-lookup"><span data-stu-id="4ef84-154">messageRule</span></span>](messagerule.md) |<span data-ttu-id="4ef84-155">Создает объект **messageRule**, определяя набор условий и действий.</span><span class="sxs-lookup"><span data-stu-id="4ef84-155">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="4ef84-156">Обновление</span><span class="sxs-lookup"><span data-stu-id="4ef84-156">Update</span></span>](../api/messagerule-update.md) | [<span data-ttu-id="4ef84-157">messageRule</span><span class="sxs-lookup"><span data-stu-id="4ef84-157">messageRule</span></span>](messagerule.md) |<span data-ttu-id="4ef84-158">Изменяет записываемые свойства объекта **messageRule** и сохраняет изменения.</span><span class="sxs-lookup"><span data-stu-id="4ef84-158">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="4ef84-159">Удаление</span><span class="sxs-lookup"><span data-stu-id="4ef84-159">Delete</span></span>](../api/messagerule-delete.md) | <span data-ttu-id="4ef84-160">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="4ef84-160">None</span></span> |<span data-ttu-id="4ef84-161">Удаляет указанный объект **messageRule**.</span><span class="sxs-lookup"><span data-stu-id="4ef84-161">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->