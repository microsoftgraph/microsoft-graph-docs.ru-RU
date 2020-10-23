---
title: Тип ресурсов openTypeExtension (открытые расширения)
description: Открытые расширения (прежнее название — расширения данных Office 365) позволяют легко добавлять нетипизированные свойства непосредственно в ресурс в Microsoft Graph.
localization_priority: Normal
author: dkershaw10
doc_type: resourcePageType
ms.prod: extensions
ms.openlocfilehash: 457eaaae7f9a595061683999f818cb0f3af8f680
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706886"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="bbadc-103">Тип ресурсов openTypeExtension (открытые расширения)</span><span class="sxs-lookup"><span data-stu-id="bbadc-103">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="bbadc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbadc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbadc-105">Открытые расширения (прежнее название — расширения данных Office 365) позволяют легко добавлять нетипизированные свойства непосредственно в ресурс в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bbadc-105">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>
<span data-ttu-id="bbadc-106">Открытые расширения представлены ресурсом **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="bbadc-106">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="bbadc-107">Все открытые расширения, добавленные в ресурс, отображаются в свойстве навигации **extensions**, которое является производным от абстрактного типа [extension](extension.md).</span><span class="sxs-lookup"><span data-stu-id="bbadc-107">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span>  <span data-ttu-id="bbadc-108">Каждое расширение, помимо пользовательских данных, содержит свойство **extensionName** — единственное предопределенное записываемое свойство для всех расширений.</span><span class="sxs-lookup"><span data-stu-id="bbadc-108">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span> <span data-ttu-id="bbadc-109">Чтобы обеспечить уникальность имен расширений, можно использовать формат обратных DNS, который зависит от _принадлежащего вам домена_, например `Com.Contoso.ContactInfo`.</span><span class="sxs-lookup"><span data-stu-id="bbadc-109">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="bbadc-110">Не указывайте домен Майкрософт (`Com.Microsoft` или `Com.OnMicrosoft`) в имени расширения.</span><span class="sxs-lookup"><span data-stu-id="bbadc-110">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="bbadc-111">Пример открытого расширения см. в статье [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users).</span><span class="sxs-lookup"><span data-stu-id="bbadc-111">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="bbadc-112">Открытые расширения поддерживаются указанными ниже ресурсами в соответствующих версиях — общедоступной (1.0 или бета-версии) или предварительной (бета-версии).</span><span class="sxs-lookup"><span data-stu-id="bbadc-112">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

| <span data-ttu-id="bbadc-113">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bbadc-113">Resource</span></span> | <span data-ttu-id="bbadc-114">Версия</span><span class="sxs-lookup"><span data-stu-id="bbadc-114">Version</span></span> |
|---------------|-------|
| [<span data-ttu-id="bbadc-115">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="bbadc-115">Administrative unit</span></span>](administrativeunit.md)  | <span data-ttu-id="bbadc-116">Только предварительная версия</span><span class="sxs-lookup"><span data-stu-id="bbadc-116">Preview only</span></span> |
| [<span data-ttu-id="bbadc-117">Событие календаря</span><span class="sxs-lookup"><span data-stu-id="bbadc-117">Calendar event</span></span>](event.md) | <span data-ttu-id="bbadc-118">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="bbadc-118">GA</span></span> |
| <span data-ttu-id="bbadc-119">[event](event.md) для календаря группы</span><span class="sxs-lookup"><span data-stu-id="bbadc-119">Group [calendar event](event.md)</span></span> | <span data-ttu-id="bbadc-120">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="bbadc-120">GA</span></span> |
| <span data-ttu-id="bbadc-121">[post](post.md) цепочки беседы группы</span><span class="sxs-lookup"><span data-stu-id="bbadc-121">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="bbadc-122">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="bbadc-122">GA</span></span> |
| [<span data-ttu-id="bbadc-123">Устройство</span><span class="sxs-lookup"><span data-stu-id="bbadc-123">Device</span></span>](device.md) | <span data-ttu-id="bbadc-124">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="bbadc-124">GA</span></span> |
| [<span data-ttu-id="bbadc-125">Группа</span><span class="sxs-lookup"><span data-stu-id="bbadc-125">Group</span></span>](group.md) | <span data-ttu-id="bbadc-126">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="bbadc-126">GA</span></span> |
| [<span data-ttu-id="bbadc-127">Сообщение</span><span class="sxs-lookup"><span data-stu-id="bbadc-127">Message</span></span>](message.md) | <span data-ttu-id="bbadc-128">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="bbadc-128">GA</span></span> |
| [<span data-ttu-id="bbadc-129">Организация</span><span class="sxs-lookup"><span data-stu-id="bbadc-129">Organization</span></span>](organization.md) | <span data-ttu-id="bbadc-130">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="bbadc-130">GA</span></span> |
| [<span data-ttu-id="bbadc-131">Личный контакт</span><span class="sxs-lookup"><span data-stu-id="bbadc-131">Personal contact</span></span>](contact.md) | <span data-ttu-id="bbadc-132">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="bbadc-132">GA</span></span> |
| [<span data-ttu-id="bbadc-133">Пользователь</span><span class="sxs-lookup"><span data-stu-id="bbadc-133">User</span></span>](user.md) | <span data-ttu-id="bbadc-134">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="bbadc-134">GA</span></span> |
| [<span data-ttu-id="bbadc-135">Задача</span><span class="sxs-lookup"><span data-stu-id="bbadc-135">Task</span></span>](todotask.md)  | <span data-ttu-id="bbadc-136">Только предварительная версия</span><span class="sxs-lookup"><span data-stu-id="bbadc-136">Preview only</span></span> ||
| [<span data-ttu-id="bbadc-137">Список задач</span><span class="sxs-lookup"><span data-stu-id="bbadc-137">Task list</span></span>](todotasklist.md)  | <span data-ttu-id="bbadc-138">Только предварительная версия</span><span class="sxs-lookup"><span data-stu-id="bbadc-138">Preview only</span></span> ||

## <a name="outlook-specific-considerations"></a><span data-ttu-id="bbadc-139">Специальные рекомендации для Outlook</span><span class="sxs-lookup"><span data-stu-id="bbadc-139">Outlook-specific considerations</span></span>

<span data-ttu-id="bbadc-140">Каждое открытое расширение, присутствующее в ресурсе Outlook (событии, сообщении или личном контакте), хранится в [именованном свойстве MAPI](/office/client-developer/outlook/mapi/mapi-named-properties).</span><span class="sxs-lookup"><span data-stu-id="bbadc-140">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](/office/client-developer/outlook/mapi/mapi-named-properties).</span></span> <span data-ttu-id="bbadc-141">Создавая открытые расширения для Outlook, учитывайте, что именованные свойства MAPI в почтовом ящике пользователя — это ограниченный ресурс.</span><span class="sxs-lookup"><span data-stu-id="bbadc-141">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="bbadc-142">Когда будет достигнута квота именованных свойств пользователя, для этого пользователя невозможно будет создавать другие именованные свойства.</span><span class="sxs-lookup"><span data-stu-id="bbadc-142">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="bbadc-143">Это может привести к неожиданным действиям пользователей, для работы которых необходимы именованные свойства.</span><span class="sxs-lookup"><span data-stu-id="bbadc-143">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="bbadc-144">Руководствуйтесь приведенными ниже рекомендациями при создании открытых расширений в ресурсах Outlook.</span><span class="sxs-lookup"><span data-stu-id="bbadc-144">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="bbadc-145">Создайте минимум необходимых расширений.</span><span class="sxs-lookup"><span data-stu-id="bbadc-145">Create the minimum number of extensions required.</span></span> <span data-ttu-id="bbadc-146">Большинству приложений должно потребоваться не более одного расширения.</span><span class="sxs-lookup"><span data-stu-id="bbadc-146">Most applications should require no more than one extension.</span></span> <span data-ttu-id="bbadc-147">У расширений нет определенных свойств или структуры, поэтому в одном расширении можно хранить несколько значений.</span><span class="sxs-lookup"><span data-stu-id="bbadc-147">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="bbadc-148">Избегайте несогласованного именования расширений (например, на основании вводимых пользователями данных и т. д.).</span><span class="sxs-lookup"><span data-stu-id="bbadc-148">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="bbadc-149">При создании открытого расширения с новым именем, которое ранее не использовалось в почтовом ящике пользователя, всегда создается новое именованное свойство MAPI.</span><span class="sxs-lookup"><span data-stu-id="bbadc-149">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="bbadc-150">При удалении расширения именованное свойство не удаляется.</span><span class="sxs-lookup"><span data-stu-id="bbadc-150">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="bbadc-151">Использование открытых расширений (для ресурсов Outlook) или расширенных свойств</span><span class="sxs-lookup"><span data-stu-id="bbadc-151">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="bbadc-152">Открытые расширения — рекомендуемое решение для большинства сценариев, предполагающих хранение пользовательских данных и доступ к ним.</span><span class="sxs-lookup"><span data-stu-id="bbadc-152">Open extensions are the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="bbadc-153">Если вам нужно получить доступ к пользовательским данным для свойств MAPI Outlook, которые еще не предоставлены при помощи [метаданных API Microsoft Graph](../index.md), используйте [расширенные свойства и соответствующий REST API](extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="bbadc-153">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](../index.md), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="bbadc-154">Вы можете проверить, какие свойства предоставляются с помощью метаданных, на странице [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span><span class="sxs-lookup"><span data-stu-id="bbadc-154">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbadc-155">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bbadc-155">JSON representation</span></span>

<span data-ttu-id="bbadc-156">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="bbadc-156">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openTypeExtension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}
```

## <a name="properties"></a><span data-ttu-id="bbadc-157">Свойства</span><span class="sxs-lookup"><span data-stu-id="bbadc-157">Properties</span></span>

| <span data-ttu-id="bbadc-158">Свойство</span><span class="sxs-lookup"><span data-stu-id="bbadc-158">Property</span></span> | <span data-ttu-id="bbadc-159">Тип</span><span class="sxs-lookup"><span data-stu-id="bbadc-159">Type</span></span> | <span data-ttu-id="bbadc-160">Описание</span><span class="sxs-lookup"><span data-stu-id="bbadc-160">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bbadc-161">extensionName</span><span class="sxs-lookup"><span data-stu-id="bbadc-161">extensionName</span></span>|<span data-ttu-id="bbadc-162">String</span><span class="sxs-lookup"><span data-stu-id="bbadc-162">String</span></span>|<span data-ttu-id="bbadc-p106">Уникальный текстовый идентификатор для модуля обработки данных открытого типа. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbadc-p106">A unique text identifier for an open type data extension. Required.</span></span>|
|<span data-ttu-id="bbadc-165">id</span><span class="sxs-lookup"><span data-stu-id="bbadc-165">id</span></span>|<span data-ttu-id="bbadc-166">String</span><span class="sxs-lookup"><span data-stu-id="bbadc-166">String</span></span>| <span data-ttu-id="bbadc-p107">Полный идентификатор, в котором сцеплены тип расширения и свойство **extensionName**. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bbadc-p107">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbadc-169">Связи</span><span class="sxs-lookup"><span data-stu-id="bbadc-169">Relationships</span></span>

<span data-ttu-id="bbadc-170">Нет</span><span class="sxs-lookup"><span data-stu-id="bbadc-170">None</span></span>

## <a name="methods"></a><span data-ttu-id="bbadc-171">Методы</span><span class="sxs-lookup"><span data-stu-id="bbadc-171">Methods</span></span>

| <span data-ttu-id="bbadc-172">Метод</span><span class="sxs-lookup"><span data-stu-id="bbadc-172">Method</span></span> | <span data-ttu-id="bbadc-173">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bbadc-173">Return Type</span></span> | <span data-ttu-id="bbadc-174">Описание</span><span class="sxs-lookup"><span data-stu-id="bbadc-174">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="bbadc-175">Создание</span><span class="sxs-lookup"><span data-stu-id="bbadc-175">Create</span></span>](../api/opentypeextension-post-opentypeextension.md) | <span data-ttu-id="bbadc-176">[openTypeExtension](opentypeextension.md)(в существующем экземпляре ресурса) или новый [контакт](contact.md), [событие](event.md), [сообщение](message.md), [POST](post.md), [тодотаск](todotask.md)или [тодотасклист](todotasklist.md) , содержащее объект openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="bbadc-176">[openTypeExtension](opentypeextension.md)(in an existing resource instance), or a new [contact](contact.md), [event](event.md), [message](message.md), [post](post.md), [todoTask](todotask.md), or [todoTaskList](todotasklist.md) that contains an openTypeExtension object.</span></span> | <span data-ttu-id="bbadc-177">Создание объекта openTypeExtension в существующем или новом экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="bbadc-177">Create an openTypeExtension object in an existing or new resource instance.</span></span>||[<span data-ttu-id="bbadc-178">Get</span><span class="sxs-lookup"><span data-stu-id="bbadc-178">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="bbadc-179">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="bbadc-179">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="bbadc-180">Чтение свойств и связей объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="bbadc-180">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="bbadc-181">Update</span><span class="sxs-lookup"><span data-stu-id="bbadc-181">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="bbadc-182">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="bbadc-182">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="bbadc-183">Обновление объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="bbadc-183">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="bbadc-184">Delete</span><span class="sxs-lookup"><span data-stu-id="bbadc-184">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="bbadc-185">Нет</span><span class="sxs-lookup"><span data-stu-id="bbadc-185">None</span></span> |<span data-ttu-id="bbadc-186">Удаление объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="bbadc-186">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
