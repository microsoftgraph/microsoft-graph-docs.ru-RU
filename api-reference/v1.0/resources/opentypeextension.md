---
title: Тип ресурсов openTypeExtension (открытые расширения)
description: Открытые расширения (прежнее название — расширения данных Office 365) позволяют легко добавлять нетипизированные свойства непосредственно в ресурс в Microsoft Graph.
localization_priority: Priority
author: dkershaw10
ms.prod: extensions
doc_type: resourcePageType
ms.openlocfilehash: 55777fd3338f362d56934479246ea477459c52cc
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863812"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="75c60-103">Тип ресурсов openTypeExtension (открытые расширения)</span><span class="sxs-lookup"><span data-stu-id="75c60-103">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="75c60-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75c60-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75c60-105">Открытые расширения (прежнее название — расширения данных Office 365) позволяют легко добавлять нетипизированные свойства непосредственно в ресурс в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="75c60-105">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>

<span data-ttu-id="75c60-106">Открытые расширения представлены ресурсом **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="75c60-106">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="75c60-107">Все открытые расширения, добавленные в ресурс, отображаются в свойстве навигации **extensions**, которое является производным от абстрактного типа [extension](extension.md).</span><span class="sxs-lookup"><span data-stu-id="75c60-107">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span> <span data-ttu-id="75c60-108">Каждое расширение, помимо пользовательских данных, содержит свойство **extensionName** — единственное предопределенное записываемое свойство для всех расширений.</span><span class="sxs-lookup"><span data-stu-id="75c60-108">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span>

<span data-ttu-id="75c60-109">Чтобы обеспечить уникальность имен расширений, можно использовать формат обратных DNS, который зависит от _принадлежащего вам домена_, например `Com.Contoso.ContactInfo`.</span><span class="sxs-lookup"><span data-stu-id="75c60-109">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="75c60-110">Не указывайте домен Майкрософт (`Com.Microsoft` или `Com.OnMicrosoft`) в имени расширения.</span><span class="sxs-lookup"><span data-stu-id="75c60-110">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="75c60-111">Пример открытого расширения см. в статье [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users).</span><span class="sxs-lookup"><span data-stu-id="75c60-111">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="75c60-112">Открытые расширения поддерживаются указанными ниже ресурсами в соответствующих версиях — общедоступной (1.0 или бета-версии) или предварительной (бета-версии).</span><span class="sxs-lookup"><span data-stu-id="75c60-112">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

|<span data-ttu-id="75c60-113">Ресурс</span><span class="sxs-lookup"><span data-stu-id="75c60-113">Resource</span></span> |<span data-ttu-id="75c60-114">Версия</span><span class="sxs-lookup"><span data-stu-id="75c60-114">Version</span></span> |
|:---------------|:-------|
| [<span data-ttu-id="75c60-115">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="75c60-115">Administrative unit</span></span>](/graph/api/resources/administrativeunit?view=graph-rest-beta)  | <span data-ttu-id="75c60-116">Только предварительная версия</span><span class="sxs-lookup"><span data-stu-id="75c60-116">Preview only</span></span> |
| <span data-ttu-id="75c60-117">[event](event.md) для календаря</span><span class="sxs-lookup"><span data-stu-id="75c60-117">[Calendar event](event.md)</span></span> | <span data-ttu-id="75c60-118">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="75c60-118">GA</span></span> |
| <span data-ttu-id="75c60-119">[event](event.md) для календаря группы</span><span class="sxs-lookup"><span data-stu-id="75c60-119">Group [calendar event](event.md)</span></span> | <span data-ttu-id="75c60-120">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="75c60-120">GA</span></span> |
| <span data-ttu-id="75c60-121">[post](post.md) цепочки беседы группы</span><span class="sxs-lookup"><span data-stu-id="75c60-121">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="75c60-122">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="75c60-122">GA</span></span> |
| [<span data-ttu-id="75c60-123">device</span><span class="sxs-lookup"><span data-stu-id="75c60-123">device</span></span>](device.md) | <span data-ttu-id="75c60-124">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="75c60-124">GA</span></span> |
| [<span data-ttu-id="75c60-125">group</span><span class="sxs-lookup"><span data-stu-id="75c60-125">group</span></span>](group.md) | <span data-ttu-id="75c60-126">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="75c60-126">GA</span></span> |
| [<span data-ttu-id="75c60-127">message</span><span class="sxs-lookup"><span data-stu-id="75c60-127">message</span></span>](message.md) | <span data-ttu-id="75c60-128">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="75c60-128">GA</span></span> |
| [<span data-ttu-id="75c60-129">organization</span><span class="sxs-lookup"><span data-stu-id="75c60-129">organization</span></span>](organization.md) | <span data-ttu-id="75c60-130">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="75c60-130">GA</span></span> |
| <span data-ttu-id="75c60-131">[contact](contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="75c60-131">[Personal contact](contact.md)</span></span> | <span data-ttu-id="75c60-132">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="75c60-132">GA</span></span> |
| [<span data-ttu-id="75c60-133">user</span><span class="sxs-lookup"><span data-stu-id="75c60-133">user</span></span>](user.md) | <span data-ttu-id="75c60-134">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="75c60-134">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="75c60-135">Специальные рекомендации для Outlook</span><span class="sxs-lookup"><span data-stu-id="75c60-135">Outlook-specific considerations</span></span>

<span data-ttu-id="75c60-136">Каждое открытое расширение, присутствующее в ресурсе Outlook (событии, сообщении или личном контакте), хранится в [именованном свойстве MAPI](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span><span class="sxs-lookup"><span data-stu-id="75c60-136">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span></span> <span data-ttu-id="75c60-137">Создавая открытые расширения для Outlook, учитывайте, что именованные свойства MAPI в почтовом ящике пользователя — это ограниченный ресурс.</span><span class="sxs-lookup"><span data-stu-id="75c60-137">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="75c60-138">Когда будет достигнута квота именованных свойств пользователя, для этого пользователя невозможно будет создавать другие именованные свойства.</span><span class="sxs-lookup"><span data-stu-id="75c60-138">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="75c60-139">Это может привести к неожиданным действиям пользователей, для работы которых необходимы именованные свойства.</span><span class="sxs-lookup"><span data-stu-id="75c60-139">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="75c60-140">Руководствуйтесь приведенными ниже рекомендациями при создании открытых расширений в ресурсах Outlook.</span><span class="sxs-lookup"><span data-stu-id="75c60-140">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="75c60-141">Создайте минимум необходимых расширений.</span><span class="sxs-lookup"><span data-stu-id="75c60-141">Create the minimum number of extensions required.</span></span> <span data-ttu-id="75c60-142">Большинству приложений должно потребоваться не более одного расширения.</span><span class="sxs-lookup"><span data-stu-id="75c60-142">Most applications should require no more than one extension.</span></span> <span data-ttu-id="75c60-143">У расширений нет определенных свойств или структуры, поэтому в одном расширении можно хранить несколько значений.</span><span class="sxs-lookup"><span data-stu-id="75c60-143">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="75c60-144">Избегайте несогласованного именования расширений (например, на основании вводимых пользователями данных и т. д.).</span><span class="sxs-lookup"><span data-stu-id="75c60-144">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="75c60-145">При создании открытого расширения с новым именем, которое ранее не использовалось в почтовом ящике пользователя, всегда создается новое именованное свойство MAPI.</span><span class="sxs-lookup"><span data-stu-id="75c60-145">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="75c60-146">При удалении расширения именованное свойство не удаляется.</span><span class="sxs-lookup"><span data-stu-id="75c60-146">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="75c60-147">Использование открытых расширений (для ресурсов Outlook) или расширенных свойств</span><span class="sxs-lookup"><span data-stu-id="75c60-147">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="75c60-148">Открытые расширения — рекомендуемое решение для большинства сценариев, предполагающих хранение пользовательских данных и доступ к ним.</span><span class="sxs-lookup"><span data-stu-id="75c60-148">Open extensions are the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="75c60-149">Если вам нужно получить доступ к пользовательским данным для свойств MAPI Outlook, которые еще не предоставлены при помощи [метаданных API Microsoft Graph](https://developer.microsoft.com/graph/docs/overview/call_api), используйте [расширенные свойства и соответствующий REST API](extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="75c60-149">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="75c60-150">Вы можете проверить, какие свойства предоставляются с помощью метаданных, на странице [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span><span class="sxs-lookup"><span data-stu-id="75c60-150">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="75c60-151">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="75c60-151">JSON representation</span></span>

<span data-ttu-id="75c60-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75c60-152">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="75c60-153">Свойства</span><span class="sxs-lookup"><span data-stu-id="75c60-153">Properties</span></span>

|<span data-ttu-id="75c60-154">Свойство</span><span class="sxs-lookup"><span data-stu-id="75c60-154">Property</span></span> | <span data-ttu-id="75c60-155">Тип</span><span class="sxs-lookup"><span data-stu-id="75c60-155">Type</span></span> | <span data-ttu-id="75c60-156">Описание</span><span class="sxs-lookup"><span data-stu-id="75c60-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="75c60-157">extensionName</span><span class="sxs-lookup"><span data-stu-id="75c60-157">extensionName</span></span>|<span data-ttu-id="75c60-158">String</span><span class="sxs-lookup"><span data-stu-id="75c60-158">String</span></span>|<span data-ttu-id="75c60-159">A unique text identifier for an open type open extension.</span><span class="sxs-lookup"><span data-stu-id="75c60-159">A unique text identifier for an open type open extension.</span></span> <span data-ttu-id="75c60-160">Required.</span><span class="sxs-lookup"><span data-stu-id="75c60-160">Required.</span></span>|
|<span data-ttu-id="75c60-161">id</span><span class="sxs-lookup"><span data-stu-id="75c60-161">id</span></span>|<span data-ttu-id="75c60-162">String</span><span class="sxs-lookup"><span data-stu-id="75c60-162">String</span></span>| <span data-ttu-id="75c60-163">A fully qualified identifier that concatenates the extension type with the **extensionName**.</span><span class="sxs-lookup"><span data-stu-id="75c60-163">A fully qualified identifier that concatenates the extension type with the **extensionName**.</span></span> <span data-ttu-id="75c60-164">Read-only.</span><span class="sxs-lookup"><span data-stu-id="75c60-164">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75c60-165">Связи</span><span class="sxs-lookup"><span data-stu-id="75c60-165">Relationships</span></span>

<span data-ttu-id="75c60-166">Нет</span><span class="sxs-lookup"><span data-stu-id="75c60-166">None</span></span>

## <a name="methods"></a><span data-ttu-id="75c60-167">Методы</span><span class="sxs-lookup"><span data-stu-id="75c60-167">Methods</span></span>

|<span data-ttu-id="75c60-168">Метод</span><span class="sxs-lookup"><span data-stu-id="75c60-168">Method</span></span> | <span data-ttu-id="75c60-169">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="75c60-169">Return Type</span></span> | <span data-ttu-id="75c60-170">Описание</span><span class="sxs-lookup"><span data-stu-id="75c60-170">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="75c60-171">[Создание](../api/opentypeextension-post-opentypeextension.md);</span><span class="sxs-lookup"><span data-stu-id="75c60-171">[Create](../api/opentypeextension-post-opentypeextension.md)</span></span> | <span data-ttu-id="75c60-172">Объект [openTypeExtension](opentypeextension.md) (в существующем экземпляре ресурса) либо новый ресурс [contact](../resources/contact.md), [event](../resources/event.md) или [message](../resources/message.md), содержащий объект openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="75c60-172">[openTypeExtension](opentypeextension.md) (in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object</span></span> | <span data-ttu-id="75c60-173">Создание объекта openTypeExtension в существующем или новом экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="75c60-173">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="75c60-174">Get</span><span class="sxs-lookup"><span data-stu-id="75c60-174">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="75c60-175">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="75c60-175">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="75c60-176">Чтение свойств и связей объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="75c60-176">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="75c60-177">Update</span><span class="sxs-lookup"><span data-stu-id="75c60-177">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="75c60-178">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="75c60-178">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="75c60-179">Обновление объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="75c60-179">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="75c60-180">Delete</span><span class="sxs-lookup"><span data-stu-id="75c60-180">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="75c60-181">Нет</span><span class="sxs-lookup"><span data-stu-id="75c60-181">None</span></span> |<span data-ttu-id="75c60-182">Удаление объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="75c60-182">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
