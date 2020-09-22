---
title: Тип ресурса fileAttachment
description: Файл (например, текстовый файл или документ Word), присоединенный к событию,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: a850e05622b22bf05dfec1011cd4371cbc9e7cc4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058466"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="27f60-103">Тип ресурса fileAttachment</span><span class="sxs-lookup"><span data-stu-id="27f60-103">fileAttachment resource type</span></span>

<span data-ttu-id="27f60-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27f60-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="27f60-105">Файл (например, текстовый файл или документ Word), присоединенный к пользовательскому [событию](../resources/event.md), [сообщению](../resources/message.md), [задаче Outlook](../resources/outlooktask.md)или [POST](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="27f60-105">A file (such as a text file or Word document) attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="27f60-106">При создании вложенного файла включите в текст запроса следующее:</span><span class="sxs-lookup"><span data-stu-id="27f60-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="27f60-107">Обязательные свойства **name** и **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="27f60-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="27f60-108">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="27f60-108">Derived from [attachment](attachment.md).</span></span>

> [!NOTE]
> <span data-ttu-id="27f60-109">Не забудьте закодировать содержимое файла в base64 перед назначением его **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="27f60-109">Make sure to encode the file content in base64 before assigning it to **contentBytes**.</span></span>

## <a name="methods"></a><span data-ttu-id="27f60-110">Методы</span><span class="sxs-lookup"><span data-stu-id="27f60-110">Methods</span></span>

| <span data-ttu-id="27f60-111">Метод</span><span class="sxs-lookup"><span data-stu-id="27f60-111">Method</span></span>       | <span data-ttu-id="27f60-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="27f60-112">Return Type</span></span>  |<span data-ttu-id="27f60-113">Описание</span><span class="sxs-lookup"><span data-stu-id="27f60-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="27f60-114">Получение</span><span class="sxs-lookup"><span data-stu-id="27f60-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="27f60-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="27f60-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="27f60-116">Чтение свойств, связей или необработанного содержимого объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="27f60-116">Read the properties, relationships, or raw contents of a fileAttachment object.</span></span>|
|[<span data-ttu-id="27f60-117">Удаление</span><span class="sxs-lookup"><span data-stu-id="27f60-117">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="27f60-118">Нет</span><span class="sxs-lookup"><span data-stu-id="27f60-118">None</span></span> |<span data-ttu-id="27f60-119">Удаление объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="27f60-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="27f60-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="27f60-120">Properties</span></span>
| <span data-ttu-id="27f60-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="27f60-121">Property</span></span>     | <span data-ttu-id="27f60-122">Тип</span><span class="sxs-lookup"><span data-stu-id="27f60-122">Type</span></span>   |<span data-ttu-id="27f60-123">Описание</span><span class="sxs-lookup"><span data-stu-id="27f60-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27f60-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="27f60-124">contentBytes</span></span>|<span data-ttu-id="27f60-125">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="27f60-125">Edm.Binary</span></span>|<span data-ttu-id="27f60-126">Содержимое файла в кодировке base64.</span><span class="sxs-lookup"><span data-stu-id="27f60-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="27f60-127">contentId</span><span class="sxs-lookup"><span data-stu-id="27f60-127">contentId</span></span>|<span data-ttu-id="27f60-128">String</span><span class="sxs-lookup"><span data-stu-id="27f60-128">String</span></span>|<span data-ttu-id="27f60-129">Идентификатор вложения в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="27f60-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="27f60-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="27f60-130">contentLocation</span></span>|<span data-ttu-id="27f60-131">String</span><span class="sxs-lookup"><span data-stu-id="27f60-131">String</span></span>|<span data-ttu-id="27f60-132">Не используйте это свойство, так как оно не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27f60-132">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="27f60-133">contentType</span><span class="sxs-lookup"><span data-stu-id="27f60-133">contentType</span></span>|<span data-ttu-id="27f60-134">String</span><span class="sxs-lookup"><span data-stu-id="27f60-134">String</span></span>|<span data-ttu-id="27f60-135">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="27f60-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="27f60-136">id</span><span class="sxs-lookup"><span data-stu-id="27f60-136">id</span></span>|<span data-ttu-id="27f60-137">String</span><span class="sxs-lookup"><span data-stu-id="27f60-137">String</span></span>|<span data-ttu-id="27f60-138">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="27f60-138">The attachment ID.</span></span>|
|<span data-ttu-id="27f60-139">isInline</span><span class="sxs-lookup"><span data-stu-id="27f60-139">isInline</span></span>|<span data-ttu-id="27f60-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="27f60-140">Boolean</span></span>|<span data-ttu-id="27f60-141">Задано значение true, если это встроенное вложение.</span><span class="sxs-lookup"><span data-stu-id="27f60-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="27f60-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27f60-142">lastModifiedDateTime</span></span>|<span data-ttu-id="27f60-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27f60-143">DateTimeOffset</span></span>|<span data-ttu-id="27f60-144">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="27f60-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="27f60-145">name</span><span class="sxs-lookup"><span data-stu-id="27f60-145">name</span></span>|<span data-ttu-id="27f60-146">String</span><span class="sxs-lookup"><span data-stu-id="27f60-146">String</span></span>|<span data-ttu-id="27f60-147">Имя, представляющее текст, который отображается под значком, представляющим внедренное вложение. Оно может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="27f60-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="27f60-148">size</span><span class="sxs-lookup"><span data-stu-id="27f60-148">size</span></span>|<span data-ttu-id="27f60-149">Int32</span><span class="sxs-lookup"><span data-stu-id="27f60-149">Int32</span></span>|<span data-ttu-id="27f60-150">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="27f60-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27f60-151">Связи</span><span class="sxs-lookup"><span data-stu-id="27f60-151">Relationships</span></span>
<span data-ttu-id="27f60-152">Нет</span><span class="sxs-lookup"><span data-stu-id="27f60-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="27f60-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27f60-153">JSON representation</span></span>

<span data-ttu-id="27f60-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27f60-154">Here is a JSON representation of the resource</span></span>

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


