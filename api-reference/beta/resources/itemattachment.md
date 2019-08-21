---
title: Тип ресурса itemAttachment
description: Контакт, событие или сообщение, присоединенное к другому событию,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: b4220a1428edab2eeab89cabe53efc91bea76a8b
ms.sourcegitcommit: 496269b62d42cb7a96752a77b0f2e0cb16918f0b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2019
ms.locfileid: "36484382"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="640b8-103">Тип ресурса itemAttachment</span><span class="sxs-lookup"><span data-stu-id="640b8-103">itemAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="640b8-104">Контакт, событие или сообщение, присоединенное к другому событию [](../resources/event.md), [сообщению](../resources/message.md), [задаче Outlook](../resources/outlooktask.md)или [POST](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="640b8-104">A contact, event, or message that's attached to another [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="640b8-105">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="640b8-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="640b8-106">Методы</span><span class="sxs-lookup"><span data-stu-id="640b8-106">Methods</span></span>

| <span data-ttu-id="640b8-107">Метод</span><span class="sxs-lookup"><span data-stu-id="640b8-107">Method</span></span>       | <span data-ttu-id="640b8-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="640b8-108">Return Type</span></span>  |<span data-ttu-id="640b8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="640b8-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="640b8-110">Получение</span><span class="sxs-lookup"><span data-stu-id="640b8-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="640b8-111">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="640b8-111">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="640b8-112">Чтение свойств и связей объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="640b8-112">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="640b8-113">Удаление</span><span class="sxs-lookup"><span data-stu-id="640b8-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="640b8-114">Нет</span><span class="sxs-lookup"><span data-stu-id="640b8-114">None</span></span> |<span data-ttu-id="640b8-115">Удаление объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="640b8-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="640b8-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="640b8-116">Properties</span></span>
| <span data-ttu-id="640b8-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="640b8-117">Property</span></span>     | <span data-ttu-id="640b8-118">Тип</span><span class="sxs-lookup"><span data-stu-id="640b8-118">Type</span></span>   |<span data-ttu-id="640b8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="640b8-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="640b8-120">contentType</span><span class="sxs-lookup"><span data-stu-id="640b8-120">contentType</span></span>|<span data-ttu-id="640b8-121">String</span><span class="sxs-lookup"><span data-stu-id="640b8-121">String</span></span>|<span data-ttu-id="640b8-122">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="640b8-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="640b8-123">id</span><span class="sxs-lookup"><span data-stu-id="640b8-123">id</span></span>|<span data-ttu-id="640b8-124">String</span><span class="sxs-lookup"><span data-stu-id="640b8-124">String</span></span>| <span data-ttu-id="640b8-125">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="640b8-125">The attachment ID.</span></span>|
|<span data-ttu-id="640b8-126">isInline</span><span class="sxs-lookup"><span data-stu-id="640b8-126">isInline</span></span>|<span data-ttu-id="640b8-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="640b8-127">Boolean</span></span>|<span data-ttu-id="640b8-128">Значение true указывает, что вложение является встроенным, например внедренным изображением в теле элемента.</span><span class="sxs-lookup"><span data-stu-id="640b8-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="640b8-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="640b8-129">lastModifiedDateTime</span></span>|<span data-ttu-id="640b8-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="640b8-130">DateTimeOffset</span></span>|<span data-ttu-id="640b8-131">Время и дата последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="640b8-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="640b8-132">name</span><span class="sxs-lookup"><span data-stu-id="640b8-132">name</span></span>|<span data-ttu-id="640b8-133">String</span><span class="sxs-lookup"><span data-stu-id="640b8-133">String</span></span>|<span data-ttu-id="640b8-134">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="640b8-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="640b8-135">size</span><span class="sxs-lookup"><span data-stu-id="640b8-135">size</span></span>|<span data-ttu-id="640b8-136">Int32</span><span class="sxs-lookup"><span data-stu-id="640b8-136">Int32</span></span>|<span data-ttu-id="640b8-137">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="640b8-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="640b8-138">Связи</span><span class="sxs-lookup"><span data-stu-id="640b8-138">Relationships</span></span>
| <span data-ttu-id="640b8-139">Отношение</span><span class="sxs-lookup"><span data-stu-id="640b8-139">Relationship</span></span> | <span data-ttu-id="640b8-140">Тип</span><span class="sxs-lookup"><span data-stu-id="640b8-140">Type</span></span>   |<span data-ttu-id="640b8-141">Описание</span><span class="sxs-lookup"><span data-stu-id="640b8-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="640b8-142">item</span><span class="sxs-lookup"><span data-stu-id="640b8-142">item</span></span>|[<span data-ttu-id="640b8-143">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="640b8-143">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="640b8-144">Вложенный контакт, сообщение или событие.</span><span class="sxs-lookup"><span data-stu-id="640b8-144">The attached contact, message or event.</span></span> <span data-ttu-id="640b8-145">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="640b8-145">Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="640b8-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="640b8-146">JSON representation</span></span>

<span data-ttu-id="640b8-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="640b8-147">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
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
  "suppressions": []
}
-->
