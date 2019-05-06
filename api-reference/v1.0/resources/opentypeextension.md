---
title: Тип ресурсов openTypeExtension (открытые расширения)
description: Открытые расширения (прежнее название — расширения данных Office 365) позволяют легко добавлять нетипизированные свойства непосредственно в ресурс в Microsoft Graph.
localization_priority: Priority
author: dkershaw10
ms.openlocfilehash: 854897e1cc4d887fc0f4d2f184a4e745e5cdc468
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462636"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="6627d-103">Тип ресурсов openTypeExtension (открытые расширения)</span><span class="sxs-lookup"><span data-stu-id="6627d-103">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="6627d-104">Открытые расширения (прежнее название — расширения данных Office 365) позволяют легко добавлять нетипизированные свойства непосредственно в ресурс в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6627d-104">Open extensions (formerly known as Office 365 data extensions) give you an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>

<span data-ttu-id="6627d-105">Открытые расширения представлены ресурсом **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="6627d-105">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="6627d-106">Все открытые расширения, добавленные в ресурс, отображаются в свойстве навигации **extensions**, которое является производным от абстрактного типа [extension](extension.md).</span><span class="sxs-lookup"><span data-stu-id="6627d-106">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span> <span data-ttu-id="6627d-107">Каждое расширение, помимо пользовательских данных, содержит свойство **extensionName** — единственное предопределенное записываемое свойство для всех расширений.</span><span class="sxs-lookup"><span data-stu-id="6627d-107">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span>

<span data-ttu-id="6627d-108">Чтобы обеспечить уникальность имен расширений, можно использовать формат обратных DNS, который зависит от _принадлежащего вам домена_, например `Com.Contoso.ContactInfo`.</span><span class="sxs-lookup"><span data-stu-id="6627d-108">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="6627d-109">Не указывайте домен Майкрософт (`Com.Microsoft` или `Com.OnMicrosoft`) в имени расширения.</span><span class="sxs-lookup"><span data-stu-id="6627d-109">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="6627d-110">Пример открытого расширения см. в статье [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users).</span><span class="sxs-lookup"><span data-stu-id="6627d-110">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="6627d-111">Открытые расширения поддерживаются указанными ниже ресурсами в соответствующих версиях — общедоступной (1.0 или бета-версии) или предварительной (бета-версии).</span><span class="sxs-lookup"><span data-stu-id="6627d-111">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

|<span data-ttu-id="6627d-112">Ресурс</span><span class="sxs-lookup"><span data-stu-id="6627d-112">Resource</span></span> |<span data-ttu-id="6627d-113">Версия</span><span class="sxs-lookup"><span data-stu-id="6627d-113">Version</span></span> |
|:---------------|:-------|
| [<span data-ttu-id="6627d-114">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="6627d-114">Administrative unit</span></span>](/graph/api/resources/administrativeunit?view=graph-rest-beta)  | <span data-ttu-id="6627d-115">Только предварительная версия</span><span class="sxs-lookup"><span data-stu-id="6627d-115">Preview only</span></span> |
| <span data-ttu-id="6627d-116">[event](event.md) для календаря</span><span class="sxs-lookup"><span data-stu-id="6627d-116">[Calendar event](event.md)</span></span> | <span data-ttu-id="6627d-117">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="6627d-117">GA</span></span> |
| <span data-ttu-id="6627d-118">[event](event.md) для календаря группы</span><span class="sxs-lookup"><span data-stu-id="6627d-118">Group [calendar event](event.md)</span></span> | <span data-ttu-id="6627d-119">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="6627d-119">GA</span></span> |
| <span data-ttu-id="6627d-120">[post](post.md) цепочки беседы группы</span><span class="sxs-lookup"><span data-stu-id="6627d-120">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="6627d-121">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="6627d-121">GA</span></span> |
| [<span data-ttu-id="6627d-122">device</span><span class="sxs-lookup"><span data-stu-id="6627d-122">device</span></span>](device.md) | <span data-ttu-id="6627d-123">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="6627d-123">GA</span></span> |
| [<span data-ttu-id="6627d-124">group</span><span class="sxs-lookup"><span data-stu-id="6627d-124">group</span></span>](group.md) | <span data-ttu-id="6627d-125">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="6627d-125">GA</span></span> |
| [<span data-ttu-id="6627d-126">message</span><span class="sxs-lookup"><span data-stu-id="6627d-126">message</span></span>](message.md) | <span data-ttu-id="6627d-127">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="6627d-127">GA</span></span> |
| [<span data-ttu-id="6627d-128">organization</span><span class="sxs-lookup"><span data-stu-id="6627d-128">organization</span></span>](organization.md) | <span data-ttu-id="6627d-129">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="6627d-129">GA</span></span> |
| <span data-ttu-id="6627d-130">[contact](contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="6627d-130">[Personal contact](contact.md)</span></span> | <span data-ttu-id="6627d-131">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="6627d-131">GA</span></span> |
| [<span data-ttu-id="6627d-132">user</span><span class="sxs-lookup"><span data-stu-id="6627d-132">user</span></span>](user.md) | <span data-ttu-id="6627d-133">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="6627d-133">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="6627d-134">Специальные рекомендации для Outlook</span><span class="sxs-lookup"><span data-stu-id="6627d-134">Outlook-specific considerations</span></span>

<span data-ttu-id="6627d-135">Каждое открытое расширение, присутствующее в ресурсе Outlook (событии, сообщении или личном контакте), хранится в [именованном свойстве MAPI](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span><span class="sxs-lookup"><span data-stu-id="6627d-135">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span></span> <span data-ttu-id="6627d-136">Создавая открытые расширения для Outlook, учитывайте, что именованные свойства MAPI в почтовом ящике пользователя — это ограниченный ресурс.</span><span class="sxs-lookup"><span data-stu-id="6627d-136">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="6627d-137">Когда будет достигнута квота именованных свойств пользователя, для этого пользователя невозможно будет создавать другие именованные свойства.</span><span class="sxs-lookup"><span data-stu-id="6627d-137">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="6627d-138">Это может привести к неожиданным действиям пользователей, для работы которых необходимы именованные свойства.</span><span class="sxs-lookup"><span data-stu-id="6627d-138">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="6627d-139">Руководствуйтесь приведенными ниже рекомендациями при создании открытых расширений в ресурсах Outlook.</span><span class="sxs-lookup"><span data-stu-id="6627d-139">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="6627d-140">Создайте минимум необходимых расширений.</span><span class="sxs-lookup"><span data-stu-id="6627d-140">Create the minimum number of extensions required.</span></span> <span data-ttu-id="6627d-141">Большинству приложений должно потребоваться не более одного расширения.</span><span class="sxs-lookup"><span data-stu-id="6627d-141">Most applications should require no more than one extension.</span></span> <span data-ttu-id="6627d-142">У расширений нет определенных свойств или структуры, поэтому в одном расширении можно хранить несколько значений.</span><span class="sxs-lookup"><span data-stu-id="6627d-142">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="6627d-143">Избегайте несогласованного именования расширений (например, на основании вводимых пользователями данных и т. д.).</span><span class="sxs-lookup"><span data-stu-id="6627d-143">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="6627d-144">При создании открытого расширения с новым именем, которое ранее не использовалось в почтовом ящике пользователя, всегда создается новое именованное свойство MAPI.</span><span class="sxs-lookup"><span data-stu-id="6627d-144">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="6627d-145">При удалении расширения именованное свойство не удаляется.</span><span class="sxs-lookup"><span data-stu-id="6627d-145">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="6627d-146">Использование открытых расширений (для ресурсов Outlook) или расширенных свойств</span><span class="sxs-lookup"><span data-stu-id="6627d-146">Use open extensions (for Outlook resources) or extended properties?</span></span>

<span data-ttu-id="6627d-147">Открытые расширения — рекомендуемое решение для большинства сценариев, предполагающих хранение пользовательских данных и доступ к ним.</span><span class="sxs-lookup"><span data-stu-id="6627d-147">Data extensions is the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="6627d-148">Если вам нужно получить доступ к пользовательским данным для свойств MAPI Outlook, которые еще не предоставлены при помощи [метаданных API Microsoft Graph](https://developer.microsoft.com/graph/docs/overview/call_api), используйте [расширенные свойства и соответствующий REST API](extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="6627d-148">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="6627d-149">Вы можете проверить, какие свойства предоставляются с помощью метаданных, на странице [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span><span class="sxs-lookup"><span data-stu-id="6627d-149">You can verify which properties the metadata exposes at https://graph.microsoft.com/v1.0/$metadata.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6627d-150">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6627d-150">JSON representation</span></span>

<span data-ttu-id="6627d-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6627d-151">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="6627d-152">Свойства</span><span class="sxs-lookup"><span data-stu-id="6627d-152">Properties</span></span>

|<span data-ttu-id="6627d-153">Свойство</span><span class="sxs-lookup"><span data-stu-id="6627d-153">Property</span></span> | <span data-ttu-id="6627d-154">Тип</span><span class="sxs-lookup"><span data-stu-id="6627d-154">Type</span></span> | <span data-ttu-id="6627d-155">Описание</span><span class="sxs-lookup"><span data-stu-id="6627d-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6627d-156">extensionName</span><span class="sxs-lookup"><span data-stu-id="6627d-156">extensionName</span></span>|<span data-ttu-id="6627d-157">String</span><span class="sxs-lookup"><span data-stu-id="6627d-157">String</span></span>|<span data-ttu-id="6627d-p107">Уникальный текстовый идентификатор для открытых расширений открытого типа. Обязательно свойство.</span><span class="sxs-lookup"><span data-stu-id="6627d-p107">A unique text identifier for an open type open extension. Required.</span></span>|
|<span data-ttu-id="6627d-160">id</span><span class="sxs-lookup"><span data-stu-id="6627d-160">id</span></span>|<span data-ttu-id="6627d-161">String</span><span class="sxs-lookup"><span data-stu-id="6627d-161">String</span></span>| <span data-ttu-id="6627d-p108">Полный идентификатор, в котором сцеплены тип расширения и свойство **extensionName**. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6627d-p108">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6627d-164">Связи</span><span class="sxs-lookup"><span data-stu-id="6627d-164">Relationships</span></span>

<span data-ttu-id="6627d-165">Нет</span><span class="sxs-lookup"><span data-stu-id="6627d-165">None</span></span>

## <a name="methods"></a><span data-ttu-id="6627d-166">Методы</span><span class="sxs-lookup"><span data-stu-id="6627d-166">Methods</span></span>

|<span data-ttu-id="6627d-167">Метод</span><span class="sxs-lookup"><span data-stu-id="6627d-167">Method</span></span> | <span data-ttu-id="6627d-168">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6627d-168">Return Type</span></span> | <span data-ttu-id="6627d-169">Описание</span><span class="sxs-lookup"><span data-stu-id="6627d-169">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="6627d-170">Post</span><span class="sxs-lookup"><span data-stu-id="6627d-170">Post</span></span>](../api/opentypeextension-post-opentypeextension.md) | <span data-ttu-id="6627d-171">Объект [openTypeExtension](opentypeextension.md) (в существующем экземпляре ресурса) либо новый ресурс [contact](../resources/contact.md), [event](../resources/event.md) или [message](../resources/message.md), содержащий объект openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="6627d-171">[openTypeExtension](opentypeextension.md) (in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object</span></span> | <span data-ttu-id="6627d-172">Создание объекта openTypeExtension в существующем или новом экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="6627d-172">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="6627d-173">Get</span><span class="sxs-lookup"><span data-stu-id="6627d-173">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="6627d-174">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="6627d-174">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="6627d-175">Чтение свойств и связей объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="6627d-175">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="6627d-176">Update</span><span class="sxs-lookup"><span data-stu-id="6627d-176">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="6627d-177">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="6627d-177">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="6627d-178">Обновление объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="6627d-178">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="6627d-179">Delete</span><span class="sxs-lookup"><span data-stu-id="6627d-179">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="6627d-180">Нет</span><span class="sxs-lookup"><span data-stu-id="6627d-180">None</span></span> |<span data-ttu-id="6627d-181">Удаление объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="6627d-181">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
