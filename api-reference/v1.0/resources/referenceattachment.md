---
title: Тип ресурса referenceAttachment
description: Ссылка на файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или в других поддерживаемых местах хранения, вложенный в событие, сообщение или запись.
localization_priority: Normal
ms.prod: outlook
author: svpsiva
doc_type: resourcePageType
ms.openlocfilehash: e410e5b039a18e32e55058d3f33c0e75be52ee79
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072832"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="e4d38-103">Тип ресурса referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="e4d38-103">referenceAttachment resource type</span></span>

<span data-ttu-id="e4d38-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4d38-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4d38-105">Ссылка на файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или в других поддерживаемых местах хранения, вложенный в событие, сообщение или запись.</span><span class="sxs-lookup"><span data-stu-id="e4d38-105">A link to a file (such as a text file or Word document) on a OneDrive for Business cloud drive or other supported storage locations, attached to an event, message, or post.</span></span>

<span data-ttu-id="e4d38-106">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="e4d38-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e4d38-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e4d38-107">Methods</span></span>

| <span data-ttu-id="e4d38-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e4d38-108">Method</span></span>       | <span data-ttu-id="e4d38-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e4d38-109">Return Type</span></span>  |<span data-ttu-id="e4d38-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e4d38-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e4d38-111">Получение</span><span class="sxs-lookup"><span data-stu-id="e4d38-111">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="e4d38-112">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="e4d38-112">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="e4d38-113">Чтение свойств и связей объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="e4d38-113">Read properties and relationships of referenceAttachment object.</span></span>|
|<span data-ttu-id="e4d38-114">[удаление](../api/attachment-delete.md);</span><span class="sxs-lookup"><span data-stu-id="e4d38-114">[Delete](../api/attachment-delete.md)</span></span> | <span data-ttu-id="e4d38-115">Нет</span><span class="sxs-lookup"><span data-stu-id="e4d38-115">None</span></span> |<span data-ttu-id="e4d38-116">Удаление объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="e4d38-116">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e4d38-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4d38-117">Properties</span></span>
| <span data-ttu-id="e4d38-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4d38-118">Property</span></span>     | <span data-ttu-id="e4d38-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e4d38-119">Type</span></span>   |<span data-ttu-id="e4d38-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e4d38-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4d38-121">contentType</span><span class="sxs-lookup"><span data-stu-id="e4d38-121">contentType</span></span>|<span data-ttu-id="e4d38-122">String</span><span class="sxs-lookup"><span data-stu-id="e4d38-122">String</span></span>|<span data-ttu-id="e4d38-123">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="e4d38-123">The content type of the attachment.</span></span>|
|<span data-ttu-id="e4d38-124">id</span><span class="sxs-lookup"><span data-stu-id="e4d38-124">id</span></span>|<span data-ttu-id="e4d38-125">Строка</span><span class="sxs-lookup"><span data-stu-id="e4d38-125">String</span></span>|<span data-ttu-id="e4d38-p101">Идентификатор вложения.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e4d38-p101">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="e4d38-128">isInline</span><span class="sxs-lookup"><span data-stu-id="e4d38-128">isInline</span></span>|<span data-ttu-id="e4d38-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4d38-129">Boolean</span></span>|<span data-ttu-id="e4d38-130">Значение true указывает, что вложение встроено в содержимое объекта.</span><span class="sxs-lookup"><span data-stu-id="e4d38-130">Set to true if the attachment appears inline in the body of the embedding object.</span></span>|
|<span data-ttu-id="e4d38-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4d38-131">lastModifiedDateTime</span></span>|<span data-ttu-id="e4d38-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4d38-132">DateTimeOffset</span></span>|<span data-ttu-id="e4d38-p102">Дата и время последнего изменения вложения. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e4d38-p102">The date and time when the attachment was last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e4d38-136">name</span><span class="sxs-lookup"><span data-stu-id="e4d38-136">name</span></span>|<span data-ttu-id="e4d38-137">String</span><span class="sxs-lookup"><span data-stu-id="e4d38-137">String</span></span>|<span data-ttu-id="e4d38-p103">Текст, который отображается под значком, представляет внедренное вложение. Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="e4d38-p103">The text that is displayed below the icon representing the embedded attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="e4d38-140">size</span><span class="sxs-lookup"><span data-stu-id="e4d38-140">size</span></span>|<span data-ttu-id="e4d38-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e4d38-141">Int32</span></span>|<span data-ttu-id="e4d38-142">Объем метаданных, которые хранятся в сообщении с вложением (в байтах).</span><span class="sxs-lookup"><span data-stu-id="e4d38-142">The size of the metadata that is stored on the message for the attachment in bytes.</span></span> <span data-ttu-id="e4d38-143">Это значение не отображает фактический размер файла.</span><span class="sxs-lookup"><span data-stu-id="e4d38-143">This value does not indicate the size of the actual file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4d38-144">Связи</span><span class="sxs-lookup"><span data-stu-id="e4d38-144">Relationships</span></span>
<span data-ttu-id="e4d38-145">Нет</span><span class="sxs-lookup"><span data-stu-id="e4d38-145">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="e4d38-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4d38-146">JSON representation</span></span>

<span data-ttu-id="e4d38-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4d38-147">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
  "@odata.type": "microsoft.graph.referenceAttachment"
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
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

