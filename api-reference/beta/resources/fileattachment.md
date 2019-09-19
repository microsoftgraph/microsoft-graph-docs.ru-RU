---
title: Тип ресурса fileAttachment
description: Файл (например, текстовый файл или документ Word), присоединенный к событию,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 2b73c69b7fdb7099994e9925815d80e2bf99d5f6
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036223"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="4ea85-103">Тип ресурса fileAttachment</span><span class="sxs-lookup"><span data-stu-id="4ea85-103">fileAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ea85-104">Файл (например, текстовый файл или документ Word), присоединенный к пользовательскому [событию](../resources/event.md), [сообщению](../resources/message.md), [задаче Outlook](../resources/outlooktask.md)или [POST](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="4ea85-104">A file (such as a text file or Word document) attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="4ea85-105">Свойство **contentBytes** включает содержимое файла в кодировке Base 64.</span><span class="sxs-lookup"><span data-stu-id="4ea85-105">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="4ea85-106">При создании вложенного файла включите в текст запроса следующее:</span><span class="sxs-lookup"><span data-stu-id="4ea85-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="4ea85-107">Обязательные свойства **name** и **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="4ea85-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="4ea85-108">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="4ea85-108">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4ea85-109">Методы</span><span class="sxs-lookup"><span data-stu-id="4ea85-109">Methods</span></span>

| <span data-ttu-id="4ea85-110">Метод</span><span class="sxs-lookup"><span data-stu-id="4ea85-110">Method</span></span>       | <span data-ttu-id="4ea85-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4ea85-111">Return Type</span></span>  |<span data-ttu-id="4ea85-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4ea85-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4ea85-113">Получение</span><span class="sxs-lookup"><span data-stu-id="4ea85-113">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="4ea85-114">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="4ea85-114">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="4ea85-115">Чтение свойств, связей или необработанного содержимого объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="4ea85-115">Read the properties, relationships, or raw contents of a fileAttachment object.</span></span>|
|[<span data-ttu-id="4ea85-116">Удаление</span><span class="sxs-lookup"><span data-stu-id="4ea85-116">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="4ea85-117">Нет</span><span class="sxs-lookup"><span data-stu-id="4ea85-117">None</span></span> |<span data-ttu-id="4ea85-118">Удаление объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="4ea85-118">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4ea85-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ea85-119">Properties</span></span>
| <span data-ttu-id="4ea85-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ea85-120">Property</span></span>     | <span data-ttu-id="4ea85-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4ea85-121">Type</span></span>   |<span data-ttu-id="4ea85-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4ea85-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ea85-123">contentBytes</span><span class="sxs-lookup"><span data-stu-id="4ea85-123">contentBytes</span></span>|<span data-ttu-id="4ea85-124">EDM. binary</span><span class="sxs-lookup"><span data-stu-id="4ea85-124">Edm.Binary</span></span>|<span data-ttu-id="4ea85-125">Содержимое файла в кодировке base64.</span><span class="sxs-lookup"><span data-stu-id="4ea85-125">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="4ea85-126">contentId</span><span class="sxs-lookup"><span data-stu-id="4ea85-126">contentId</span></span>|<span data-ttu-id="4ea85-127">String.</span><span class="sxs-lookup"><span data-stu-id="4ea85-127">String</span></span>|<span data-ttu-id="4ea85-128">Идентификатор вложения в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ea85-128">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="4ea85-129">contentLocation</span><span class="sxs-lookup"><span data-stu-id="4ea85-129">contentLocation</span></span>|<span data-ttu-id="4ea85-130">String</span><span class="sxs-lookup"><span data-stu-id="4ea85-130">String</span></span>|<span data-ttu-id="4ea85-131">Не используйте это свойство, так как оно не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ea85-131">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="4ea85-132">contentType</span><span class="sxs-lookup"><span data-stu-id="4ea85-132">contentType</span></span>|<span data-ttu-id="4ea85-133">String</span><span class="sxs-lookup"><span data-stu-id="4ea85-133">String</span></span>|<span data-ttu-id="4ea85-134">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="4ea85-134">The content type of the attachment.</span></span>|
|<span data-ttu-id="4ea85-135">id</span><span class="sxs-lookup"><span data-stu-id="4ea85-135">id</span></span>|<span data-ttu-id="4ea85-136">Строка</span><span class="sxs-lookup"><span data-stu-id="4ea85-136">String</span></span>|<span data-ttu-id="4ea85-137">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="4ea85-137">The attachment ID.</span></span>|
|<span data-ttu-id="4ea85-138">isInline</span><span class="sxs-lookup"><span data-stu-id="4ea85-138">isInline</span></span>|<span data-ttu-id="4ea85-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ea85-139">Boolean</span></span>|<span data-ttu-id="4ea85-140">Задано значение true, если это встроенное вложение.</span><span class="sxs-lookup"><span data-stu-id="4ea85-140">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="4ea85-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ea85-141">lastModifiedDateTime</span></span>|<span data-ttu-id="4ea85-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ea85-142">DateTimeOffset</span></span>|<span data-ttu-id="4ea85-143">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="4ea85-143">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="4ea85-144">name</span><span class="sxs-lookup"><span data-stu-id="4ea85-144">name</span></span>|<span data-ttu-id="4ea85-145">String</span><span class="sxs-lookup"><span data-stu-id="4ea85-145">String</span></span>|<span data-ttu-id="4ea85-146">Имя, представляющее текст, который отображается под значком, представляющим внедренное вложение. Оно может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="4ea85-146">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="4ea85-147">size</span><span class="sxs-lookup"><span data-stu-id="4ea85-147">size</span></span>|<span data-ttu-id="4ea85-148">Int32</span><span class="sxs-lookup"><span data-stu-id="4ea85-148">Int32</span></span>|<span data-ttu-id="4ea85-149">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="4ea85-149">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ea85-150">Связи</span><span class="sxs-lookup"><span data-stu-id="4ea85-150">Relationships</span></span>
<span data-ttu-id="4ea85-151">Нет</span><span class="sxs-lookup"><span data-stu-id="4ea85-151">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4ea85-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ea85-152">JSON representation</span></span>

<span data-ttu-id="4ea85-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ea85-153">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
