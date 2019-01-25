---
title: Тип ресурса messageRule
description: Правило, которое применяется к сообщениям в папке "Входящие" пользователя.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 790968563acfe7ed1fb760839454957bb2ac0ecb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522387"
---
# <a name="messagerule-resource-type"></a><span data-ttu-id="cccff-103">Тип ресурса messageRule</span><span class="sxs-lookup"><span data-stu-id="cccff-103">messageRule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cccff-104">Правило, которое применяется к сообщениям в папке "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="cccff-104">A rule that applies to messages in the Inbox of a user.</span></span>

<span data-ttu-id="cccff-105">В Outlook можно настроить правила для сообщений в папке "Входящие", согласно которым при соблюдении определенных условий выполняются нужные действия.</span><span class="sxs-lookup"><span data-stu-id="cccff-105">In Outlook, you can set up rules for incoming messages in the Inbox to carry out specific actions upon certain conditions.</span></span> 

<span data-ttu-id="cccff-106">Программным способом можно получить доступ к правилам, используя свойство навигации **messageRules** [папки](mailfolder.md) "Входящие".</span><span class="sxs-lookup"><span data-stu-id="cccff-106">Programmatically, you can access rules through the **messageRules** navigation property of the Inbox [folder](mailfolder.md).</span></span> <span data-ttu-id="cccff-107">Каждое правило определено ресурсом **messageRule**, доступные действия правил определяются сложным типом [messageRuleActions](messageruleactions.md), а доступные условия и исключения для правил — сложным типом [messageRulePredicates](messagerulepredicates.md).</span><span class="sxs-lookup"><span data-stu-id="cccff-107">Each rule is represented by this **messageRule** resource, available rule actions are represented by the [messageRuleActions](messageruleactions.md) complex type, and available rule conditions and exceptions are represented by the [messageRulePredicates](messagerulepredicates.md) complex type.</span></span>


## <a name="properties"></a><span data-ttu-id="cccff-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cccff-108">Properties</span></span>
| <span data-ttu-id="cccff-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cccff-109">Property</span></span>     | <span data-ttu-id="cccff-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cccff-110">Type</span></span>   |<span data-ttu-id="cccff-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cccff-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cccff-112">actions</span><span class="sxs-lookup"><span data-stu-id="cccff-112">actions</span></span> | [<span data-ttu-id="cccff-113">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="cccff-113">messageRuleActions</span></span>](messageruleactions.md) | <span data-ttu-id="cccff-114">Действия, которые нужно применить к сообщению при выполнении определенных условий.</span><span class="sxs-lookup"><span data-stu-id="cccff-114">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="cccff-115">conditions</span><span class="sxs-lookup"><span data-stu-id="cccff-115">conditions</span></span> | [<span data-ttu-id="cccff-116">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="cccff-116">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="cccff-117">Условия, при соблюдении которых с указанным правилом выполняются соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="cccff-117">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="cccff-118">displayName</span><span class="sxs-lookup"><span data-stu-id="cccff-118">displayName</span></span> | <span data-ttu-id="cccff-119">String</span><span class="sxs-lookup"><span data-stu-id="cccff-119">String</span></span> | <span data-ttu-id="cccff-120">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="cccff-120">The display name of the rule.</span></span> |
| <span data-ttu-id="cccff-121">exceptions</span><span class="sxs-lookup"><span data-stu-id="cccff-121">exceptions</span></span> | [<span data-ttu-id="cccff-122">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="cccff-122">messageRulePredicates</span></span>](messagerulepredicates.md) | <span data-ttu-id="cccff-123">Условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="cccff-123">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="cccff-124">hasError</span><span class="sxs-lookup"><span data-stu-id="cccff-124">hasError</span></span> | <span data-ttu-id="cccff-125">Логическое</span><span class="sxs-lookup"><span data-stu-id="cccff-125">Boolean</span></span> | <span data-ttu-id="cccff-126">Указывает, является ли правило ошибкой.</span><span class="sxs-lookup"><span data-stu-id="cccff-126">Indicates whether the rule is in an error condition.</span></span> <span data-ttu-id="cccff-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cccff-127">Read-only.</span></span> |
| <span data-ttu-id="cccff-128">id</span><span class="sxs-lookup"><span data-stu-id="cccff-128">id</span></span> |<span data-ttu-id="cccff-129">String</span><span class="sxs-lookup"><span data-stu-id="cccff-129">String</span></span>|<span data-ttu-id="cccff-130">Уникальный идентификатор правила.</span><span class="sxs-lookup"><span data-stu-id="cccff-130">The unique identifier of the rule.</span></span> <span data-ttu-id="cccff-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cccff-131">Read-only.</span></span>|
| <span data-ttu-id="cccff-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="cccff-132">isEnabled</span></span> | <span data-ttu-id="cccff-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="cccff-133">Boolean</span></span> | <span data-ttu-id="cccff-134">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="cccff-134">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="cccff-135">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="cccff-135">isReadOnly</span></span> | <span data-ttu-id="cccff-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="cccff-136">Boolean</span></span> | <span data-ttu-id="cccff-137">Указывает, доступно ли правило только для чтения и можно ли изменить или удалить его с помощью REST API для правил.</span><span class="sxs-lookup"><span data-stu-id="cccff-137">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="cccff-138">sequence</span><span class="sxs-lookup"><span data-stu-id="cccff-138">sequence</span></span> | <span data-ttu-id="cccff-139">Int32</span><span class="sxs-lookup"><span data-stu-id="cccff-139">Int32</span></span> | <span data-ttu-id="cccff-140">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="cccff-140">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="cccff-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cccff-141">JSON representation</span></span>
<span data-ttu-id="cccff-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cccff-142">Here is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="cccff-143">Методы</span><span class="sxs-lookup"><span data-stu-id="cccff-143">Methods</span></span>
| <span data-ttu-id="cccff-144">Метод</span><span class="sxs-lookup"><span data-stu-id="cccff-144">Method</span></span>           | <span data-ttu-id="cccff-145">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cccff-145">Return Type</span></span>    |<span data-ttu-id="cccff-146">Описание</span><span class="sxs-lookup"><span data-stu-id="cccff-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cccff-147">Список правил</span><span class="sxs-lookup"><span data-stu-id="cccff-147">List rules</span></span>](../api/mailfolder-list-messagerules.md) | <span data-ttu-id="cccff-148">Коллекция [messageRule](messagerule.md)</span><span class="sxs-lookup"><span data-stu-id="cccff-148">[messageRule](messagerule.md) collection</span></span> |<span data-ttu-id="cccff-149">Получает все объекты **messageRule**, определенные для папки "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="cccff-149">Get all the **messageRule** objects defined for the user's Inbox.</span></span>|
|[<span data-ttu-id="cccff-150">Получение правила</span><span class="sxs-lookup"><span data-stu-id="cccff-150">Get rule</span></span>](../api/messagerule-get.md) | [<span data-ttu-id="cccff-151">messageRule</span><span class="sxs-lookup"><span data-stu-id="cccff-151">messageRule</span></span>](messagerule.md) |<span data-ttu-id="cccff-152">Считывает свойства и отношения объекта **messageRule**.</span><span class="sxs-lookup"><span data-stu-id="cccff-152">Read the properties and relationships of a **messageRule** object.</span></span>|
|[<span data-ttu-id="cccff-153">Создание</span><span class="sxs-lookup"><span data-stu-id="cccff-153">Create</span></span>](../api/mailfolder-post-messagerules.md) | [<span data-ttu-id="cccff-154">messageRule</span><span class="sxs-lookup"><span data-stu-id="cccff-154">messageRule</span></span>](messagerule.md) |<span data-ttu-id="cccff-155">Создает объект **messageRule**, определяя набор условий и действий.</span><span class="sxs-lookup"><span data-stu-id="cccff-155">Create a **messageRule** object by specifying a set of conditions and actions.</span></span>|
|[<span data-ttu-id="cccff-156">Обновление</span><span class="sxs-lookup"><span data-stu-id="cccff-156">Update</span></span>](../api/messagerule-update.md) | [<span data-ttu-id="cccff-157">messageRule</span><span class="sxs-lookup"><span data-stu-id="cccff-157">messageRule</span></span>](messagerule.md) |<span data-ttu-id="cccff-158">Изменяет записываемые свойства объекта **messageRule** и сохраняет изменения.</span><span class="sxs-lookup"><span data-stu-id="cccff-158">Change writable properties on a **messageRule** object and save the changes.</span></span> |
|[<span data-ttu-id="cccff-159">Удаление</span><span class="sxs-lookup"><span data-stu-id="cccff-159">Delete</span></span>](../api/messagerule-delete.md) | <span data-ttu-id="cccff-160">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="cccff-160">None</span></span> |<span data-ttu-id="cccff-161">Удаляет указанный объект **messageRule**.</span><span class="sxs-lookup"><span data-stu-id="cccff-161">Delete the specified **messageRule** object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/messagerule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
