---
title: Тип ресурса referenceAttachment
description: Ссылка на файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или в других поддерживаемых местах хранения, вложенный в событие, сообщение или запись.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 21f88a6b3e8374eda3af11ca7094539e66137148
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034792"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="8e40f-103">Тип ресурса referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="8e40f-103">referenceAttachment resource type</span></span>

<span data-ttu-id="8e40f-104">Ссылка на файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или в других поддерживаемых местах хранения, вложенный в событие, сообщение или запись.</span><span class="sxs-lookup"><span data-stu-id="8e40f-104">A link to a file (such as a text file or Word document) on a OneDrive for Business cloud drive or other supported storage locations, attached to an event, message, or post.</span></span>

<span data-ttu-id="8e40f-105">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="8e40f-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8e40f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8e40f-106">Methods</span></span>

| <span data-ttu-id="8e40f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8e40f-107">Method</span></span>       | <span data-ttu-id="8e40f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8e40f-108">Return Type</span></span>  |<span data-ttu-id="8e40f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8e40f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8e40f-110">Получение</span><span class="sxs-lookup"><span data-stu-id="8e40f-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="8e40f-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="8e40f-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="8e40f-112">Чтение свойств и связей объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="8e40f-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="8e40f-113">Удаление</span><span class="sxs-lookup"><span data-stu-id="8e40f-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="8e40f-114">Нет</span><span class="sxs-lookup"><span data-stu-id="8e40f-114">None</span></span> |<span data-ttu-id="8e40f-115">Удаление объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="8e40f-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8e40f-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e40f-116">Properties</span></span>
| <span data-ttu-id="8e40f-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e40f-117">Property</span></span>     | <span data-ttu-id="8e40f-118">Тип</span><span class="sxs-lookup"><span data-stu-id="8e40f-118">Type</span></span>   |<span data-ttu-id="8e40f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8e40f-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e40f-120">contentType</span><span class="sxs-lookup"><span data-stu-id="8e40f-120">contentType</span></span>|<span data-ttu-id="8e40f-121">String</span><span class="sxs-lookup"><span data-stu-id="8e40f-121">String</span></span>|<span data-ttu-id="8e40f-122">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="8e40f-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="8e40f-123">id</span><span class="sxs-lookup"><span data-stu-id="8e40f-123">id</span></span>|<span data-ttu-id="8e40f-124">Строка</span><span class="sxs-lookup"><span data-stu-id="8e40f-124">String</span></span>|<span data-ttu-id="8e40f-p101">Идентификатор вложения.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e40f-p101">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="8e40f-127">isInline</span><span class="sxs-lookup"><span data-stu-id="8e40f-127">isInline</span></span>|<span data-ttu-id="8e40f-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e40f-128">Boolean</span></span>|<span data-ttu-id="8e40f-129">Значение true указывает, что вложение встроено в содержимое объекта.</span><span class="sxs-lookup"><span data-stu-id="8e40f-129">Set to true if the attachment appears inline in the body of the embedding object.</span></span>|
|<span data-ttu-id="8e40f-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e40f-130">lastModifiedDateTime</span></span>|<span data-ttu-id="8e40f-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e40f-131">DateTimeOffset</span></span>|<span data-ttu-id="8e40f-p102">Дата и время последнего изменения вложения. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8e40f-p102">The date and time when the attachment was last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8e40f-135">name</span><span class="sxs-lookup"><span data-stu-id="8e40f-135">name</span></span>|<span data-ttu-id="8e40f-136">String</span><span class="sxs-lookup"><span data-stu-id="8e40f-136">String</span></span>|<span data-ttu-id="8e40f-p103">Текст, который отображается под значком, представляет внедренное вложение. Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="8e40f-p103">The text that is displayed below the icon representing the embedded attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="8e40f-139">size</span><span class="sxs-lookup"><span data-stu-id="8e40f-139">size</span></span>|<span data-ttu-id="8e40f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8e40f-140">Int32</span></span>|<span data-ttu-id="8e40f-141">Объем метаданных, которые хранятся в сообщении с вложением (в байтах).</span><span class="sxs-lookup"><span data-stu-id="8e40f-141">The size of the metadata that is stored on the message for the attachment in bytes.</span></span> <span data-ttu-id="8e40f-142">Это значение не отображает фактический размер файла.</span><span class="sxs-lookup"><span data-stu-id="8e40f-142">This value does not indicate the size of the actual file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e40f-143">Отношения</span><span class="sxs-lookup"><span data-stu-id="8e40f-143">Relationships</span></span>
<span data-ttu-id="8e40f-144">Нет</span><span class="sxs-lookup"><span data-stu-id="8e40f-144">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="8e40f-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e40f-145">JSON representation</span></span>

<span data-ttu-id="8e40f-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e40f-146">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.attachment",
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
