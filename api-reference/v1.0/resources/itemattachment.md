---
title: Тип ресурса itemAttachment
description: 'Контакт, событие или сообщение, вложенное в другое событие, сообщение или запись.  '
ms.openlocfilehash: 79097b10327d895a41090e068a2fd8e9681df125
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026263"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="0db6e-103">Тип ресурса itemAttachment</span><span class="sxs-lookup"><span data-stu-id="0db6e-103">itemAttachment resource type</span></span>

<span data-ttu-id="0db6e-104">Контакт, событие или сообщение, вложенное в другое событие, сообщение или запись.</span><span class="sxs-lookup"><span data-stu-id="0db6e-104">A contact, event, or message that's attached to another event, message, or post.</span></span>  

<span data-ttu-id="0db6e-105">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="0db6e-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0db6e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="0db6e-106">Methods</span></span>

| <span data-ttu-id="0db6e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="0db6e-107">Method</span></span>       | <span data-ttu-id="0db6e-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0db6e-108">Return Type</span></span>  |<span data-ttu-id="0db6e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0db6e-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0db6e-110">Get</span><span class="sxs-lookup"><span data-stu-id="0db6e-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="0db6e-111">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="0db6e-111">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="0db6e-112">Чтение свойств и связей объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="0db6e-112">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="0db6e-113">Delete</span><span class="sxs-lookup"><span data-stu-id="0db6e-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="0db6e-114">Нет</span><span class="sxs-lookup"><span data-stu-id="0db6e-114">None</span></span> |<span data-ttu-id="0db6e-115">Удаление объекта itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="0db6e-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0db6e-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="0db6e-116">Properties</span></span>
| <span data-ttu-id="0db6e-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="0db6e-117">Property</span></span>     | <span data-ttu-id="0db6e-118">Тип</span><span class="sxs-lookup"><span data-stu-id="0db6e-118">Type</span></span>   |<span data-ttu-id="0db6e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0db6e-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0db6e-120">contentType</span><span class="sxs-lookup"><span data-stu-id="0db6e-120">contentType</span></span>|<span data-ttu-id="0db6e-121">String</span><span class="sxs-lookup"><span data-stu-id="0db6e-121">String</span></span>|<span data-ttu-id="0db6e-122">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="0db6e-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="0db6e-123">id</span><span class="sxs-lookup"><span data-stu-id="0db6e-123">id</span></span>|<span data-ttu-id="0db6e-124">String</span><span class="sxs-lookup"><span data-stu-id="0db6e-124">String</span></span>| <span data-ttu-id="0db6e-125">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="0db6e-125">The attachment ID.</span></span>|
|<span data-ttu-id="0db6e-126">isInline</span><span class="sxs-lookup"><span data-stu-id="0db6e-126">isInline</span></span>|<span data-ttu-id="0db6e-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="0db6e-127">Boolean</span></span>|<span data-ttu-id="0db6e-128">Значение true указывает, что вложение является встроенным, например внедренным изображением в теле элемента.</span><span class="sxs-lookup"><span data-stu-id="0db6e-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="0db6e-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0db6e-129">lastModifiedDateTime</span></span>|<span data-ttu-id="0db6e-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0db6e-130">DateTimeOffset</span></span>|<span data-ttu-id="0db6e-131">Время и дата последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="0db6e-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="0db6e-132">name</span><span class="sxs-lookup"><span data-stu-id="0db6e-132">name</span></span>|<span data-ttu-id="0db6e-133">String</span><span class="sxs-lookup"><span data-stu-id="0db6e-133">String</span></span>|<span data-ttu-id="0db6e-134">Отображаемое имя вложения.</span><span class="sxs-lookup"><span data-stu-id="0db6e-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="0db6e-135">size</span><span class="sxs-lookup"><span data-stu-id="0db6e-135">size</span></span>|<span data-ttu-id="0db6e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="0db6e-136">Int32</span></span>|<span data-ttu-id="0db6e-137">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="0db6e-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0db6e-138">Связи</span><span class="sxs-lookup"><span data-stu-id="0db6e-138">Relationships</span></span>
| <span data-ttu-id="0db6e-139">Связь</span><span class="sxs-lookup"><span data-stu-id="0db6e-139">Relationship</span></span> | <span data-ttu-id="0db6e-140">Тип</span><span class="sxs-lookup"><span data-stu-id="0db6e-140">Type</span></span>   |<span data-ttu-id="0db6e-141">Описание</span><span class="sxs-lookup"><span data-stu-id="0db6e-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0db6e-142">item</span><span class="sxs-lookup"><span data-stu-id="0db6e-142">item</span></span>|[<span data-ttu-id="0db6e-143">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="0db6e-143">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="0db6e-p101">Вложенное сообщение или событие. Свойство навигации.</span><span class="sxs-lookup"><span data-stu-id="0db6e-p101">The attached message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0db6e-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0db6e-146">JSON representation</span></span>

<span data-ttu-id="0db6e-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0db6e-147">Here is a JSON representation of the resource</span></span>

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
