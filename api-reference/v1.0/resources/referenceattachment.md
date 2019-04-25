---
title: Тип ресурса referenceAttachment
description: Ссылка на файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или в других поддерживаемых местах хранения, вложенный в событие, сообщение или запись.
localization_priority: Normal
ms.openlocfilehash: 0696ac4b0f93ed4982ec576a15afe071486f9c88
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579417"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="a57d1-103">Тип ресурса referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="a57d1-103">referenceAttachment resource type</span></span>

<span data-ttu-id="a57d1-104">Ссылка на файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или в других поддерживаемых местах хранения, вложенный в событие, сообщение или запись.</span><span class="sxs-lookup"><span data-stu-id="a57d1-104">A link to a file (such as a text file or Word document) on a OneDrive for Business cloud drive or other supported storage locations, attached to an event, message, or post.</span></span>

<span data-ttu-id="a57d1-105">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="a57d1-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a57d1-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a57d1-106">Methods</span></span>

| <span data-ttu-id="a57d1-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a57d1-107">Method</span></span>       | <span data-ttu-id="a57d1-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a57d1-108">Return Type</span></span>  |<span data-ttu-id="a57d1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a57d1-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a57d1-110">Get</span><span class="sxs-lookup"><span data-stu-id="a57d1-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="a57d1-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="a57d1-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="a57d1-112">Чтение свойств и связей объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="a57d1-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="a57d1-113">Удаление</span><span class="sxs-lookup"><span data-stu-id="a57d1-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="a57d1-114">Нет</span><span class="sxs-lookup"><span data-stu-id="a57d1-114">None</span></span> |<span data-ttu-id="a57d1-115">Удаление объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="a57d1-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a57d1-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="a57d1-116">Properties</span></span>
| <span data-ttu-id="a57d1-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="a57d1-117">Property</span></span>     | <span data-ttu-id="a57d1-118">Тип</span><span class="sxs-lookup"><span data-stu-id="a57d1-118">Type</span></span>   |<span data-ttu-id="a57d1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a57d1-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a57d1-120">contentType</span><span class="sxs-lookup"><span data-stu-id="a57d1-120">contentType</span></span>|<span data-ttu-id="a57d1-121">String</span><span class="sxs-lookup"><span data-stu-id="a57d1-121">String</span></span>|<span data-ttu-id="a57d1-122">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="a57d1-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="a57d1-123">id</span><span class="sxs-lookup"><span data-stu-id="a57d1-123">id</span></span>|<span data-ttu-id="a57d1-124">Строка</span><span class="sxs-lookup"><span data-stu-id="a57d1-124">String</span></span>|<span data-ttu-id="a57d1-p101">Идентификатор вложения.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a57d1-p101">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="a57d1-127">isInline</span><span class="sxs-lookup"><span data-stu-id="a57d1-127">isInline</span></span>|<span data-ttu-id="a57d1-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="a57d1-128">Boolean</span></span>|<span data-ttu-id="a57d1-129">Значение true указывает, что вложение встроено в содержимое объекта.</span><span class="sxs-lookup"><span data-stu-id="a57d1-129">Set to true if the attachment appears inline in the body of the embedding object.</span></span>|
|<span data-ttu-id="a57d1-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a57d1-130">lastModifiedDateTime</span></span>|<span data-ttu-id="a57d1-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a57d1-131">DateTimeOffset</span></span>|<span data-ttu-id="a57d1-p102">Дата и время последнего изменения вложения. Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a57d1-p102">The date and time when the attachment was last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a57d1-135">name</span><span class="sxs-lookup"><span data-stu-id="a57d1-135">name</span></span>|<span data-ttu-id="a57d1-136">String</span><span class="sxs-lookup"><span data-stu-id="a57d1-136">String</span></span>|<span data-ttu-id="a57d1-p103">Текст, который отображается под значком, представляет внедренное вложение. Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="a57d1-p103">The text that is displayed below the icon representing the embedded attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="a57d1-139">size</span><span class="sxs-lookup"><span data-stu-id="a57d1-139">size</span></span>|<span data-ttu-id="a57d1-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a57d1-140">Int32</span></span>|<span data-ttu-id="a57d1-141">Объем метаданных, которые хранятся в сообщении с вложением (в байтах).</span><span class="sxs-lookup"><span data-stu-id="a57d1-141">The size of the metadata that is stored on the message for the attachment in bytes.</span></span> <span data-ttu-id="a57d1-142">Это значение не отображает фактический размер файла.</span><span class="sxs-lookup"><span data-stu-id="a57d1-142">This value does not indicate the size of the actual file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a57d1-143">Отношения</span><span class="sxs-lookup"><span data-stu-id="a57d1-143">Relationships</span></span>
<span data-ttu-id="a57d1-144">Нет</span><span class="sxs-lookup"><span data-stu-id="a57d1-144">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="a57d1-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a57d1-145">JSON representation</span></span>

<span data-ttu-id="a57d1-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a57d1-146">Here is a JSON representation of the resource</span></span>

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
