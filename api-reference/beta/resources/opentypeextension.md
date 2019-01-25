---
title: Тип ресурсов openTypeExtension (открытые расширения)
description: Открыть extensions (ранее называлась расширения данные Office 365) предоставляют простой способ добавлять нетипизированный свойства непосредственно к ресурсам в Microsoft Graph.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: ba5dbcd6c5ae1705ffe7e89ca6f529280d98adf5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508834"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="68243-103">Тип ресурсов openTypeExtension (открытые расширения)</span><span class="sxs-lookup"><span data-stu-id="68243-103">openTypeExtension resource type (open extensions)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68243-104">Открыть extensions (ранее называлась расширения данные Office 365) предоставляют простой способ добавлять нетипизированный свойства непосредственно к ресурсам в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="68243-104">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>
<span data-ttu-id="68243-105">Открытые расширения представлены ресурсом **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="68243-105">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="68243-106">Все открытые расширения, добавленные в ресурс, отображаются в свойстве навигации **extensions**, которое является производным от абстрактного типа [extension](extension.md).</span><span class="sxs-lookup"><span data-stu-id="68243-106">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span>  <span data-ttu-id="68243-107">Каждое расширение, помимо пользовательских данных, содержит свойство **extensionName** — единственное предопределенное записываемое свойство для всех расширений.</span><span class="sxs-lookup"><span data-stu-id="68243-107">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span> <span data-ttu-id="68243-108">Чтобы обеспечить уникальность имен расширений, можно использовать формат обратных DNS, который зависит от _принадлежащего вам домена_, например `Com.Contoso.ContactInfo`.</span><span class="sxs-lookup"><span data-stu-id="68243-108">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="68243-109">Не указывайте домен Майкрософт (`Com.Microsoft` или `Com.OnMicrosoft`) в имени расширения.</span><span class="sxs-lookup"><span data-stu-id="68243-109">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="68243-110">Пример открытого расширения. [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users).</span><span class="sxs-lookup"><span data-stu-id="68243-110">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="68243-111">Открытые расширения поддерживаются указанными ниже ресурсами в соответствующих версиях — общедоступной (1.0 или бета-версии) или предварительной (бета-версии).</span><span class="sxs-lookup"><span data-stu-id="68243-111">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

| <span data-ttu-id="68243-112">Ресурс</span><span class="sxs-lookup"><span data-stu-id="68243-112">Resource</span></span> | <span data-ttu-id="68243-113">Версия</span><span class="sxs-lookup"><span data-stu-id="68243-113">Version</span></span> |
|---------------|-------|
| [<span data-ttu-id="68243-114">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="68243-114">Administrative unit</span></span>](administrativeunit.md)  | <span data-ttu-id="68243-115">Только предварительная версия</span><span class="sxs-lookup"><span data-stu-id="68243-115">Preview only</span></span> |
| <span data-ttu-id="68243-116">[event](event.md) для календаря</span><span class="sxs-lookup"><span data-stu-id="68243-116">[Calendar event](event.md)</span></span> | <span data-ttu-id="68243-117">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="68243-117">GA</span></span> |
| <span data-ttu-id="68243-118">[event](event.md) для календаря группы</span><span class="sxs-lookup"><span data-stu-id="68243-118">Group [calendar event](event.md)</span></span> | <span data-ttu-id="68243-119">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="68243-119">GA</span></span> |
| <span data-ttu-id="68243-120">[post](post.md) цепочки беседы группы</span><span class="sxs-lookup"><span data-stu-id="68243-120">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="68243-121">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="68243-121">GA</span></span> |
| [<span data-ttu-id="68243-122">device</span><span class="sxs-lookup"><span data-stu-id="68243-122">device</span></span>](device.md) | <span data-ttu-id="68243-123">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="68243-123">GA</span></span> |
| [<span data-ttu-id="68243-124">group</span><span class="sxs-lookup"><span data-stu-id="68243-124">group</span></span>](group.md) | <span data-ttu-id="68243-125">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="68243-125">GA</span></span> |
| [<span data-ttu-id="68243-126">message</span><span class="sxs-lookup"><span data-stu-id="68243-126">message</span></span>](message.md) | <span data-ttu-id="68243-127">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="68243-127">GA</span></span> |
| [<span data-ttu-id="68243-128">organization</span><span class="sxs-lookup"><span data-stu-id="68243-128">organization</span></span>](organization.md) | <span data-ttu-id="68243-129">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="68243-129">GA</span></span> |
| <span data-ttu-id="68243-130">[contact](contact.md) (личный контакт)</span><span class="sxs-lookup"><span data-stu-id="68243-130">[Personal contact](contact.md)</span></span> | <span data-ttu-id="68243-131">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="68243-131">GA</span></span> |
| [<span data-ttu-id="68243-132">user</span><span class="sxs-lookup"><span data-stu-id="68243-132">user</span></span>](user.md) | <span data-ttu-id="68243-133">Общедоступная версия</span><span class="sxs-lookup"><span data-stu-id="68243-133">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="68243-134">Вопросы, относящиеся к Outlook</span><span class="sxs-lookup"><span data-stu-id="68243-134">Outlook-specific considerations</span></span>

<span data-ttu-id="68243-135">Каждое open расширение на ресурс Outlook (событий, сообщение или личный контакт) хранятся в [MAPI именованное свойство](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span><span class="sxs-lookup"><span data-stu-id="68243-135">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span></span> <span data-ttu-id="68243-136">При создании open расширений для Outlook необходимо учитывайте, что именованные свойства MAPI, ограничение ресурсов в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="68243-136">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="68243-137">Когда закончится квоту именованное свойство невозможно создать более именованные свойства для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="68243-137">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="68243-138">Это может привести к непредсказуемым последствиям от клиентов, зависящие от именованных свойств функции.</span><span class="sxs-lookup"><span data-stu-id="68243-138">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="68243-139">При создании open расширений ресурсов Outlook применяются следующие рекомендации:</span><span class="sxs-lookup"><span data-stu-id="68243-139">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="68243-140">Создайте минимальное число необходимых расширений.</span><span class="sxs-lookup"><span data-stu-id="68243-140">Create the minimum number of extensions required.</span></span> <span data-ttu-id="68243-141">Большинство приложений требуется не более одного расширения.</span><span class="sxs-lookup"><span data-stu-id="68243-141">Most applications should require no more than one extension.</span></span> <span data-ttu-id="68243-142">Расширения не имеют определенный набор свойств или структуры, чтобы можно было хранить несколько значений в одном расширении.</span><span class="sxs-lookup"><span data-stu-id="68243-142">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="68243-143">Избегайте именования расширений в виде переменной (например, на основе введенных данных, и т.д.).</span><span class="sxs-lookup"><span data-stu-id="68243-143">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="68243-144">Каждый раз, когда open расширение создается новое имя, которое не использовалась в почтовом ящике пользователя перед, будет создан новый MAPI именованное свойство.</span><span class="sxs-lookup"><span data-stu-id="68243-144">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="68243-145">Удаление расширения не удаляет именованное свойство.</span><span class="sxs-lookup"><span data-stu-id="68243-145">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="68243-146">Что использовать — открытые расширения (для ресурсов Outlook) или расширенные свойства</span><span class="sxs-lookup"><span data-stu-id="68243-146">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="68243-147">Открыть расширения — это рекомендуемое решение для большинства сценариев с помощью хранение и доступ к пользовательских данных.</span><span class="sxs-lookup"><span data-stu-id="68243-147">Open extensions is the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="68243-148">Если требуется доступ к пользовательские данные для свойства Outlook MAPI, которые еще не предоставляется через [Microsoft Graph API метаданных](https://developer.microsoft.com/graph/docs/overview/call_api), можно использовать [Расширенные свойства и его API -Интерфейс REST](extended-properties-overview.md).</span><span class="sxs-lookup"><span data-stu-id="68243-148">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="68243-149">Вы можете проверить свойств, которые предоставляет метаданные во [ https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span><span class="sxs-lookup"><span data-stu-id="68243-149">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="68243-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="68243-150">JSON representation</span></span>

<span data-ttu-id="68243-151">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="68243-151">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="68243-152">Свойства</span><span class="sxs-lookup"><span data-stu-id="68243-152">Properties</span></span>

| <span data-ttu-id="68243-153">Свойство</span><span class="sxs-lookup"><span data-stu-id="68243-153">Property</span></span> | <span data-ttu-id="68243-154">Тип</span><span class="sxs-lookup"><span data-stu-id="68243-154">Type</span></span> | <span data-ttu-id="68243-155">Описание</span><span class="sxs-lookup"><span data-stu-id="68243-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="68243-156">extensionName</span><span class="sxs-lookup"><span data-stu-id="68243-156">extensionName</span></span>|<span data-ttu-id="68243-157">String</span><span class="sxs-lookup"><span data-stu-id="68243-157">String</span></span>|<span data-ttu-id="68243-p106">Уникальный текстовый идентификатор для модуля обработки данных открытого типа. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68243-p106">A unique text identifier for an open type data extension. Required.</span></span>|
|<span data-ttu-id="68243-160">id</span><span class="sxs-lookup"><span data-stu-id="68243-160">id</span></span>|<span data-ttu-id="68243-161">String</span><span class="sxs-lookup"><span data-stu-id="68243-161">String</span></span>| <span data-ttu-id="68243-p107">Полный идентификатор, в котором сцеплены тип расширения и свойство **extensionName**. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="68243-p107">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68243-164">Отношения</span><span class="sxs-lookup"><span data-stu-id="68243-164">Relationships</span></span>

<span data-ttu-id="68243-165">Нет</span><span class="sxs-lookup"><span data-stu-id="68243-165">None</span></span>

## <a name="methods"></a><span data-ttu-id="68243-166">Методы</span><span class="sxs-lookup"><span data-stu-id="68243-166">Methods</span></span>

| <span data-ttu-id="68243-167">Метод</span><span class="sxs-lookup"><span data-stu-id="68243-167">Method</span></span> | <span data-ttu-id="68243-168">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="68243-168">Return Type</span></span> | <span data-ttu-id="68243-169">Описание</span><span class="sxs-lookup"><span data-stu-id="68243-169">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="68243-170">Post</span><span class="sxs-lookup"><span data-stu-id="68243-170">Post</span></span>](../api/opentypeextension-post-opentypeextension.md) | <span data-ttu-id="68243-171">[openTypeExtension](opentypeextension.md) (в существующий ресурсов экземпляр) или создать [контактов](../resources/contact.md), [события](../resources/event.md)или [сообщение](../resources/message.md) , содержащее объект openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="68243-171">[openTypeExtension](opentypeextension.md)(in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object.</span></span> | <span data-ttu-id="68243-172">Создание объекта openTypeExtension в существующем или новом экземпляре ресурса.</span><span class="sxs-lookup"><span data-stu-id="68243-172">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="68243-173">Get</span><span class="sxs-lookup"><span data-stu-id="68243-173">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="68243-174">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="68243-174">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="68243-175">Чтение свойств и связей объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="68243-175">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="68243-176">Update</span><span class="sxs-lookup"><span data-stu-id="68243-176">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="68243-177">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="68243-177">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="68243-178">Обновление объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="68243-178">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="68243-179">Delete</span><span class="sxs-lookup"><span data-stu-id="68243-179">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="68243-180">Нет</span><span class="sxs-lookup"><span data-stu-id="68243-180">None</span></span> |<span data-ttu-id="68243-181">Удаление объекта openTypeExtension.</span><span class="sxs-lookup"><span data-stu-id="68243-181">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/opentypeextension.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
