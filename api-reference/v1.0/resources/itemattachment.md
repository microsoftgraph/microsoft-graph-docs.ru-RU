---
title: Тип ресурса itemAttachment
description: 'Контакт, событие или сообщение, вложенное в другое событие, сообщение или запись.  '
localization_priority: Priority
ms.prod: outlook
author: angelgolfer-ms
doc_type: resourcePageType
ms.openlocfilehash: c5c565e81ed9218d3d04f15585236b87a362d5e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447642"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="49e97-103">Тип ресурса itemAttachment</span><span class="sxs-lookup"><span data-stu-id="49e97-103">itemAttachment resource type</span></span>

<span data-ttu-id="49e97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49e97-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49e97-105">Контакт, событие или сообщение, вложенное в [событие](../resources/event.md), [сообщение](../resources/message.md) или [запись](../resources/post.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="49e97-105">A contact, event, or message that's attached to a user [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="49e97-106">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="49e97-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="49e97-107">Методы</span><span class="sxs-lookup"><span data-stu-id="49e97-107">Methods</span></span>

| <span data-ttu-id="49e97-108">Метод</span><span class="sxs-lookup"><span data-stu-id="49e97-108">Method</span></span>       | <span data-ttu-id="49e97-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="49e97-109">Return Type</span></span>  |<span data-ttu-id="49e97-110">Описание</span><span class="sxs-lookup"><span data-stu-id="49e97-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="49e97-111">Получение</span><span class="sxs-lookup"><span data-stu-id="49e97-111">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="49e97-112">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="49e97-112">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="49e97-113">Чтение свойств, связей или необработанного содержимого объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="49e97-113">Read the properties, relationships, or raw contents of an itemAttachment object.</span></span>|
|<span data-ttu-id="49e97-114">[удаление](../api/attachment-delete.md);</span><span class="sxs-lookup"><span data-stu-id="49e97-114">[Delete](../api/attachment-delete.md)</span></span> | <span data-ttu-id="49e97-115">Нет</span><span class="sxs-lookup"><span data-stu-id="49e97-115">None</span></span> |<span data-ttu-id="49e97-116">Удаление объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="49e97-116">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="49e97-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="49e97-117">Properties</span></span>
| <span data-ttu-id="49e97-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="49e97-118">Property</span></span>     | <span data-ttu-id="49e97-119">Тип</span><span class="sxs-lookup"><span data-stu-id="49e97-119">Type</span></span>   |<span data-ttu-id="49e97-120">Описание</span><span class="sxs-lookup"><span data-stu-id="49e97-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49e97-121">contentType</span><span class="sxs-lookup"><span data-stu-id="49e97-121">contentType</span></span>|<span data-ttu-id="49e97-122">String</span><span class="sxs-lookup"><span data-stu-id="49e97-122">String</span></span>|<span data-ttu-id="49e97-123">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="49e97-123">The content type of the attachment.</span></span>|
|<span data-ttu-id="49e97-124">id</span><span class="sxs-lookup"><span data-stu-id="49e97-124">id</span></span>|<span data-ttu-id="49e97-125">String</span><span class="sxs-lookup"><span data-stu-id="49e97-125">String</span></span>| <span data-ttu-id="49e97-126">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="49e97-126">The attachment ID.</span></span>|
|<span data-ttu-id="49e97-127">isInline</span><span class="sxs-lookup"><span data-stu-id="49e97-127">isInline</span></span>|<span data-ttu-id="49e97-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="49e97-128">Boolean</span></span>|<span data-ttu-id="49e97-129">Значение true указывает, что вложение является встроенным, например внедренным изображением в теле элемента.</span><span class="sxs-lookup"><span data-stu-id="49e97-129">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="49e97-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49e97-130">lastModifiedDateTime</span></span>|<span data-ttu-id="49e97-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49e97-131">DateTimeOffset</span></span>|<span data-ttu-id="49e97-132">Время и дата последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="49e97-132">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="49e97-133">name</span><span class="sxs-lookup"><span data-stu-id="49e97-133">name</span></span>|<span data-ttu-id="49e97-134">String</span><span class="sxs-lookup"><span data-stu-id="49e97-134">String</span></span>|<span data-ttu-id="49e97-135">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="49e97-135">The display name of the attachment.</span></span>|
|<span data-ttu-id="49e97-136">size</span><span class="sxs-lookup"><span data-stu-id="49e97-136">size</span></span>|<span data-ttu-id="49e97-137">Int32</span><span class="sxs-lookup"><span data-stu-id="49e97-137">Int32</span></span>|<span data-ttu-id="49e97-138">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="49e97-138">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49e97-139">Связи</span><span class="sxs-lookup"><span data-stu-id="49e97-139">Relationships</span></span>
| <span data-ttu-id="49e97-140">Связь</span><span class="sxs-lookup"><span data-stu-id="49e97-140">Relationship</span></span> | <span data-ttu-id="49e97-141">Тип</span><span class="sxs-lookup"><span data-stu-id="49e97-141">Type</span></span>   |<span data-ttu-id="49e97-142">Описание</span><span class="sxs-lookup"><span data-stu-id="49e97-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49e97-143">item</span><span class="sxs-lookup"><span data-stu-id="49e97-143">item</span></span>|[<span data-ttu-id="49e97-144">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="49e97-144">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="49e97-p101">Вложенное сообщение или событие. Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="49e97-p101">The attached message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49e97-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="49e97-147">JSON representation</span></span>

<span data-ttu-id="49e97-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49e97-148">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
  "@odata.type": "microsoft.graph.itemAttachment",
  "@odata.annotations": [
    {
      "property": "item",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024,
  "item": { "@odata.type": "microsoft.graph.outlookItem" }
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
