---
title: Тип ресурса fileAttachment
description: 'Файл (например, текстовый файл или документ Word), вложенный в сведения о событии, сообщение или запись. **contentBytes** '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4975e9b46a4b55429906fbcd9b7b23f8774a47e9
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036202"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="3f66b-104">Тип ресурса fileAttachment</span><span class="sxs-lookup"><span data-stu-id="3f66b-104">fileAttachment resource type</span></span>

<span data-ttu-id="3f66b-p102">Файл (например, текстовый файл или документ Word), вложенный в сведения о пользовательском [событии](../resources/event.md), [сообщение](../resources/message.md) или [запись](../resources/post.md). Свойство **contentBytes** включает содержимое файла в кодировке base64.</span><span class="sxs-lookup"><span data-stu-id="3f66b-p102">A file (such as a text file or Word document) attached to an event, message or post. The  contentBytes property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="3f66b-107">При создании вложенного файла включите в текст запроса следующее:</span><span class="sxs-lookup"><span data-stu-id="3f66b-107">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="3f66b-108">Обязательные свойства **name** и **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="3f66b-108">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="3f66b-109">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="3f66b-109">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3f66b-110">Методы</span><span class="sxs-lookup"><span data-stu-id="3f66b-110">Methods</span></span>

| <span data-ttu-id="3f66b-111">Метод</span><span class="sxs-lookup"><span data-stu-id="3f66b-111">Method</span></span>       | <span data-ttu-id="3f66b-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3f66b-112">Return Type</span></span>  |<span data-ttu-id="3f66b-113">Описание</span><span class="sxs-lookup"><span data-stu-id="3f66b-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3f66b-114">Получение</span><span class="sxs-lookup"><span data-stu-id="3f66b-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="3f66b-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="3f66b-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="3f66b-116">Чтение свойств, связей или необработанного содержимого объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="3f66b-116">Read properties, relationships, or raw contents of a fileAttachment object.</span></span>|
|[<span data-ttu-id="3f66b-117">Удаление</span><span class="sxs-lookup"><span data-stu-id="3f66b-117">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="3f66b-118">Нет</span><span class="sxs-lookup"><span data-stu-id="3f66b-118">None</span></span> |<span data-ttu-id="3f66b-119">Удаление объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="3f66b-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3f66b-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f66b-120">Properties</span></span>
| <span data-ttu-id="3f66b-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f66b-121">Property</span></span>     | <span data-ttu-id="3f66b-122">Тип</span><span class="sxs-lookup"><span data-stu-id="3f66b-122">Type</span></span>   |<span data-ttu-id="3f66b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3f66b-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f66b-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="3f66b-124">contentBytes</span></span>|<span data-ttu-id="3f66b-125">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="3f66b-125">Edm.Binary</span></span>|<span data-ttu-id="3f66b-126">Содержимое файла в кодировке base64.</span><span class="sxs-lookup"><span data-stu-id="3f66b-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="3f66b-127">contentId</span><span class="sxs-lookup"><span data-stu-id="3f66b-127">contentId</span></span>|<span data-ttu-id="3f66b-128">String</span><span class="sxs-lookup"><span data-stu-id="3f66b-128">String</span></span>|<span data-ttu-id="3f66b-129">Идентификатор вложения в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f66b-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="3f66b-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="3f66b-130">contentLocation</span></span>|<span data-ttu-id="3f66b-131">String</span><span class="sxs-lookup"><span data-stu-id="3f66b-131">String</span></span>|<span data-ttu-id="3f66b-132">Не используйте это свойство, так как оно не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f66b-132">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="3f66b-133">contentType</span><span class="sxs-lookup"><span data-stu-id="3f66b-133">contentType</span></span>|<span data-ttu-id="3f66b-134">String</span><span class="sxs-lookup"><span data-stu-id="3f66b-134">String</span></span>|<span data-ttu-id="3f66b-135">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="3f66b-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="3f66b-136">id</span><span class="sxs-lookup"><span data-stu-id="3f66b-136">id</span></span>|<span data-ttu-id="3f66b-137">String</span><span class="sxs-lookup"><span data-stu-id="3f66b-137">String</span></span>|<span data-ttu-id="3f66b-138">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="3f66b-138">The attachment ID.</span></span>|
|<span data-ttu-id="3f66b-139">isInline</span><span class="sxs-lookup"><span data-stu-id="3f66b-139">isInline</span></span>|<span data-ttu-id="3f66b-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f66b-140">Boolean</span></span>|<span data-ttu-id="3f66b-141">Задано значение true, если это встроенное вложение.</span><span class="sxs-lookup"><span data-stu-id="3f66b-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="3f66b-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f66b-142">lastModifiedDateTime</span></span>|<span data-ttu-id="3f66b-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f66b-143">DateTimeOffset</span></span>|<span data-ttu-id="3f66b-144">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="3f66b-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="3f66b-145">name</span><span class="sxs-lookup"><span data-stu-id="3f66b-145">name</span></span>|<span data-ttu-id="3f66b-146">String</span><span class="sxs-lookup"><span data-stu-id="3f66b-146">String</span></span>|<span data-ttu-id="3f66b-147">Имя, представляющее текст, который отображается под значком, представляющим внедренное вложение. Оно может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="3f66b-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="3f66b-148">size</span><span class="sxs-lookup"><span data-stu-id="3f66b-148">size</span></span>|<span data-ttu-id="3f66b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3f66b-149">Int32</span></span>|<span data-ttu-id="3f66b-150">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="3f66b-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f66b-151">Связи</span><span class="sxs-lookup"><span data-stu-id="3f66b-151">Relationships</span></span>
<span data-ttu-id="3f66b-152">Нет</span><span class="sxs-lookup"><span data-stu-id="3f66b-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3f66b-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f66b-153">JSON representation</span></span>

<span data-ttu-id="3f66b-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f66b-154">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "string (binary)",
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
