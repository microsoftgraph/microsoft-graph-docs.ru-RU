---
title: Тип ресурса messageRule
description: Правило, которое применяется к сообщениям в папке "Входящие" пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ec7225800c179ae5592c5d2ef040f8a009568ac7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522675"
---
# <a name="messagerule-resource-type"></a><span data-ttu-id="9c33a-103">Тип ресурса messageRule</span><span class="sxs-lookup"><span data-stu-id="9c33a-103">messageRule resource type</span></span>

<span data-ttu-id="9c33a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9c33a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c33a-105">Правило, которое применяется к сообщениям в папке "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="9c33a-105">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="9c33a-106">В Outlook можно настроить правила для сообщений в папке "Входящие", согласно которым при соблюдении определенных условий выполняются нужные действия.</span><span class="sxs-lookup"><span data-stu-id="9c33a-106">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="9c33a-107">Программным способом можно получить доступ к правилам, используя свойство навигации **messageRules** [папки](mailfolder.md) "Входящие".</span><span class="sxs-lookup"><span data-stu-id="9c33a-107">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="9c33a-108">Каждое правило определено ресурсом **messageRule**, доступные действия правил определяются сложным типом [messageRuleActions](messageruleactions.md), а доступные условия и исключения для правил — сложным типом [messageRulePredicates](messagerulepredicates.md).</span><span class="sxs-lookup"><span data-stu-id="9c33a-108">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="9c33a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c33a-109">Properties</span></span>
| <span data-ttu-id="9c33a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c33a-110">Property</span></span>     | <span data-ttu-id="9c33a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9c33a-111">Type</span></span>   |<span data-ttu-id="9c33a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9c33a-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9c33a-113">actions</span><span class="sxs-lookup"><span data-stu-id="9c33a-113">actions</span></span> | [<span data-ttu-id="9c33a-114">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="9c33a-114">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="9c33a-115">Действия, которые нужно применить к сообщению при выполнении определенных условий.</span><span class="sxs-lookup"><span data-stu-id="9c33a-115">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="9c33a-116">conditions</span><span class="sxs-lookup"><span data-stu-id="9c33a-116">conditions</span></span> | [<span data-ttu-id="9c33a-117">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="9c33a-117">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="9c33a-118">Условия, выполнение которых активирует соответствующие действия для указанного правила.</span><span class="sxs-lookup"><span data-stu-id="9c33a-118">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="9c33a-119">displayName</span><span class="sxs-lookup"><span data-stu-id="9c33a-119">displayName</span></span> | <span data-ttu-id="9c33a-120">Строка</span><span class="sxs-lookup"><span data-stu-id="9c33a-120">String</span></span> | <span data-ttu-id="9c33a-121">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="9c33a-121">The display name of the rule.</span></span> |
| <span data-ttu-id="9c33a-122">exceptions</span><span class="sxs-lookup"><span data-stu-id="9c33a-122">exceptions</span></span> | [<span data-ttu-id="9c33a-123">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="9c33a-123">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="9c33a-124">Условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="9c33a-124">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="9c33a-125">hasError</span><span class="sxs-lookup"><span data-stu-id="9c33a-125">hasError</span></span> | <span data-ttu-id="9c33a-126">Логический</span><span class="sxs-lookup"><span data-stu-id="9c33a-126">Boolean</span></span> | <span data-ttu-id="9c33a-127">Указывает, является ли правило ошибкой.</span><span class="sxs-lookup"><span data-stu-id="9c33a-127">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="9c33a-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9c33a-128">Read-only.</span></span> |
| <span data-ttu-id="9c33a-129">id</span><span class="sxs-lookup"><span data-stu-id="9c33a-129">id</span></span> |<span data-ttu-id="9c33a-130">String</span><span class="sxs-lookup"><span data-stu-id="9c33a-130">String</span></span>|<span data-ttu-id="9c33a-131">Уникальный идентификатор правила.</span><span class="sxs-lookup"><span data-stu-id="9c33a-131">The unique identifier of the rule.</span></span> <span data-ttu-id="9c33a-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9c33a-132">Read-only.</span></span>|
| <span data-ttu-id="9c33a-133">isEnabled</span><span class="sxs-lookup"><span data-stu-id="9c33a-133">isEnabled</span></span> | <span data-ttu-id="9c33a-134">Логический</span><span class="sxs-lookup"><span data-stu-id="9c33a-134">Boolean</span></span> | <span data-ttu-id="9c33a-135">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="9c33a-135">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="9c33a-136">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="9c33a-136">isReadOnly</span></span> | <span data-ttu-id="9c33a-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c33a-137">Boolean</span></span> | <span data-ttu-id="9c33a-138">Указывает, доступно ли правило только для чтения и можно ли изменить или удалить его с помощью REST API для правил.</span><span class="sxs-lookup"><span data-stu-id="9c33a-138">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="9c33a-139">sequence</span><span class="sxs-lookup"><span data-stu-id="9c33a-139">sequence</span></span> | <span data-ttu-id="9c33a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="9c33a-140">Int32</span></span> | <span data-ttu-id="9c33a-141">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="9c33a-141">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="9c33a-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9c33a-142">JSON representation</span></span>
<span data-ttu-id="9c33a-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c33a-143">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="9c33a-144">Методы</span><span class="sxs-lookup"><span data-stu-id="9c33a-144">Methods</span></span>
| <span data-ttu-id="9c33a-145">Метод</span><span class="sxs-lookup"><span data-stu-id="9c33a-145">Method</span></span>           | <span data-ttu-id="9c33a-146">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9c33a-146">Return Type</span></span>    |<span data-ttu-id="9c33a-147">Описание</span><span class="sxs-lookup"><span data-stu-id="9c33a-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c33a-148">Список правил</span><span class="sxs-lookup"><span data-stu-id="9c33a-148">List rules</span></span>](../api/mailfolder-list-messagerules.md) | <span data-ttu-id="9c33a-149">Коллекция [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="9c33a-149">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="9c33a-150">Получает все объекты **messageRule**, определенные для папки "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="9c33a-150">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="9c33a-151">Получение правила</span><span class="sxs-lookup"><span data-stu-id="9c33a-151">Get rule</span></span>](../api/messagerule-get.md) | [<span data-ttu-id="9c33a-152">messageRule</span><span class="sxs-lookup"><span data-stu-id="9c33a-152">messageRule</span></span>](messagerule.md) |<span data-ttu-id="9c33a-153">Считывает свойства и отношения объекта **messageRule**.</span><span class="sxs-lookup"><span data-stu-id="9c33a-153">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="9c33a-154">Создание</span><span class="sxs-lookup"><span data-stu-id="9c33a-154">Create</span></span>](../api/mailfolder-post-messagerules.md) | [<span data-ttu-id="9c33a-155">messageRule</span><span class="sxs-lookup"><span data-stu-id="9c33a-155">messageRule</span></span>](messagerule.md) |<span data-ttu-id="9c33a-156">Создает объект **messageRule**, определяя набор условий и действий.</span><span class="sxs-lookup"><span data-stu-id="9c33a-156">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="9c33a-157">Обновление</span><span class="sxs-lookup"><span data-stu-id="9c33a-157">Update</span></span>](../api/messagerule-update.md) | [<span data-ttu-id="9c33a-158">messageRule</span><span class="sxs-lookup"><span data-stu-id="9c33a-158">messageRule</span></span>](messagerule.md) |<span data-ttu-id="9c33a-159">Изменяет записываемые свойства объекта **messageRule** и сохраняет изменения.</span><span class="sxs-lookup"><span data-stu-id="9c33a-159">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|<span data-ttu-id="9c33a-160">[удаление](../api/messagerule-delete.md);</span><span class="sxs-lookup"><span data-stu-id="9c33a-160">[Delete](../api/messagerule-delete.md)</span></span> | <span data-ttu-id="9c33a-161">Нет</span><span class="sxs-lookup"><span data-stu-id="9c33a-161">None</span></span> |<span data-ttu-id="9c33a-162">Удаляет указанный объект **messageRule**.</span><span class="sxs-lookup"><span data-stu-id="9c33a-162">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
