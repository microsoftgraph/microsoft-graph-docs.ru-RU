---
title: Тип ресурса itemAttachment
description: Контакт, события или сообщения, подключенный к другой событий
localization_priority: Normal
ms.openlocfilehash: b0e3b62e5f6100884e6fbea40d16221bf8503897
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571410"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="c4c37-103">Тип ресурса itemAttachment</span><span class="sxs-lookup"><span data-stu-id="c4c37-103">itemAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4c37-104">Контакт, события или сообщения, подключенный к другого [события](../resources/event.md), [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [публикации](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="c4c37-104">A contact, event, or message that's attached to another [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="c4c37-105">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="c4c37-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c4c37-106">Методы</span><span class="sxs-lookup"><span data-stu-id="c4c37-106">Methods</span></span>

| <span data-ttu-id="c4c37-107">Метод</span><span class="sxs-lookup"><span data-stu-id="c4c37-107">Method</span></span>       | <span data-ttu-id="c4c37-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c4c37-108">Return Type</span></span>  |<span data-ttu-id="c4c37-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c4c37-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c4c37-110">Get</span><span class="sxs-lookup"><span data-stu-id="c4c37-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="c4c37-111">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="c4c37-111">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="c4c37-112">Чтение свойств и связей объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="c4c37-112">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="c4c37-113">Delete</span><span class="sxs-lookup"><span data-stu-id="c4c37-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="c4c37-114">Нет</span><span class="sxs-lookup"><span data-stu-id="c4c37-114">None</span></span> |<span data-ttu-id="c4c37-115">Удаление объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="c4c37-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c4c37-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4c37-116">Properties</span></span>
| <span data-ttu-id="c4c37-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4c37-117">Property</span></span>     | <span data-ttu-id="c4c37-118">Тип</span><span class="sxs-lookup"><span data-stu-id="c4c37-118">Type</span></span>   |<span data-ttu-id="c4c37-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c4c37-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4c37-120">contentType</span><span class="sxs-lookup"><span data-stu-id="c4c37-120">contentType</span></span>|<span data-ttu-id="c4c37-121">String</span><span class="sxs-lookup"><span data-stu-id="c4c37-121">String</span></span>|<span data-ttu-id="c4c37-122">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="c4c37-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="c4c37-123">id</span><span class="sxs-lookup"><span data-stu-id="c4c37-123">id</span></span>|<span data-ttu-id="c4c37-124">String</span><span class="sxs-lookup"><span data-stu-id="c4c37-124">String</span></span>| <span data-ttu-id="c4c37-125">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="c4c37-125">The attachment ID.</span></span>|
|<span data-ttu-id="c4c37-126">isInline</span><span class="sxs-lookup"><span data-stu-id="c4c37-126">isInline</span></span>|<span data-ttu-id="c4c37-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4c37-127">Boolean</span></span>|<span data-ttu-id="c4c37-128">Значение true указывает, что вложение является встроенным, например внедренным изображением в теле элемента.</span><span class="sxs-lookup"><span data-stu-id="c4c37-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="c4c37-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4c37-129">lastModifiedDateTime</span></span>|<span data-ttu-id="c4c37-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4c37-130">DateTimeOffset</span></span>|<span data-ttu-id="c4c37-131">Время и дата последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="c4c37-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="c4c37-132">name</span><span class="sxs-lookup"><span data-stu-id="c4c37-132">name</span></span>|<span data-ttu-id="c4c37-133">String</span><span class="sxs-lookup"><span data-stu-id="c4c37-133">String</span></span>|<span data-ttu-id="c4c37-134">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="c4c37-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="c4c37-135">size</span><span class="sxs-lookup"><span data-stu-id="c4c37-135">size</span></span>|<span data-ttu-id="c4c37-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c4c37-136">Int32</span></span>|<span data-ttu-id="c4c37-137">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="c4c37-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4c37-138">Связи</span><span class="sxs-lookup"><span data-stu-id="c4c37-138">Relationships</span></span>
| <span data-ttu-id="c4c37-139">Связь</span><span class="sxs-lookup"><span data-stu-id="c4c37-139">Relationship</span></span> | <span data-ttu-id="c4c37-140">Тип</span><span class="sxs-lookup"><span data-stu-id="c4c37-140">Type</span></span>   |<span data-ttu-id="c4c37-141">Описание</span><span class="sxs-lookup"><span data-stu-id="c4c37-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4c37-142">item</span><span class="sxs-lookup"><span data-stu-id="c4c37-142">item</span></span>|[<span data-ttu-id="c4c37-143">outlookItem</span><span class="sxs-lookup"><span data-stu-id="c4c37-143">outlookItem</span></span>](outlookitem.md)|<span data-ttu-id="c4c37-144">Вложенные контакта, сообщение или события.</span><span class="sxs-lookup"><span data-stu-id="c4c37-144">The attached contact, message or event.</span></span> <span data-ttu-id="c4c37-145">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="c4c37-145">Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4c37-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4c37-146">JSON representation</span></span>

<span data-ttu-id="c4c37-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4c37-147">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "@odata.type": "microsoft.graph.itemAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/itemattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
