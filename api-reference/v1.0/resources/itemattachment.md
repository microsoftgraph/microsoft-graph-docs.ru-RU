---
title: Тип ресурса itemAttachment
description: 'Контакт, событие или сообщение, вложенное в другое событие, сообщение или запись.  '
localization_priority: Priority
ms.prod: outlook
author: angelgolfer-ms
doc_type: resourcePageType
ms.openlocfilehash: 554a1cd2e0f6059cf9213f1f19d756349ef000fc
ms.sourcegitcommit: 6deec57c0ab736260ee3599703bfd3f567ee6d82
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2019
ms.locfileid: "37036363"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="3855d-103">Тип ресурса itemAttachment</span><span class="sxs-lookup"><span data-stu-id="3855d-103">itemAttachment resource type</span></span>

<span data-ttu-id="3855d-104">Контакт, событие или сообщение, вложенное в [событие](../resources/event.md), [сообщение](../resources/message.md) или [запись](../resources/post.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="3855d-104">A contact, event, or message that's attached to another event, message, or post.</span></span>  

<span data-ttu-id="3855d-105">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="3855d-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3855d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3855d-106">Methods</span></span>

| <span data-ttu-id="3855d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="3855d-107">Method</span></span>       | <span data-ttu-id="3855d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3855d-108">Return Type</span></span>  |<span data-ttu-id="3855d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3855d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3855d-110">Получение</span><span class="sxs-lookup"><span data-stu-id="3855d-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="3855d-111">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="3855d-111">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="3855d-112">Чтение свойств, связей или необработанного содержимого объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="3855d-112">Read properties, relationships, or raw contents of a fileAttachment object.</span></span>|
|<span data-ttu-id="3855d-113">[удаление](../api/attachment-delete.md);</span><span class="sxs-lookup"><span data-stu-id="3855d-113">[Delete](../api/attachment-delete.md)</span></span> | <span data-ttu-id="3855d-114">Нет</span><span class="sxs-lookup"><span data-stu-id="3855d-114">None</span></span> |<span data-ttu-id="3855d-115">Удаление объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="3855d-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3855d-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="3855d-116">Properties</span></span>
| <span data-ttu-id="3855d-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="3855d-117">Property</span></span>     | <span data-ttu-id="3855d-118">Тип</span><span class="sxs-lookup"><span data-stu-id="3855d-118">Type</span></span>   |<span data-ttu-id="3855d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3855d-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3855d-120">contentType</span><span class="sxs-lookup"><span data-stu-id="3855d-120">contentType</span></span>|<span data-ttu-id="3855d-121">String</span><span class="sxs-lookup"><span data-stu-id="3855d-121">String</span></span>|<span data-ttu-id="3855d-122">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="3855d-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="3855d-123">id</span><span class="sxs-lookup"><span data-stu-id="3855d-123">id</span></span>|<span data-ttu-id="3855d-124">String</span><span class="sxs-lookup"><span data-stu-id="3855d-124">String</span></span>| <span data-ttu-id="3855d-125">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="3855d-125">The attachment ID.</span></span>|
|<span data-ttu-id="3855d-126">isInline</span><span class="sxs-lookup"><span data-stu-id="3855d-126">isInline</span></span>|<span data-ttu-id="3855d-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="3855d-127">Boolean</span></span>|<span data-ttu-id="3855d-128">Значение true указывает, что вложение является встроенным, например внедренным изображением в теле элемента.</span><span class="sxs-lookup"><span data-stu-id="3855d-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="3855d-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3855d-129">lastModifiedDateTime</span></span>|<span data-ttu-id="3855d-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3855d-130">DateTimeOffset</span></span>|<span data-ttu-id="3855d-131">Время и дата последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="3855d-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="3855d-132">name</span><span class="sxs-lookup"><span data-stu-id="3855d-132">name</span></span>|<span data-ttu-id="3855d-133">String</span><span class="sxs-lookup"><span data-stu-id="3855d-133">String</span></span>|<span data-ttu-id="3855d-134">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="3855d-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="3855d-135">size</span><span class="sxs-lookup"><span data-stu-id="3855d-135">size</span></span>|<span data-ttu-id="3855d-136">Int32</span><span class="sxs-lookup"><span data-stu-id="3855d-136">Int32</span></span>|<span data-ttu-id="3855d-137">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="3855d-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3855d-138">Связи</span><span class="sxs-lookup"><span data-stu-id="3855d-138">Relationships</span></span>
| <span data-ttu-id="3855d-139">Связь</span><span class="sxs-lookup"><span data-stu-id="3855d-139">Relationship</span></span> | <span data-ttu-id="3855d-140">Тип</span><span class="sxs-lookup"><span data-stu-id="3855d-140">Type</span></span>   |<span data-ttu-id="3855d-141">Описание</span><span class="sxs-lookup"><span data-stu-id="3855d-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3855d-142">item</span><span class="sxs-lookup"><span data-stu-id="3855d-142">item</span></span>|[<span data-ttu-id="3855d-143">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="3855d-143">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="3855d-p101">Вложенное сообщение или событие. Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="3855d-p101">The attached message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3855d-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3855d-146">JSON representation</span></span>

<span data-ttu-id="3855d-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3855d-147">Here is a JSON representation of the resource</span></span>

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
