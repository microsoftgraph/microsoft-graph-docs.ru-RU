---
title: Тип ресурса fileAttachment
description: 'Файл (например, текстовый файл или документ Word) подключенного к события, сообщение или post. **ContentBytes** '
localization_priority: Priority
ms.openlocfilehash: 81de7a12ca371158d7f6369861a8a197fd544821
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870058"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="dcf14-104">Тип ресурса fileAttachment</span><span class="sxs-lookup"><span data-stu-id="dcf14-104">fileAttachment resource type</span></span>

<span data-ttu-id="dcf14-p102">Файл (например, текстовый файл или документ Word), вложенный в сведения о событии, сообщение или запись. Свойство **contentBytes** включает содержимое файла в кодировке Base 64.</span><span class="sxs-lookup"><span data-stu-id="dcf14-p102">A file (such as a text file or Word document) attached to an event, message or post. The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="dcf14-107">При создании вложенного файла включите в текст запроса следующее:</span><span class="sxs-lookup"><span data-stu-id="dcf14-107">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="dcf14-108">Обязательные свойства **name** и **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="dcf14-108">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="dcf14-109">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="dcf14-109">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dcf14-110">Методы</span><span class="sxs-lookup"><span data-stu-id="dcf14-110">Methods</span></span>

| <span data-ttu-id="dcf14-111">Метод</span><span class="sxs-lookup"><span data-stu-id="dcf14-111">Method</span></span>       | <span data-ttu-id="dcf14-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dcf14-112">Return Type</span></span>  |<span data-ttu-id="dcf14-113">Описание</span><span class="sxs-lookup"><span data-stu-id="dcf14-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dcf14-114">Получение</span><span class="sxs-lookup"><span data-stu-id="dcf14-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="dcf14-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="dcf14-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="dcf14-116">Чтение свойств и связей объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="dcf14-116">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="dcf14-117">Удаление</span><span class="sxs-lookup"><span data-stu-id="dcf14-117">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="dcf14-118">Нет</span><span class="sxs-lookup"><span data-stu-id="dcf14-118">None</span></span> |<span data-ttu-id="dcf14-119">Удаление объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="dcf14-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dcf14-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="dcf14-120">Properties</span></span>
| <span data-ttu-id="dcf14-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="dcf14-121">Property</span></span>     | <span data-ttu-id="dcf14-122">Тип</span><span class="sxs-lookup"><span data-stu-id="dcf14-122">Type</span></span>   |<span data-ttu-id="dcf14-123">Описание</span><span class="sxs-lookup"><span data-stu-id="dcf14-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dcf14-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="dcf14-124">contentBytes</span></span>|<span data-ttu-id="dcf14-125">Двоичный</span><span class="sxs-lookup"><span data-stu-id="dcf14-125">Binary</span></span>|<span data-ttu-id="dcf14-126">Содержимое файла в кодировке base64.</span><span class="sxs-lookup"><span data-stu-id="dcf14-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="dcf14-127">contentId</span><span class="sxs-lookup"><span data-stu-id="dcf14-127">contentId</span></span>|<span data-ttu-id="dcf14-128">String</span><span class="sxs-lookup"><span data-stu-id="dcf14-128">String</span></span>|<span data-ttu-id="dcf14-129">Идентификатор вложения в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="dcf14-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="dcf14-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="dcf14-130">contentLocation</span></span>|<span data-ttu-id="dcf14-131">String</span><span class="sxs-lookup"><span data-stu-id="dcf14-131">String</span></span>|<span data-ttu-id="dcf14-132">Универсальный код ресурса (URI), который соответствует расположению содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="dcf14-132">The Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>|
|<span data-ttu-id="dcf14-133">contentType</span><span class="sxs-lookup"><span data-stu-id="dcf14-133">contentType</span></span>|<span data-ttu-id="dcf14-134">String</span><span class="sxs-lookup"><span data-stu-id="dcf14-134">String</span></span>|<span data-ttu-id="dcf14-135">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="dcf14-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="dcf14-136">id</span><span class="sxs-lookup"><span data-stu-id="dcf14-136">id</span></span>|<span data-ttu-id="dcf14-137">String</span><span class="sxs-lookup"><span data-stu-id="dcf14-137">String</span></span>|<span data-ttu-id="dcf14-138">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="dcf14-138">The attachment ID.</span></span>|
|<span data-ttu-id="dcf14-139">isInline</span><span class="sxs-lookup"><span data-stu-id="dcf14-139">isInline</span></span>|<span data-ttu-id="dcf14-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="dcf14-140">Boolean</span></span>|<span data-ttu-id="dcf14-141">Задано значение true, если это встроенное вложение.</span><span class="sxs-lookup"><span data-stu-id="dcf14-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="dcf14-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dcf14-142">lastModifiedDateTime</span></span>|<span data-ttu-id="dcf14-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dcf14-143">DateTimeOffset</span></span>|<span data-ttu-id="dcf14-144">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="dcf14-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="dcf14-145">name</span><span class="sxs-lookup"><span data-stu-id="dcf14-145">name</span></span>|<span data-ttu-id="dcf14-146">String</span><span class="sxs-lookup"><span data-stu-id="dcf14-146">String</span></span>|<span data-ttu-id="dcf14-147">Имя, представляющее текст, который отображается под значком, представляющим внедренное вложение. Оно может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="dcf14-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="dcf14-148">size</span><span class="sxs-lookup"><span data-stu-id="dcf14-148">size</span></span>|<span data-ttu-id="dcf14-149">Int32</span><span class="sxs-lookup"><span data-stu-id="dcf14-149">Int32</span></span>|<span data-ttu-id="dcf14-150">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="dcf14-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dcf14-151">Связи</span><span class="sxs-lookup"><span data-stu-id="dcf14-151">Relationships</span></span>
<span data-ttu-id="dcf14-152">Нет</span><span class="sxs-lookup"><span data-stu-id="dcf14-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="dcf14-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dcf14-153">JSON representation</span></span>

<span data-ttu-id="dcf14-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dcf14-154">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "binary",
  "contentId": "string",
  "contentLocation": "string",
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
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
