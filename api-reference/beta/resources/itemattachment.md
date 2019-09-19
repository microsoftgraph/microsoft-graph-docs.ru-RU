---
title: Тип ресурса itemAttachment
description: Контакт, событие или сообщение, присоединенное к другому событию,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 166cd8eb5d6add0d96705ae59f38819c64b1465b
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036300"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="ec7a0-103">Тип ресурса itemAttachment</span><span class="sxs-lookup"><span data-stu-id="ec7a0-103">itemAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec7a0-104">Контакт, событие или сообщение, прикрепленное к [событию](../resources/event.md)пользователя, [сообщению](../resources/message.md), [задаче Outlook](../resources/outlooktask.md)или [POST](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="ec7a0-104">A contact, event, or message that's attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="ec7a0-105">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="ec7a0-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ec7a0-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ec7a0-106">Methods</span></span>

| <span data-ttu-id="ec7a0-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ec7a0-107">Method</span></span>       | <span data-ttu-id="ec7a0-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ec7a0-108">Return Type</span></span>  |<span data-ttu-id="ec7a0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ec7a0-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ec7a0-110">Получение</span><span class="sxs-lookup"><span data-stu-id="ec7a0-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="ec7a0-111">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="ec7a0-111">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="ec7a0-112">Чтение свойств, связей или необработанного содержимого объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="ec7a0-112">Read the properties, relationships, or raw contents of an itemAttachment object.</span></span>|
|[<span data-ttu-id="ec7a0-113">Удаление</span><span class="sxs-lookup"><span data-stu-id="ec7a0-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="ec7a0-114">Нет</span><span class="sxs-lookup"><span data-stu-id="ec7a0-114">None</span></span> |<span data-ttu-id="ec7a0-115">Удаление объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="ec7a0-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ec7a0-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec7a0-116">Properties</span></span>
| <span data-ttu-id="ec7a0-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec7a0-117">Property</span></span>     | <span data-ttu-id="ec7a0-118">Тип</span><span class="sxs-lookup"><span data-stu-id="ec7a0-118">Type</span></span>   |<span data-ttu-id="ec7a0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ec7a0-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec7a0-120">contentType</span><span class="sxs-lookup"><span data-stu-id="ec7a0-120">contentType</span></span>|<span data-ttu-id="ec7a0-121">String</span><span class="sxs-lookup"><span data-stu-id="ec7a0-121">String</span></span>|<span data-ttu-id="ec7a0-122">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="ec7a0-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="ec7a0-123">id</span><span class="sxs-lookup"><span data-stu-id="ec7a0-123">id</span></span>|<span data-ttu-id="ec7a0-124">String</span><span class="sxs-lookup"><span data-stu-id="ec7a0-124">String</span></span>| <span data-ttu-id="ec7a0-125">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="ec7a0-125">The attachment ID.</span></span>|
|<span data-ttu-id="ec7a0-126">isInline</span><span class="sxs-lookup"><span data-stu-id="ec7a0-126">isInline</span></span>|<span data-ttu-id="ec7a0-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec7a0-127">Boolean</span></span>|<span data-ttu-id="ec7a0-128">Значение true указывает, что вложение является встроенным, например внедренным изображением в теле элемента.</span><span class="sxs-lookup"><span data-stu-id="ec7a0-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="ec7a0-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec7a0-129">lastModifiedDateTime</span></span>|<span data-ttu-id="ec7a0-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec7a0-130">DateTimeOffset</span></span>|<span data-ttu-id="ec7a0-131">Время и дата последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="ec7a0-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="ec7a0-132">name</span><span class="sxs-lookup"><span data-stu-id="ec7a0-132">name</span></span>|<span data-ttu-id="ec7a0-133">String</span><span class="sxs-lookup"><span data-stu-id="ec7a0-133">String</span></span>|<span data-ttu-id="ec7a0-134">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="ec7a0-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="ec7a0-135">size</span><span class="sxs-lookup"><span data-stu-id="ec7a0-135">size</span></span>|<span data-ttu-id="ec7a0-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ec7a0-136">Int32</span></span>|<span data-ttu-id="ec7a0-137">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="ec7a0-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec7a0-138">Связи</span><span class="sxs-lookup"><span data-stu-id="ec7a0-138">Relationships</span></span>
| <span data-ttu-id="ec7a0-139">Отношение</span><span class="sxs-lookup"><span data-stu-id="ec7a0-139">Relationship</span></span> | <span data-ttu-id="ec7a0-140">Тип</span><span class="sxs-lookup"><span data-stu-id="ec7a0-140">Type</span></span>   |<span data-ttu-id="ec7a0-141">Описание</span><span class="sxs-lookup"><span data-stu-id="ec7a0-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec7a0-142">item</span><span class="sxs-lookup"><span data-stu-id="ec7a0-142">item</span></span>|[<span data-ttu-id="ec7a0-143">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="ec7a0-143">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="ec7a0-144">Вложенный контакт, сообщение или событие.</span><span class="sxs-lookup"><span data-stu-id="ec7a0-144">The attached contact, message or event.</span></span> <span data-ttu-id="ec7a0-145">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="ec7a0-145">Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec7a0-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ec7a0-146">JSON representation</span></span>

<span data-ttu-id="ec7a0-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec7a0-147">Here is a JSON representation of the resource</span></span>

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
