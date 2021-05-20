---
title: Тип ресурсов openTypeExtension (открытые расширения)
description: Открытые расширения (прежнее название — расширения данных Office 365) позволяют легко добавлять нетипизированные свойства непосредственно в ресурс в Microsoft Graph.
localization_priority: Priority
author: dkershaw10
ms.prod: extensions
doc_type: resourcePageType
ms.openlocfilehash: ad9baa66d82437d53fc500a99205cf9f4d03280c
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547283"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="a0265-103">Тип ресурсов openTypeExtension (открытые расширения)</span><span class="sxs-lookup"><span data-stu-id="a0265-103">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="a0265-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0265-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a0265-105">Открытые расширения (прежнее название — расширения данных Office 365) позволяют легко добавлять нетипизированные свойства непосредственно в ресурс в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a0265-105">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>

<span data-ttu-id="a0265-106">Открытые расширения представлены ресурсом **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="a0265-106">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="a0265-107">Все открытые расширения, добавленные в ресурс, отображаются в свойстве навигации **extensions**, которое является производным от абстрактного типа [extension](extension.md).</span><span class="sxs-lookup"><span data-stu-id="a0265-107">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span> <span data-ttu-id="a0265-108">Каждое расширение, помимо пользовательских данных, содержит свойство **extensionName** — единственное предопределенное записываемое свойство для всех расширений.</span><span class="sxs-lookup"><span data-stu-id="a0265-108">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span>

<span data-ttu-id="a0265-109">Чтобы обеспечить уникальность имен расширений, можно использовать формат обратных DNS, который зависит от _принадлежащего вам домена_, например `Com.Contoso.ContactInfo`.</span><span class="sxs-lookup"><span data-stu-id="a0265-109">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="a0265-110">Не указывайте домен Майкрософт (`Com.Microsoft` или `Com.OnMicrosoft`) в имени расширения.</span><span class="sxs-lookup"><span data-stu-id="a0265-110">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="a0265-111">Пример открытого расширения см. в статье [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users).</span><span class="sxs-lookup"><span data-stu-id="a0265-111">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="a0265-112">Открытые расширения поддерживаются указанными ниже ресурсами в соответствующих версиях — общедоступной (1.0 или бета-версии) или предварительной (бета-версии).</span><span class="sxs-lookup"><span data-stu-id="a0265-112">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

|<span data-ttu-id="a0265-113">Ресурс</span><span class="sxs-lookup"><span data-stu-id="a0265-113">Resource</span></span> |<span data-ttu-id="a0265-114">Версия</span><span class="sxs-lookup"><span data-stu-id="a0265-114">Version</span></span> |
|:---------------|:-------|
| [<span data-ttu-id="a0265-115">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="a0265-115">Administrative unit</span></span>](/graph/api/resources/administrativeunit)  | <span data-ttu-id="a0265-116">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="a0265-116">GA</span></span> |
| [<span data-ttu-id="a0265-117">Событие календаря</span><span class="sxs-lookup"><span data-stu-id="a0265-117">Calendar event</span></span>](event.md) | <span data-ttu-id="a0265-118">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="a0265-118">GA</span></span> |
| <span data-ttu-id="a0265-119">[event](event.md) для календаря группы</span><span class="sxs-lookup"><span data-stu-id="a0265-119">Group [calendar event](event.md)</span></span> | <span data-ttu-id="a0265-120">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="a0265-120">GA</span></span> |
| <span data-ttu-id="a0265-121">[post](post.md) цепочки беседы группы</span><span class="sxs-lookup"><span data-stu-id="a0265-121">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="a0265-122">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="a0265-122">GA</span></span> |
| [<span data-ttu-id="a0265-123">device</span><span class="sxs-lookup"><span data-stu-id="a0265-123">device</span></span>](device.md) | <span data-ttu-id="a0265-124">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="a0265-124">GA</span></span> |
| [<span data-ttu-id="a0265-125">group</span><span class="sxs-lookup"><span data-stu-id="a0265-125">group</span></span>](group.md) | <span data-ttu-id="a0265-126">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="a0265-126">GA</span></span> |
| [<span data-ttu-id="a0265-127">message</span><span class="sxs-lookup"><span data-stu-id="a0265-127">message</span></span>](message.md) | <span data-ttu-id="a0265-128">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="a0265-128">GA</span></span> |
| [<span data-ttu-id="a0265-129">organization</span><span class="sxs-lookup"><span data-stu-id="a0265-129">organization</span></span>](organization.md) | <span data-ttu-id="a0265-130">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="a0265-130">GA</span></span> |
| [<span data-ttu-id="a0265-131">Личный контакт</span><span class="sxs-lookup"><span data-stu-id="a0265-131">Personal contact</span></span>](contact.md) | <span data-ttu-id="a0265-132">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="a0265-132">GA</span></span> |
| [<span data-ttu-id="a0265-133">user</span><span class="sxs-lookup"><span data-stu-id="a0265-133">user</span></span>](user.md) | <span data-ttu-id="a0265-134">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="a0265-134">GA</span></span> |
| [<span data-ttu-id="a0265-135">Задача</span><span class="sxs-lookup"><span data-stu-id="a0265-135">Task</span></span>](todotask.md)  | <span data-ttu-id="a0265-136">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="a0265-136">GA</span></span> |
| [<span data-ttu-id="a0265-137">Список задач</span><span class="sxs-lookup"><span data-stu-id="a0265-137">Task list</span></span>](todotasklist.md)  | <span data-ttu-id="a0265-138">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="a0265-138">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="a0265-139">Специальные рекомендации для Outlook</span><span class="sxs-lookup"><span data-stu-id="a0265-139">Outlook-specific considerations</span></span>

<span data-ttu-id="a0265-140">Каждое открытое расширение, присутствующее в ресурсе Outlook (событии, сообщении или личном контакте), хранится в [именованном свойстве MAPI](/office/client-developer/outlook/mapi/mapi-named-properties).</span><span class="sxs-lookup"><span data-stu-id="a0265-140">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](/office/client-developer/outlook/mapi/mapi-named-properties).</span></span> <span data-ttu-id="a0265-141">Создавая открытые расширения для Outlook, учитывайте, что именованные свойства MAPI в почтовом ящике пользователя — это ограниченный ресурс.</span><span class="sxs-lookup"><span data-stu-id="a0265-141">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="a0265-142">Когда будет достигнута квота именованных свойств пользователя, для этого пользователя невозможно будет создавать другие именованные свойства.</span><span class="sxs-lookup"><span data-stu-id="a0265-142">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="a0265-143">Это может привести к неожиданным действиям пользователей, для работы которых необходимы именованные свойства.</span><span class="sxs-lookup"><span data-stu-id="a0265-143">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="a0265-144">Руководствуйтесь приведенными ниже рекомендациями при создании открытых расширений в ресурсах Outlook.</span><span class="sxs-lookup"><span data-stu-id="a0265-144">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="a0265-145">Создайте минимум необходимых расширений.</span><span class="sxs-lookup"><span data-stu-id="a0265-145">Create the minimum number of extensions required.</span></span> <span data-ttu-id="a0265-146">Большинству приложений должно потребоваться не более одного расширения.</span><span class="sxs-lookup"><span data-stu-id="a0265-146">Most applications should require no more than one extension.</span></span> <span data-ttu-id="a0265-147">У расширений нет определенных свойств или структуры, поэтому в одном расширении можно хранить несколько значений.</span><span class="sxs-lookup"><span data-stu-id="a0265-147">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="a0265-148">Избегайте несогласованного именования расширений (например, на основании вводимых пользователями данных и т. д.).</span><span class="sxs-lookup"><span data-stu-id="a0265-148">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="a0265-149">При создании открытого расширения с новым именем, которое ранее не использовалось в почтовом ящике пользователя, всегда создается новое именованное свойство MAPI.</span><span class="sxs-lookup"><span data-stu-id="a0265-149">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="a0265-150">При удалении расширения именованное свойство не удаляется.</span><span class="sxs-lookup"><span data-stu-id="a0265-150">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="a0265-151">Использование открытых расширений (для ресурсов Outlook) или расширенных свойств</span><span class="sxs-lookup"><span data-stu-id="a0265-151">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="a0265-152">Открытые расширения — рекомендуемое решение для большинства сценариев, предполагающих хранение пользовательских данных и доступ к ним.</span><span class="sxs-lookup"><span data-stu-id="a0265-152">Open extensions are the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="a0265-153">Если вам нужно получить доступ к пользовательским данным для свойств MAPI Outlook, которые еще не предоставлены при помощи [метаданных API Microsoft Graph](/graph/traverse-the-graph#microsoft-graph-api-metadata), используйте [расширенные свойства и соответствующий REST API](extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="a0265-153">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](/graph/traverse-the-graph#microsoft-graph-api-metadata), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="a0265-154">Вы можете проверить, какие свойства предоставляются с помощью метаданных, на странице https://graph.microsoft.com/v1.0/$metadata.</span><span class="sxs-lookup"><span data-stu-id="a0265-154">You can verify which properties the metadata exposes at https://graph.microsoft.com/v1.0/$metadata.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0265-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0265-155">JSON representation</span></span>

<span data-ttu-id="a0265-156">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0265-156">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.extension",
  "@odata.type": "microsoft.graph.openTypeExtension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}
```

## <a name="properties"></a><span data-ttu-id="a0265-157">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0265-157">Properties</span></span>

|<span data-ttu-id="a0265-158">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0265-158">Property</span></span> | <span data-ttu-id="a0265-159">Тип</span><span class="sxs-lookup"><span data-stu-id="a0265-159">Type</span></span> | <span data-ttu-id="a0265-160">Описание</span><span class="sxs-lookup"><span data-stu-id="a0265-160">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a0265-161">extensionName</span><span class="sxs-lookup"><span data-stu-id="a0265-161">extensionName</span></span>|<span data-ttu-id="a0265-162">String</span><span class="sxs-lookup"><span data-stu-id="a0265-162">String</span></span>|<span data-ttu-id="a0265-p107">Уникальный текстовый идентификатор для открытых расширений открытого типа. Обязательно свойство.</span><span class="sxs-lookup"><span data-stu-id="a0265-p107">A unique text identifier for an open type open extension. Required.</span></span>|
|<span data-ttu-id="a0265-165">id</span><span class="sxs-lookup"><span data-stu-id="a0265-165">id</span></span>|<span data-ttu-id="a0265-166">String</span><span class="sxs-lookup"><span data-stu-id="a0265-166">String</span></span>| <span data-ttu-id="a0265-p108">Полный идентификатор, в котором сцеплены тип расширения и свойство **extensionName**. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a0265-p108">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0265-169">Связи</span><span class="sxs-lookup"><span data-stu-id="a0265-169">Relationships</span></span>

<span data-ttu-id="a0265-170">Нет</span><span class="sxs-lookup"><span data-stu-id="a0265-170">None</span></span>

## <a name="methods"></a><span data-ttu-id="a0265-171">Методы</span><span class="sxs-lookup"><span data-stu-id="a0265-171">Methods</span></span>

|<span data-ttu-id="a0265-172">Метод</span><span class="sxs-lookup"><span data-stu-id="a0265-172">Method</span></span> | <span data-ttu-id="a0265-173">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a0265-173">Return Type</span></span> | <span data-ttu-id="a0265-174">Описание</span><span class="sxs-lookup"><span data-stu-id="a0265-174">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="a0265-175">Создание</span><span class="sxs-lookup"><span data-stu-id="a0265-175">Create</span></span>](../api/opentypeextension-post-opentypeextension.md) | <span data-ttu-id="a0265-176">Объект [openTypeExtension](opentypeextension.md) (в существующем экземпляре ресурса) либо новый ресурс [contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md), [post](post.md), [todoTask](todotask.md) или [todoTaskList](todotasklist.md), содержащий объект openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="a0265-176">[openTypeExtension](opentypeextension.md) (in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md), [post](post.md), [todoTask](todotask.md), or [todoTaskList](todotasklist.md) that contains an openTypeExtension object</span></span> | <span data-ttu-id="a0265-177">Создание объекта openTypeExtension в существующем или новом экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="a0265-177">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="a0265-178">Get</span><span class="sxs-lookup"><span data-stu-id="a0265-178">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="a0265-179">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="a0265-179">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="a0265-180">Чтение свойств и связей объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="a0265-180">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="a0265-181">Update</span><span class="sxs-lookup"><span data-stu-id="a0265-181">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="a0265-182">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="a0265-182">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="a0265-183">Обновление объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="a0265-183">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="a0265-184">Delete</span><span class="sxs-lookup"><span data-stu-id="a0265-184">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="a0265-185">Нет</span><span class="sxs-lookup"><span data-stu-id="a0265-185">None</span></span> |<span data-ttu-id="a0265-186">Удаление объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="a0265-186">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
