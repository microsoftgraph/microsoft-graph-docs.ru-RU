---
title: Тип ресурса itemAttachment
description: 'Контакт, событие или сообщение, вложенное в другое событие, сообщение или запись.  '
localization_priority: Priority
ms.prod: outlook
author: svpsiva
doc_type: resourcePageType
ms.openlocfilehash: 1450d365da1146900a661273fa5e19dac58e2903
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461908"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="e8ac7-103">Тип ресурса itemAttachment</span><span class="sxs-lookup"><span data-stu-id="e8ac7-103">itemAttachment resource type</span></span>

<span data-ttu-id="e8ac7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8ac7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e8ac7-105">Контакт, событие или сообщение, вложенное в [событие](../resources/event.md), [сообщение](../resources/message.md) или [запись](../resources/post.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="e8ac7-105">A contact, event, or message that's attached to a user [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="e8ac7-106">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="e8ac7-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e8ac7-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e8ac7-107">Methods</span></span>

| <span data-ttu-id="e8ac7-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e8ac7-108">Method</span></span>       | <span data-ttu-id="e8ac7-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e8ac7-109">Return Type</span></span>  |<span data-ttu-id="e8ac7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e8ac7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e8ac7-111">Получение</span><span class="sxs-lookup"><span data-stu-id="e8ac7-111">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="e8ac7-112">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="e8ac7-112">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="e8ac7-113">Чтение свойств, связей или необработанного содержимого объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="e8ac7-113">Read the properties, relationships, or raw contents of an itemAttachment object.</span></span>|
|<span data-ttu-id="e8ac7-114">[удаление](../api/attachment-delete.md);</span><span class="sxs-lookup"><span data-stu-id="e8ac7-114">[Delete](../api/attachment-delete.md)</span></span> | <span data-ttu-id="e8ac7-115">Нет</span><span class="sxs-lookup"><span data-stu-id="e8ac7-115">None</span></span> |<span data-ttu-id="e8ac7-116">Удаление объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="e8ac7-116">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e8ac7-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="e8ac7-117">Properties</span></span>
| <span data-ttu-id="e8ac7-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8ac7-118">Property</span></span>     | <span data-ttu-id="e8ac7-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e8ac7-119">Type</span></span>   |<span data-ttu-id="e8ac7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e8ac7-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8ac7-121">contentType</span><span class="sxs-lookup"><span data-stu-id="e8ac7-121">contentType</span></span>|<span data-ttu-id="e8ac7-122">String</span><span class="sxs-lookup"><span data-stu-id="e8ac7-122">String</span></span>|<span data-ttu-id="e8ac7-123">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="e8ac7-123">The content type of the attachment.</span></span>|
|<span data-ttu-id="e8ac7-124">id</span><span class="sxs-lookup"><span data-stu-id="e8ac7-124">id</span></span>|<span data-ttu-id="e8ac7-125">String</span><span class="sxs-lookup"><span data-stu-id="e8ac7-125">String</span></span>| <span data-ttu-id="e8ac7-126">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="e8ac7-126">The attachment ID.</span></span>|
|<span data-ttu-id="e8ac7-127">isInline</span><span class="sxs-lookup"><span data-stu-id="e8ac7-127">isInline</span></span>|<span data-ttu-id="e8ac7-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8ac7-128">Boolean</span></span>|<span data-ttu-id="e8ac7-129">Значение true указывает, что вложение является встроенным, например внедренным изображением в теле элемента.</span><span class="sxs-lookup"><span data-stu-id="e8ac7-129">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="e8ac7-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8ac7-130">lastModifiedDateTime</span></span>|<span data-ttu-id="e8ac7-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8ac7-131">DateTimeOffset</span></span>|<span data-ttu-id="e8ac7-132">Время и дата последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="e8ac7-132">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="e8ac7-133">name</span><span class="sxs-lookup"><span data-stu-id="e8ac7-133">name</span></span>|<span data-ttu-id="e8ac7-134">String</span><span class="sxs-lookup"><span data-stu-id="e8ac7-134">String</span></span>|<span data-ttu-id="e8ac7-135">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="e8ac7-135">The display name of the attachment.</span></span>|
|<span data-ttu-id="e8ac7-136">size</span><span class="sxs-lookup"><span data-stu-id="e8ac7-136">size</span></span>|<span data-ttu-id="e8ac7-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e8ac7-137">Int32</span></span>|<span data-ttu-id="e8ac7-138">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="e8ac7-138">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8ac7-139">Связи</span><span class="sxs-lookup"><span data-stu-id="e8ac7-139">Relationships</span></span>
| <span data-ttu-id="e8ac7-140">Связь</span><span class="sxs-lookup"><span data-stu-id="e8ac7-140">Relationship</span></span> | <span data-ttu-id="e8ac7-141">Тип</span><span class="sxs-lookup"><span data-stu-id="e8ac7-141">Type</span></span>   |<span data-ttu-id="e8ac7-142">Описание</span><span class="sxs-lookup"><span data-stu-id="e8ac7-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8ac7-143">item</span><span class="sxs-lookup"><span data-stu-id="e8ac7-143">item</span></span>|[<span data-ttu-id="e8ac7-144">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="e8ac7-144">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="e8ac7-p101">Вложенное сообщение или событие. Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="e8ac7-p101">The attached message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8ac7-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e8ac7-147">JSON representation</span></span>

<span data-ttu-id="e8ac7-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8ac7-148">Here is a JSON representation of the resource</span></span>

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
