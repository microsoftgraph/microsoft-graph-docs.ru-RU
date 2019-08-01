---
title: Тип ресурса fileAttachment
description: 'Файл (например, текстовый файл или документ Word), вложенный в сведения о событии, сообщение или запись. **contentBytes** '
localization_priority: Priority
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7e80a4599d79d17829f2bb07bb61d4adf60df607
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032510"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="e6b0f-104">Тип ресурса fileAttachment</span><span class="sxs-lookup"><span data-stu-id="e6b0f-104">fileAttachment resource type</span></span>

<span data-ttu-id="e6b0f-p102">Файл (например, текстовый файл или документ Word), вложенный в сведения о событии, сообщение или запись. Свойство **contentBytes** включает содержимое файла в кодировке Base 64.</span><span class="sxs-lookup"><span data-stu-id="e6b0f-p102">A file (such as a text file or Word document) attached to an event, message or post. The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="e6b0f-107">При создании вложенного файла включите в текст запроса следующее:</span><span class="sxs-lookup"><span data-stu-id="e6b0f-107">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="e6b0f-108">Обязательные свойства **name** и **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="e6b0f-108">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="e6b0f-109">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="e6b0f-109">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e6b0f-110">Методы</span><span class="sxs-lookup"><span data-stu-id="e6b0f-110">Methods</span></span>

| <span data-ttu-id="e6b0f-111">Метод</span><span class="sxs-lookup"><span data-stu-id="e6b0f-111">Method</span></span>       | <span data-ttu-id="e6b0f-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e6b0f-112">Return Type</span></span>  |<span data-ttu-id="e6b0f-113">Описание</span><span class="sxs-lookup"><span data-stu-id="e6b0f-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e6b0f-114">Получение</span><span class="sxs-lookup"><span data-stu-id="e6b0f-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="e6b0f-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="e6b0f-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="e6b0f-116">Чтение свойств и связей объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="e6b0f-116">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="e6b0f-117">Удаление</span><span class="sxs-lookup"><span data-stu-id="e6b0f-117">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="e6b0f-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e6b0f-118">None</span></span> |<span data-ttu-id="e6b0f-119">Удаление объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="e6b0f-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e6b0f-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6b0f-120">Properties</span></span>
| <span data-ttu-id="e6b0f-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6b0f-121">Property</span></span>     | <span data-ttu-id="e6b0f-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e6b0f-122">Type</span></span>   |<span data-ttu-id="e6b0f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e6b0f-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6b0f-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="e6b0f-124">contentBytes</span></span>|<span data-ttu-id="e6b0f-125">Двоичный</span><span class="sxs-lookup"><span data-stu-id="e6b0f-125">Binary</span></span>|<span data-ttu-id="e6b0f-126">Содержимое файла в кодировке base64.</span><span class="sxs-lookup"><span data-stu-id="e6b0f-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="e6b0f-127">contentId</span><span class="sxs-lookup"><span data-stu-id="e6b0f-127">contentId</span></span>|<span data-ttu-id="e6b0f-128">String</span><span class="sxs-lookup"><span data-stu-id="e6b0f-128">String</span></span>|<span data-ttu-id="e6b0f-129">Идентификатор вложения в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e6b0f-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="e6b0f-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="e6b0f-130">contentLocation</span></span>|<span data-ttu-id="e6b0f-131">String</span><span class="sxs-lookup"><span data-stu-id="e6b0f-131">String</span></span>|<span data-ttu-id="e6b0f-132">Не используйте это свойство, так как оно не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6b0f-132">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="e6b0f-133">contentType</span><span class="sxs-lookup"><span data-stu-id="e6b0f-133">contentType</span></span>|<span data-ttu-id="e6b0f-134">String</span><span class="sxs-lookup"><span data-stu-id="e6b0f-134">String</span></span>|<span data-ttu-id="e6b0f-135">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="e6b0f-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="e6b0f-136">id</span><span class="sxs-lookup"><span data-stu-id="e6b0f-136">id</span></span>|<span data-ttu-id="e6b0f-137">String</span><span class="sxs-lookup"><span data-stu-id="e6b0f-137">String</span></span>|<span data-ttu-id="e6b0f-138">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="e6b0f-138">The attachment ID.</span></span>|
|<span data-ttu-id="e6b0f-139">isInline</span><span class="sxs-lookup"><span data-stu-id="e6b0f-139">isInline</span></span>|<span data-ttu-id="e6b0f-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6b0f-140">Boolean</span></span>|<span data-ttu-id="e6b0f-141">Задано значение true, если это встроенное вложение.</span><span class="sxs-lookup"><span data-stu-id="e6b0f-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="e6b0f-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6b0f-142">lastModifiedDateTime</span></span>|<span data-ttu-id="e6b0f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6b0f-143">DateTimeOffset</span></span>|<span data-ttu-id="e6b0f-144">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="e6b0f-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="e6b0f-145">name</span><span class="sxs-lookup"><span data-stu-id="e6b0f-145">name</span></span>|<span data-ttu-id="e6b0f-146">String</span><span class="sxs-lookup"><span data-stu-id="e6b0f-146">String</span></span>|<span data-ttu-id="e6b0f-147">Имя, представляющее текст, который отображается под значком, представляющим внедренное вложение. Оно может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="e6b0f-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="e6b0f-148">size</span><span class="sxs-lookup"><span data-stu-id="e6b0f-148">size</span></span>|<span data-ttu-id="e6b0f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e6b0f-149">Int32</span></span>|<span data-ttu-id="e6b0f-150">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="e6b0f-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6b0f-151">Связи</span><span class="sxs-lookup"><span data-stu-id="e6b0f-151">Relationships</span></span>
<span data-ttu-id="e6b0f-152">Нет</span><span class="sxs-lookup"><span data-stu-id="e6b0f-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e6b0f-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6b0f-153">JSON representation</span></span>

<span data-ttu-id="e6b0f-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6b0f-154">Here is a JSON representation of the resource</span></span>

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
