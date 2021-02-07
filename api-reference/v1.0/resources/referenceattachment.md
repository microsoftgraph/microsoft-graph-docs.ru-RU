---
title: Тип ресурса referenceAttachment
description: Ссылка на файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или в других поддерживаемых местах хранения, вложенный в событие, сообщение или запись.
localization_priority: Normal
ms.prod: outlook
author: abheek-das
doc_type: resourcePageType
ms.openlocfilehash: ae16b7df05a6a240b0081e189d74b4622f2f7988
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129342"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="4e554-103">Тип ресурса referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="4e554-103">referenceAttachment resource type</span></span>

<span data-ttu-id="4e554-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e554-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4e554-105">Ссылка на файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или в других поддерживаемых местах хранения, вложенный в событие, сообщение или запись.</span><span class="sxs-lookup"><span data-stu-id="4e554-105">A link to a file (such as a text file or Word document) on a OneDrive for Business cloud drive or other supported storage locations, attached to an event, message, or post.</span></span>

<span data-ttu-id="4e554-106">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="4e554-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4e554-107">Методы</span><span class="sxs-lookup"><span data-stu-id="4e554-107">Methods</span></span>

| <span data-ttu-id="4e554-108">Метод</span><span class="sxs-lookup"><span data-stu-id="4e554-108">Method</span></span>       | <span data-ttu-id="4e554-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4e554-109">Return Type</span></span>  |<span data-ttu-id="4e554-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4e554-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e554-111">[получение](../api/attachment-get.md);</span><span class="sxs-lookup"><span data-stu-id="4e554-111">[Get](../api/attachment-get.md)</span></span> | [<span data-ttu-id="4e554-112">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="4e554-112">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="4e554-113">Чтение свойств и связей объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="4e554-113">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="4e554-114">Удаление</span><span class="sxs-lookup"><span data-stu-id="4e554-114">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="4e554-115">Нет</span><span class="sxs-lookup"><span data-stu-id="4e554-115">None</span></span> |<span data-ttu-id="4e554-116">Удаление объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="4e554-116">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4e554-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e554-117">Properties</span></span>
| <span data-ttu-id="4e554-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e554-118">Property</span></span>     | <span data-ttu-id="4e554-119">Тип</span><span class="sxs-lookup"><span data-stu-id="4e554-119">Type</span></span>   |<span data-ttu-id="4e554-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4e554-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e554-121">contentType</span><span class="sxs-lookup"><span data-stu-id="4e554-121">contentType</span></span>|<span data-ttu-id="4e554-122">String</span><span class="sxs-lookup"><span data-stu-id="4e554-122">String</span></span>|<span data-ttu-id="4e554-123">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="4e554-123">The content type of the attachment.</span></span>|
|<span data-ttu-id="4e554-124">id</span><span class="sxs-lookup"><span data-stu-id="4e554-124">id</span></span>|<span data-ttu-id="4e554-125">String</span><span class="sxs-lookup"><span data-stu-id="4e554-125">String</span></span>|<span data-ttu-id="4e554-p101">Идентификатор вложения.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e554-p101">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="4e554-128">isInline</span><span class="sxs-lookup"><span data-stu-id="4e554-128">isInline</span></span>|<span data-ttu-id="4e554-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e554-129">Boolean</span></span>|<span data-ttu-id="4e554-130">Значение true указывает, что вложение встроено в содержимое объекта.</span><span class="sxs-lookup"><span data-stu-id="4e554-130">Set to true if the attachment appears inline in the body of the embedding object.</span></span>|
|<span data-ttu-id="4e554-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e554-131">lastModifiedDateTime</span></span>|<span data-ttu-id="4e554-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e554-132">DateTimeOffset</span></span>|<span data-ttu-id="4e554-p102">Дата и время последнего изменения вложения. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4e554-p102">The date and time when the attachment was last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4e554-136">name</span><span class="sxs-lookup"><span data-stu-id="4e554-136">name</span></span>|<span data-ttu-id="4e554-137">String</span><span class="sxs-lookup"><span data-stu-id="4e554-137">String</span></span>|<span data-ttu-id="4e554-p103">Текст, который отображается под значком, представляет внедренное вложение. Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="4e554-p103">The text that is displayed below the icon representing the embedded attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="4e554-140">size</span><span class="sxs-lookup"><span data-stu-id="4e554-140">size</span></span>|<span data-ttu-id="4e554-141">Int32</span><span class="sxs-lookup"><span data-stu-id="4e554-141">Int32</span></span>|<span data-ttu-id="4e554-142">Объем метаданных, которые хранятся в сообщении с вложением (в байтах).</span><span class="sxs-lookup"><span data-stu-id="4e554-142">The size of the metadata that is stored on the message for the attachment in bytes.</span></span> <span data-ttu-id="4e554-143">Это значение не отображает фактический размер файла.</span><span class="sxs-lookup"><span data-stu-id="4e554-143">This value does not indicate the size of the actual file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e554-144">Связи</span><span class="sxs-lookup"><span data-stu-id="4e554-144">Relationships</span></span>
<span data-ttu-id="4e554-145">Нет</span><span class="sxs-lookup"><span data-stu-id="4e554-145">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="4e554-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e554-146">JSON representation</span></span>

<span data-ttu-id="4e554-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e554-147">Here is a JSON representation of the resource</span></span>

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

