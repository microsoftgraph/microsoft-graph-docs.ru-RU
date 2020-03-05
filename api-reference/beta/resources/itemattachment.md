---
title: Тип ресурса itemAttachment
description: Контакт, событие или сообщение, присоединенное к другому событию,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 82f0e9fa1ab499d7adc305cd74fcf7cdf09fd796
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523095"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="bd5e5-103">Тип ресурса itemAttachment</span><span class="sxs-lookup"><span data-stu-id="bd5e5-103">itemAttachment resource type</span></span>

<span data-ttu-id="bd5e5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bd5e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd5e5-105">Контакт, событие или сообщение, прикрепленное к [событию](../resources/event.md)пользователя, [сообщению](../resources/message.md), [задаче Outlook](../resources/outlooktask.md)или [POST](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="bd5e5-105">A contact, event, or message that's attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="bd5e5-106">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="bd5e5-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="bd5e5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="bd5e5-107">Methods</span></span>

| <span data-ttu-id="bd5e5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="bd5e5-108">Method</span></span>       | <span data-ttu-id="bd5e5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bd5e5-109">Return Type</span></span>  |<span data-ttu-id="bd5e5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bd5e5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bd5e5-111">Получение</span><span class="sxs-lookup"><span data-stu-id="bd5e5-111">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="bd5e5-112">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="bd5e5-112">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="bd5e5-113">Чтение свойств, связей или необработанного содержимого объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="bd5e5-113">Read the properties, relationships, or raw contents of an itemAttachment object.</span></span>|
|<span data-ttu-id="bd5e5-114">[удаление](../api/attachment-delete.md);</span><span class="sxs-lookup"><span data-stu-id="bd5e5-114">[Delete](../api/attachment-delete.md)</span></span> | <span data-ttu-id="bd5e5-115">Нет</span><span class="sxs-lookup"><span data-stu-id="bd5e5-115">None</span></span> |<span data-ttu-id="bd5e5-116">Удаление объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="bd5e5-116">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bd5e5-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd5e5-117">Properties</span></span>
| <span data-ttu-id="bd5e5-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd5e5-118">Property</span></span>     | <span data-ttu-id="bd5e5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="bd5e5-119">Type</span></span>   |<span data-ttu-id="bd5e5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bd5e5-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd5e5-121">contentType</span><span class="sxs-lookup"><span data-stu-id="bd5e5-121">contentType</span></span>|<span data-ttu-id="bd5e5-122">String</span><span class="sxs-lookup"><span data-stu-id="bd5e5-122">String</span></span>|<span data-ttu-id="bd5e5-123">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="bd5e5-123">The content type of the attachment.</span></span>|
|<span data-ttu-id="bd5e5-124">id</span><span class="sxs-lookup"><span data-stu-id="bd5e5-124">id</span></span>|<span data-ttu-id="bd5e5-125">Строка</span><span class="sxs-lookup"><span data-stu-id="bd5e5-125">String</span></span>| <span data-ttu-id="bd5e5-126">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="bd5e5-126">The attachment ID.</span></span>|
|<span data-ttu-id="bd5e5-127">isInline</span><span class="sxs-lookup"><span data-stu-id="bd5e5-127">isInline</span></span>|<span data-ttu-id="bd5e5-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd5e5-128">Boolean</span></span>|<span data-ttu-id="bd5e5-129">Значение true указывает, что вложение является встроенным, например внедренным изображением в теле элемента.</span><span class="sxs-lookup"><span data-stu-id="bd5e5-129">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="bd5e5-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd5e5-130">lastModifiedDateTime</span></span>|<span data-ttu-id="bd5e5-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd5e5-131">DateTimeOffset</span></span>|<span data-ttu-id="bd5e5-132">Время и дата последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="bd5e5-132">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="bd5e5-133">name</span><span class="sxs-lookup"><span data-stu-id="bd5e5-133">name</span></span>|<span data-ttu-id="bd5e5-134">String</span><span class="sxs-lookup"><span data-stu-id="bd5e5-134">String</span></span>|<span data-ttu-id="bd5e5-135">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="bd5e5-135">The display name of the attachment.</span></span>|
|<span data-ttu-id="bd5e5-136">size</span><span class="sxs-lookup"><span data-stu-id="bd5e5-136">size</span></span>|<span data-ttu-id="bd5e5-137">Int32</span><span class="sxs-lookup"><span data-stu-id="bd5e5-137">Int32</span></span>|<span data-ttu-id="bd5e5-138">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="bd5e5-138">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd5e5-139">Связи</span><span class="sxs-lookup"><span data-stu-id="bd5e5-139">Relationships</span></span>
| <span data-ttu-id="bd5e5-140">Связь</span><span class="sxs-lookup"><span data-stu-id="bd5e5-140">Relationship</span></span> | <span data-ttu-id="bd5e5-141">Тип</span><span class="sxs-lookup"><span data-stu-id="bd5e5-141">Type</span></span>   |<span data-ttu-id="bd5e5-142">Описание</span><span class="sxs-lookup"><span data-stu-id="bd5e5-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd5e5-143">item</span><span class="sxs-lookup"><span data-stu-id="bd5e5-143">item</span></span>|[<span data-ttu-id="bd5e5-144">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="bd5e5-144">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="bd5e5-145">Вложенный контакт, сообщение или событие.</span><span class="sxs-lookup"><span data-stu-id="bd5e5-145">The attached contact, message or event.</span></span> <span data-ttu-id="bd5e5-146">Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="bd5e5-146">Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bd5e5-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd5e5-147">JSON representation</span></span>

<span data-ttu-id="bd5e5-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd5e5-148">Here is a JSON representation of the resource</span></span>

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
