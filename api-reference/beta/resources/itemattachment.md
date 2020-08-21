---
title: Тип ресурса itemAttachment
description: Контакт, событие или сообщение, вложенное в другое событие.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 5544c2d4530832f1d18d9760445821fbafeec6e3
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849767"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="f84fe-103">Тип ресурса itemAttachment</span><span class="sxs-lookup"><span data-stu-id="f84fe-103">itemAttachment resource type</span></span>

<span data-ttu-id="f84fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f84fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="f84fe-105">Контакт, событие или сообщение, вложенное в событие [message](../resources/message.md) [пользователя, сообщение,](../resources/event.md) [задачу Outlook](../resources/outlooktask.md)или [запись.](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="f84fe-105">A contact, event, or message that's attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="f84fe-106">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="f84fe-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f84fe-107">Методы</span><span class="sxs-lookup"><span data-stu-id="f84fe-107">Methods</span></span>

| <span data-ttu-id="f84fe-108">Метод</span><span class="sxs-lookup"><span data-stu-id="f84fe-108">Method</span></span>       | <span data-ttu-id="f84fe-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f84fe-109">Return Type</span></span>  |<span data-ttu-id="f84fe-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f84fe-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f84fe-111">Получение</span><span class="sxs-lookup"><span data-stu-id="f84fe-111">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="f84fe-112">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="f84fe-112">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="f84fe-113">Чтение свойств, связей или необработанного содержимого объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="f84fe-113">Read the properties, relationships, or raw contents of an itemAttachment object.</span></span>|
|<span data-ttu-id="f84fe-114">[удаление](../api/attachment-delete.md);</span><span class="sxs-lookup"><span data-stu-id="f84fe-114">[Delete](../api/attachment-delete.md)</span></span> | <span data-ttu-id="f84fe-115">Нет</span><span class="sxs-lookup"><span data-stu-id="f84fe-115">None</span></span> |<span data-ttu-id="f84fe-116">Удаление объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="f84fe-116">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f84fe-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="f84fe-117">Properties</span></span>
| <span data-ttu-id="f84fe-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="f84fe-118">Property</span></span>     | <span data-ttu-id="f84fe-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f84fe-119">Type</span></span>   |<span data-ttu-id="f84fe-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f84fe-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f84fe-121">contentType</span><span class="sxs-lookup"><span data-stu-id="f84fe-121">contentType</span></span>|<span data-ttu-id="f84fe-122">String</span><span class="sxs-lookup"><span data-stu-id="f84fe-122">String</span></span>|<span data-ttu-id="f84fe-123">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="f84fe-123">The content type of the attachment.</span></span>|
|<span data-ttu-id="f84fe-124">id</span><span class="sxs-lookup"><span data-stu-id="f84fe-124">id</span></span>|<span data-ttu-id="f84fe-125">String</span><span class="sxs-lookup"><span data-stu-id="f84fe-125">String</span></span>| <span data-ttu-id="f84fe-126">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="f84fe-126">The attachment ID.</span></span>|
|<span data-ttu-id="f84fe-127">isInline</span><span class="sxs-lookup"><span data-stu-id="f84fe-127">isInline</span></span>|<span data-ttu-id="f84fe-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="f84fe-128">Boolean</span></span>|<span data-ttu-id="f84fe-129">Значение true указывает, что вложение является встроенным, например внедренным изображением в теле элемента.</span><span class="sxs-lookup"><span data-stu-id="f84fe-129">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="f84fe-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f84fe-130">lastModifiedDateTime</span></span>|<span data-ttu-id="f84fe-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f84fe-131">DateTimeOffset</span></span>|<span data-ttu-id="f84fe-132">Время и дата последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="f84fe-132">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="f84fe-133">name</span><span class="sxs-lookup"><span data-stu-id="f84fe-133">name</span></span>|<span data-ttu-id="f84fe-134">String</span><span class="sxs-lookup"><span data-stu-id="f84fe-134">String</span></span>|<span data-ttu-id="f84fe-135">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="f84fe-135">The display name of the attachment.</span></span>|
|<span data-ttu-id="f84fe-136">size</span><span class="sxs-lookup"><span data-stu-id="f84fe-136">size</span></span>|<span data-ttu-id="f84fe-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f84fe-137">Int32</span></span>|<span data-ttu-id="f84fe-138">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="f84fe-138">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f84fe-139">Связи</span><span class="sxs-lookup"><span data-stu-id="f84fe-139">Relationships</span></span>
| <span data-ttu-id="f84fe-140">Связь</span><span class="sxs-lookup"><span data-stu-id="f84fe-140">Relationship</span></span> | <span data-ttu-id="f84fe-141">Тип</span><span class="sxs-lookup"><span data-stu-id="f84fe-141">Type</span></span>   |<span data-ttu-id="f84fe-142">Описание</span><span class="sxs-lookup"><span data-stu-id="f84fe-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f84fe-143">item</span><span class="sxs-lookup"><span data-stu-id="f84fe-143">item</span></span>|[<span data-ttu-id="f84fe-144">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="f84fe-144">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="f84fe-p101">Вложенный контакт, сообщение или событие. Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="f84fe-p101">The attached contact, message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f84fe-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f84fe-147">JSON representation</span></span>

<span data-ttu-id="f84fe-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f84fe-148">Here is a JSON representation of the resource</span></span>

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
