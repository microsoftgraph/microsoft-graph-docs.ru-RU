---
title: Тип ресурсов openTypeExtension (открытые расширения)
description: Открыть extensions (ранее называлась расширения данные Office 365) предоставляют простой способ добавлять нетипизированный свойства непосредственно к ресурсам в Microsoft Graph.
localization_priority: Normal
ms.openlocfilehash: 4bab83766d1fc44e96043689677713cb59084f4f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870961"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="876be-103">Тип ресурсов openTypeExtension (открытые расширения)</span><span class="sxs-lookup"><span data-stu-id="876be-103">openTypeExtension resource type (open extensions)</span></span>

> <span data-ttu-id="876be-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="876be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="876be-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="876be-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="876be-106">Открыть extensions (ранее называлась расширения данные Office 365) предоставляют простой способ добавлять нетипизированный свойства непосредственно к ресурсам в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="876be-106">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>
<span data-ttu-id="876be-107">Открытые расширения представлены ресурсом **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="876be-107">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="876be-108">Все открытые расширения, добавленные в ресурс, отображаются в свойстве навигации **extensions**, которое является производным от абстрактного типа [extension](extension.md).</span><span class="sxs-lookup"><span data-stu-id="876be-108">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span>  <span data-ttu-id="876be-109">Каждое расширение, помимо пользовательских данных, содержит свойство **extensionName** — единственное предопределенное записываемое свойство для всех расширений.</span><span class="sxs-lookup"><span data-stu-id="876be-109">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span> <span data-ttu-id="876be-110">Чтобы обеспечить уникальность имен расширений, можно использовать формат обратных DNS, который зависит от _принадлежащего вам домена_, например `Com.Contoso.ContactInfo`.</span><span class="sxs-lookup"><span data-stu-id="876be-110">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="876be-111">Не указывайте домен Майкрософт (`Com.Microsoft` или `Com.OnMicrosoft`) в имени расширения.</span><span class="sxs-lookup"><span data-stu-id="876be-111">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="876be-112">Пример открытого расширения. [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users).</span><span class="sxs-lookup"><span data-stu-id="876be-112">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="876be-113">Открытые расширения поддерживаются указанными ниже ресурсами в соответствующих версиях — общедоступной (1.0 или бета-версии) или предварительной (бета-версии).</span><span class="sxs-lookup"><span data-stu-id="876be-113">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

| <span data-ttu-id="876be-114">Ресурс</span><span class="sxs-lookup"><span data-stu-id="876be-114">Resource</span></span> | <span data-ttu-id="876be-115">Версия</span><span class="sxs-lookup"><span data-stu-id="876be-115">Version</span></span> |
|---------------|-------|
| [<span data-ttu-id="876be-116">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="876be-116">Administrative unit</span></span>](administrativeunit.md)  | <span data-ttu-id="876be-117">Только предварительная версия</span><span class="sxs-lookup"><span data-stu-id="876be-117">Preview only</span></span> |
| <span data-ttu-id="876be-118">[event](event.md) для календаря</span><span class="sxs-lookup"><span data-stu-id="876be-118">[Calendar event](event.md)</span></span> | <span data-ttu-id="876be-119">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="876be-119">GA</span></span> |
| <span data-ttu-id="876be-120">[event](event.md) для календаря группы</span><span class="sxs-lookup"><span data-stu-id="876be-120">Group [calendar event](event.md)</span></span> | <span data-ttu-id="876be-121">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="876be-121">GA</span></span> |
| <span data-ttu-id="876be-122">[post](post.md) цепочки беседы группы</span><span class="sxs-lookup"><span data-stu-id="876be-122">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="876be-123">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="876be-123">GA</span></span> |
| [<span data-ttu-id="876be-124">device</span><span class="sxs-lookup"><span data-stu-id="876be-124">device</span></span>](device.md) | <span data-ttu-id="876be-125">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="876be-125">GA</span></span> |
| [<span data-ttu-id="876be-126">group</span><span class="sxs-lookup"><span data-stu-id="876be-126">group</span></span>](group.md) | <span data-ttu-id="876be-127">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="876be-127">GA</span></span> |
| [<span data-ttu-id="876be-128">message</span><span class="sxs-lookup"><span data-stu-id="876be-128">message</span></span>](message.md) | <span data-ttu-id="876be-129">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="876be-129">GA</span></span> |
| [<span data-ttu-id="876be-130">organization</span><span class="sxs-lookup"><span data-stu-id="876be-130">organization</span></span>](organization.md) | <span data-ttu-id="876be-131">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="876be-131">GA</span></span> |
| <span data-ttu-id="876be-132">[contact](contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="876be-132">[Personal contact](contact.md)</span></span> | <span data-ttu-id="876be-133">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="876be-133">GA</span></span> |
| [<span data-ttu-id="876be-134">user</span><span class="sxs-lookup"><span data-stu-id="876be-134">user</span></span>](user.md) | <span data-ttu-id="876be-135">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="876be-135">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="876be-136">Вопросы, относящиеся к Outlook</span><span class="sxs-lookup"><span data-stu-id="876be-136">Outlook-specific considerations</span></span>

<span data-ttu-id="876be-137">Каждое open расширение на ресурс Outlook (событий, сообщение или личный контакт) хранятся в [MAPI именованное свойство](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span><span class="sxs-lookup"><span data-stu-id="876be-137">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span></span> <span data-ttu-id="876be-138">При создании open расширений для Outlook необходимо учитывайте, что именованные свойства MAPI, ограничение ресурсов в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="876be-138">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="876be-139">Когда закончится квоту именованное свойство невозможно создать более именованные свойства для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="876be-139">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="876be-140">Это может привести к непредсказуемым последствиям от клиентов, зависящие от именованных свойств функции.</span><span class="sxs-lookup"><span data-stu-id="876be-140">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="876be-141">При создании open расширений ресурсов Outlook применяются следующие рекомендации:</span><span class="sxs-lookup"><span data-stu-id="876be-141">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="876be-142">Создайте минимальное число необходимых расширений.</span><span class="sxs-lookup"><span data-stu-id="876be-142">Create the minimum number of extensions required.</span></span> <span data-ttu-id="876be-143">Большинство приложений требуется не более одного расширения.</span><span class="sxs-lookup"><span data-stu-id="876be-143">Most applications should require no more than one extension.</span></span> <span data-ttu-id="876be-144">Расширения не имеют определенный набор свойств или структуры, чтобы можно было хранить несколько значений в одном расширении.</span><span class="sxs-lookup"><span data-stu-id="876be-144">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="876be-145">Избегайте именования расширений в виде переменной (например, на основе введенных данных, и т.д.).</span><span class="sxs-lookup"><span data-stu-id="876be-145">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="876be-146">Каждый раз, когда open расширение создается новое имя, которое не использовалась в почтовом ящике пользователя перед, будет создан новый MAPI именованное свойство.</span><span class="sxs-lookup"><span data-stu-id="876be-146">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="876be-147">Удаление расширения не удаляет именованное свойство.</span><span class="sxs-lookup"><span data-stu-id="876be-147">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="876be-148">Использование открытия расширения (для ресурсов Outlook) или расширенные свойства</span><span class="sxs-lookup"><span data-stu-id="876be-148">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="876be-149">Открыть расширения — это рекомендуемое решение для большинства сценариев с помощью хранение и доступ к пользовательских данных.</span><span class="sxs-lookup"><span data-stu-id="876be-149">Open extensions is the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="876be-150">Если требуется доступ к пользовательские данные для свойства Outlook MAPI, которые еще не предоставляется через [Microsoft Graph API метаданных](https://developer.microsoft.com/graph/docs/overview/call_api), можно использовать [Расширенные свойства и его API -Интерфейс REST](extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="876be-150">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="876be-151">Вы можете проверить свойств, которые предоставляет метаданные во [ https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span><span class="sxs-lookup"><span data-stu-id="876be-151">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="876be-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="876be-152">JSON representation</span></span>

<span data-ttu-id="876be-153">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="876be-153">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.opentypeextension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```

## <a name="properties"></a><span data-ttu-id="876be-154">Свойства</span><span class="sxs-lookup"><span data-stu-id="876be-154">Properties</span></span>

| <span data-ttu-id="876be-155">Свойство</span><span class="sxs-lookup"><span data-stu-id="876be-155">Property</span></span> | <span data-ttu-id="876be-156">Тип</span><span class="sxs-lookup"><span data-stu-id="876be-156">Type</span></span> | <span data-ttu-id="876be-157">Описание</span><span class="sxs-lookup"><span data-stu-id="876be-157">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="876be-158">extensionName</span><span class="sxs-lookup"><span data-stu-id="876be-158">extensionName</span></span>|<span data-ttu-id="876be-159">Строка</span><span class="sxs-lookup"><span data-stu-id="876be-159">String</span></span>|<span data-ttu-id="876be-p107">Уникальный текстовый идентификатор для модуля обработки данных открытого типа. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="876be-p107">A unique text identifier for an open type data extension. Required.</span></span>|
|<span data-ttu-id="876be-162">id</span><span class="sxs-lookup"><span data-stu-id="876be-162">id</span></span>|<span data-ttu-id="876be-163">Строка</span><span class="sxs-lookup"><span data-stu-id="876be-163">String</span></span>| <span data-ttu-id="876be-p108">Полный идентификатор, в котором сцеплены тип расширения и свойство **extensionName**. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="876be-p108">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="876be-166">Связи</span><span class="sxs-lookup"><span data-stu-id="876be-166">Relationships</span></span>

<span data-ttu-id="876be-167">Нет</span><span class="sxs-lookup"><span data-stu-id="876be-167">None</span></span>

## <a name="methods"></a><span data-ttu-id="876be-168">Методы</span><span class="sxs-lookup"><span data-stu-id="876be-168">Methods</span></span>

| <span data-ttu-id="876be-169">Метод</span><span class="sxs-lookup"><span data-stu-id="876be-169">Method</span></span> | <span data-ttu-id="876be-170">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="876be-170">Return Type</span></span> | <span data-ttu-id="876be-171">Описание</span><span class="sxs-lookup"><span data-stu-id="876be-171">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="876be-172">Post</span><span class="sxs-lookup"><span data-stu-id="876be-172">Post</span></span>](../api/opentypeextension-post-opentypeextension.md) | <span data-ttu-id="876be-173">[openTypeExtension](opentypeextension.md) (в существующий ресурсов экземпляр) или создать [контактов](../resources/contact.md), [события](../resources/event.md)или [сообщение](../resources/message.md) , содержащее объект openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="876be-173">[openTypeExtension](opentypeextension.md)(in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object.</span></span> | <span data-ttu-id="876be-174">Создание объекта openTypeExtension в существующем или новом экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="876be-174">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="876be-175">Get</span><span class="sxs-lookup"><span data-stu-id="876be-175">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="876be-176">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="876be-176">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="876be-177">Чтение свойств и связей объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="876be-177">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="876be-178">Update</span><span class="sxs-lookup"><span data-stu-id="876be-178">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="876be-179">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="876be-179">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="876be-180">Обновление объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="876be-180">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="876be-181">Delete</span><span class="sxs-lookup"><span data-stu-id="876be-181">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="876be-182">Нет</span><span class="sxs-lookup"><span data-stu-id="876be-182">None</span></span> |<span data-ttu-id="876be-183">Удаление объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="876be-183">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
