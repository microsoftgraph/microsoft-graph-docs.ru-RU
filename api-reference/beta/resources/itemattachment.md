---
title: Тип ресурса itemAttachment
description: Контакт, события или сообщения, подключенный к другой событий
ms.openlocfilehash: fd8638a7d263c2ebbe09c77f717af989e1dd5a0e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080236"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="ece08-103">Тип ресурса itemAttachment</span><span class="sxs-lookup"><span data-stu-id="ece08-103">itemAttachment resource type</span></span>

> <span data-ttu-id="ece08-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ece08-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ece08-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ece08-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ece08-106">Контакт, события или сообщения, подключенный к другого [события](../resources/event.md), [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [публикации](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="ece08-106">A contact, event, or message that's attached to another [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="ece08-107">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="ece08-107">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ece08-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ece08-108">Methods</span></span>

| <span data-ttu-id="ece08-109">Метод</span><span class="sxs-lookup"><span data-stu-id="ece08-109">Method</span></span>       | <span data-ttu-id="ece08-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ece08-110">Return Type</span></span>  |<span data-ttu-id="ece08-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ece08-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ece08-112">Get</span><span class="sxs-lookup"><span data-stu-id="ece08-112">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="ece08-113">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="ece08-113">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="ece08-114">Чтение свойств и связей объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="ece08-114">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="ece08-115">Delete</span><span class="sxs-lookup"><span data-stu-id="ece08-115">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="ece08-116">Нет</span><span class="sxs-lookup"><span data-stu-id="ece08-116">None</span></span> |<span data-ttu-id="ece08-117">Удаление объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="ece08-117">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ece08-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="ece08-118">Properties</span></span>
| <span data-ttu-id="ece08-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="ece08-119">Property</span></span>     | <span data-ttu-id="ece08-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ece08-120">Type</span></span>   |<span data-ttu-id="ece08-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ece08-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ece08-122">contentType</span><span class="sxs-lookup"><span data-stu-id="ece08-122">contentType</span></span>|<span data-ttu-id="ece08-123">String</span><span class="sxs-lookup"><span data-stu-id="ece08-123">String</span></span>|<span data-ttu-id="ece08-124">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="ece08-124">The content type of the attachment.</span></span>|
|<span data-ttu-id="ece08-125">id</span><span class="sxs-lookup"><span data-stu-id="ece08-125">id</span></span>|<span data-ttu-id="ece08-126">String</span><span class="sxs-lookup"><span data-stu-id="ece08-126">String</span></span>| <span data-ttu-id="ece08-127">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="ece08-127">The attachment ID.</span></span>|
|<span data-ttu-id="ece08-128">isInline</span><span class="sxs-lookup"><span data-stu-id="ece08-128">isInline</span></span>|<span data-ttu-id="ece08-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="ece08-129">Boolean</span></span>|<span data-ttu-id="ece08-130">Значение true указывает, что вложение является встроенным, например внедренным изображением в теле элемента.</span><span class="sxs-lookup"><span data-stu-id="ece08-130">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="ece08-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ece08-131">lastModifiedDateTime</span></span>|<span data-ttu-id="ece08-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ece08-132">DateTimeOffset</span></span>|<span data-ttu-id="ece08-133">Время и дата последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="ece08-133">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="ece08-134">name</span><span class="sxs-lookup"><span data-stu-id="ece08-134">name</span></span>|<span data-ttu-id="ece08-135">String</span><span class="sxs-lookup"><span data-stu-id="ece08-135">String</span></span>|<span data-ttu-id="ece08-136">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="ece08-136">The display name of the attachment.</span></span>|
|<span data-ttu-id="ece08-137">size</span><span class="sxs-lookup"><span data-stu-id="ece08-137">size</span></span>|<span data-ttu-id="ece08-138">Int32</span><span class="sxs-lookup"><span data-stu-id="ece08-138">Int32</span></span>|<span data-ttu-id="ece08-139">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="ece08-139">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ece08-140">Связи</span><span class="sxs-lookup"><span data-stu-id="ece08-140">Relationships</span></span>
| <span data-ttu-id="ece08-141">Связь</span><span class="sxs-lookup"><span data-stu-id="ece08-141">Relationship</span></span> | <span data-ttu-id="ece08-142">Тип</span><span class="sxs-lookup"><span data-stu-id="ece08-142">Type</span></span>   |<span data-ttu-id="ece08-143">Описание</span><span class="sxs-lookup"><span data-stu-id="ece08-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ece08-144">item</span><span class="sxs-lookup"><span data-stu-id="ece08-144">item</span></span>|[<span data-ttu-id="ece08-145">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="ece08-145">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="ece08-146">Вложенные контакта, сообщение или события.</span><span class="sxs-lookup"><span data-stu-id="ece08-146">The attached contact, message or event.</span></span> <span data-ttu-id="ece08-147">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="ece08-147">Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ece08-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ece08-148">JSON representation</span></span>

<span data-ttu-id="ece08-149">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ece08-149">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
