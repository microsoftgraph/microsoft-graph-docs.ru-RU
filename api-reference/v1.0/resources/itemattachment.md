---
title: Тип ресурса itemAttachment
description: 'Контакт, событие или сообщение, вложенное в другое событие, сообщение или запись.  '
localization_priority: Priority
ms.openlocfilehash: df996175e545b78f4ca9a1b6271b9cb012ffffce
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853524"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="585b2-103">Тип ресурса itemAttachment</span><span class="sxs-lookup"><span data-stu-id="585b2-103">itemAttachment resource type</span></span>

<span data-ttu-id="585b2-104">Контакт, событие или сообщение, вложенное в другое событие, сообщение или запись.</span><span class="sxs-lookup"><span data-stu-id="585b2-104">A contact, event, or message that's attached to another event, message, or post.</span></span>  

<span data-ttu-id="585b2-105">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="585b2-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="585b2-106">Методы</span><span class="sxs-lookup"><span data-stu-id="585b2-106">Methods</span></span>

| <span data-ttu-id="585b2-107">Метод</span><span class="sxs-lookup"><span data-stu-id="585b2-107">Method</span></span>       | <span data-ttu-id="585b2-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="585b2-108">Return Type</span></span>  |<span data-ttu-id="585b2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="585b2-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="585b2-110">Получение</span><span class="sxs-lookup"><span data-stu-id="585b2-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="585b2-111">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="585b2-111">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="585b2-112">Чтение свойств и связей объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="585b2-112">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="585b2-113">Delete</span><span class="sxs-lookup"><span data-stu-id="585b2-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="585b2-114">Нет</span><span class="sxs-lookup"><span data-stu-id="585b2-114">None</span></span> |<span data-ttu-id="585b2-115">Удаление объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="585b2-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="585b2-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="585b2-116">Properties</span></span>
| <span data-ttu-id="585b2-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="585b2-117">Property</span></span>     | <span data-ttu-id="585b2-118">Тип</span><span class="sxs-lookup"><span data-stu-id="585b2-118">Type</span></span>   |<span data-ttu-id="585b2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="585b2-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="585b2-120">contentType</span><span class="sxs-lookup"><span data-stu-id="585b2-120">contentType</span></span>|<span data-ttu-id="585b2-121">String</span><span class="sxs-lookup"><span data-stu-id="585b2-121">String</span></span>|<span data-ttu-id="585b2-122">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="585b2-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="585b2-123">id</span><span class="sxs-lookup"><span data-stu-id="585b2-123">id</span></span>|<span data-ttu-id="585b2-124">String</span><span class="sxs-lookup"><span data-stu-id="585b2-124">String</span></span>| <span data-ttu-id="585b2-125">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="585b2-125">The attachment ID.</span></span>|
|<span data-ttu-id="585b2-126">isInline</span><span class="sxs-lookup"><span data-stu-id="585b2-126">isInline</span></span>|<span data-ttu-id="585b2-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="585b2-127">Boolean</span></span>|<span data-ttu-id="585b2-128">Значение true указывает, что вложение является встроенным, например внедренным изображением в теле элемента.</span><span class="sxs-lookup"><span data-stu-id="585b2-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="585b2-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="585b2-129">lastModifiedDateTime</span></span>|<span data-ttu-id="585b2-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="585b2-130">DateTimeOffset</span></span>|<span data-ttu-id="585b2-131">Время и дата последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="585b2-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="585b2-132">name</span><span class="sxs-lookup"><span data-stu-id="585b2-132">name</span></span>|<span data-ttu-id="585b2-133">String</span><span class="sxs-lookup"><span data-stu-id="585b2-133">String</span></span>|<span data-ttu-id="585b2-134">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="585b2-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="585b2-135">size</span><span class="sxs-lookup"><span data-stu-id="585b2-135">size</span></span>|<span data-ttu-id="585b2-136">Int32</span><span class="sxs-lookup"><span data-stu-id="585b2-136">Int32</span></span>|<span data-ttu-id="585b2-137">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="585b2-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="585b2-138">Связи</span><span class="sxs-lookup"><span data-stu-id="585b2-138">Relationships</span></span>
| <span data-ttu-id="585b2-139">Связь</span><span class="sxs-lookup"><span data-stu-id="585b2-139">Relationship</span></span> | <span data-ttu-id="585b2-140">Тип</span><span class="sxs-lookup"><span data-stu-id="585b2-140">Type</span></span>   |<span data-ttu-id="585b2-141">Описание</span><span class="sxs-lookup"><span data-stu-id="585b2-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="585b2-142">item</span><span class="sxs-lookup"><span data-stu-id="585b2-142">item</span></span>|[<span data-ttu-id="585b2-143">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="585b2-143">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="585b2-p101">Вложенное сообщение или событие. Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="585b2-p101">The attached message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="585b2-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="585b2-146">JSON representation</span></span>

<span data-ttu-id="585b2-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="585b2-147">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "baseType": "microsoft.graph.attachment",
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
