---
title: Тип ресурса referenceAttachment
description: Ссылка на файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или в других поддерживаемых местах хранения, вложенный в событие, сообщение или запись.
ms.openlocfilehash: b3604791c7e06d4f765a81263e1f6afe51743390
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028207"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="b2941-103">Тип ресурса referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="b2941-103">referenceAttachment resource type</span></span>

<span data-ttu-id="b2941-104">Ссылка на файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или в других поддерживаемых местах хранения, вложенный в событие, сообщение или запись.</span><span class="sxs-lookup"><span data-stu-id="b2941-104">A link to a file (such as a text file or Word document) on a OneDrive for Business cloud drive or other supported storage locations, attached to an event, message, or post.</span></span>

<span data-ttu-id="b2941-105">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="b2941-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b2941-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b2941-106">Methods</span></span>

| <span data-ttu-id="b2941-107">Метод</span><span class="sxs-lookup"><span data-stu-id="b2941-107">Method</span></span>       | <span data-ttu-id="b2941-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b2941-108">Return Type</span></span>  |<span data-ttu-id="b2941-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b2941-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b2941-110">Get</span><span class="sxs-lookup"><span data-stu-id="b2941-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="b2941-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="b2941-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="b2941-112">Чтение свойств и связей объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="b2941-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="b2941-113">Delete</span><span class="sxs-lookup"><span data-stu-id="b2941-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="b2941-114">Нет</span><span class="sxs-lookup"><span data-stu-id="b2941-114">None</span></span> |<span data-ttu-id="b2941-115">Удаление объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="b2941-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b2941-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2941-116">Properties</span></span>
| <span data-ttu-id="b2941-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2941-117">Property</span></span>     | <span data-ttu-id="b2941-118">Тип</span><span class="sxs-lookup"><span data-stu-id="b2941-118">Type</span></span>   |<span data-ttu-id="b2941-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b2941-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2941-120">contentType</span><span class="sxs-lookup"><span data-stu-id="b2941-120">contentType</span></span>|<span data-ttu-id="b2941-121">String</span><span class="sxs-lookup"><span data-stu-id="b2941-121">String</span></span>|<span data-ttu-id="b2941-122">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="b2941-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="b2941-123">id</span><span class="sxs-lookup"><span data-stu-id="b2941-123">id</span></span>|<span data-ttu-id="b2941-124">String</span><span class="sxs-lookup"><span data-stu-id="b2941-124">String</span></span>|<span data-ttu-id="b2941-p101">Идентификатор вложения.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b2941-p101">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="b2941-127">isInline</span><span class="sxs-lookup"><span data-stu-id="b2941-127">isInline</span></span>|<span data-ttu-id="b2941-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2941-128">Boolean</span></span>|<span data-ttu-id="b2941-129">Значение true указывает, что вложение встроено в содержимое объекта.</span><span class="sxs-lookup"><span data-stu-id="b2941-129">Set to true if the attachment appears inline in the body of the embedding object.</span></span>|
|<span data-ttu-id="b2941-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2941-130">lastModifiedDateTime</span></span>|<span data-ttu-id="b2941-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2941-131">DateTimeOffset</span></span>|<span data-ttu-id="b2941-p102">Дата и время последнего изменения вложения. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b2941-p102">The date and time when the attachment was last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b2941-135">имя</span><span class="sxs-lookup"><span data-stu-id="b2941-135">name</span></span>|<span data-ttu-id="b2941-136">String</span><span class="sxs-lookup"><span data-stu-id="b2941-136">String</span></span>|<span data-ttu-id="b2941-p103">Текст, который отображается под значком, представляет внедренное вложение. Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="b2941-p103">The text that is displayed below the icon representing the embedded attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="b2941-139">size</span><span class="sxs-lookup"><span data-stu-id="b2941-139">size</span></span>|<span data-ttu-id="b2941-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b2941-140">Int32</span></span>|<span data-ttu-id="b2941-141">Объем метаданных, которые хранятся в сообщении с вложением (в байтах).</span><span class="sxs-lookup"><span data-stu-id="b2941-141">The size of the metadata that is stored on the message for the attachment in bytes.</span></span> <span data-ttu-id="b2941-142">Это значение не отображает фактический размер файла.</span><span class="sxs-lookup"><span data-stu-id="b2941-142">This value does not indicate the size of the actual file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2941-143">Связи</span><span class="sxs-lookup"><span data-stu-id="b2941-143">Relationships</span></span>
<span data-ttu-id="b2941-144">Нет</span><span class="sxs-lookup"><span data-stu-id="b2941-144">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="b2941-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2941-145">JSON representation</span></span>

<span data-ttu-id="b2941-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2941-146">Here is a JSON representation of the resource</span></span>

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
