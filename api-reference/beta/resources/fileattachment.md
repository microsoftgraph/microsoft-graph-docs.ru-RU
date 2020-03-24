---
title: Тип ресурса fileAttachment
description: Файл (например, текстовый файл или документ Word), присоединенный к событию,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: e14b98c5ee3302d5b19bc7ad92187112b6d8c80b
ms.sourcegitcommit: d0f88dcb7f4c72196c45a00cccbb9fc30b715637
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/24/2020
ms.locfileid: "42926801"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="ec5f0-103">Тип ресурса fileAttachment</span><span class="sxs-lookup"><span data-stu-id="ec5f0-103">fileAttachment resource type</span></span>

<span data-ttu-id="ec5f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec5f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec5f0-105">Файл (например, текстовый файл или документ Word), присоединенный к пользовательскому [событию](../resources/event.md), [сообщению](../resources/message.md), [задаче Outlook](../resources/outlooktask.md)или [POST](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="ec5f0-105">A file (such as a text file or Word document) attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="ec5f0-106">При создании вложенного файла включите в текст запроса следующее:</span><span class="sxs-lookup"><span data-stu-id="ec5f0-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="ec5f0-107">Обязательные свойства **name** и **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="ec5f0-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="ec5f0-108">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="ec5f0-108">Derived from [attachment](attachment.md).</span></span>

> [!NOTE]
> <span data-ttu-id="ec5f0-109">Перед назначением файла в **contentBytes**необходимо закодировать его в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="ec5f0-109">Make sure to encode the file content in base64 before assigning it to **contentBytes**.</span></span>

## <a name="methods"></a><span data-ttu-id="ec5f0-110">Методы</span><span class="sxs-lookup"><span data-stu-id="ec5f0-110">Methods</span></span>

| <span data-ttu-id="ec5f0-111">Метод</span><span class="sxs-lookup"><span data-stu-id="ec5f0-111">Method</span></span>       | <span data-ttu-id="ec5f0-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ec5f0-112">Return Type</span></span>  |<span data-ttu-id="ec5f0-113">Описание</span><span class="sxs-lookup"><span data-stu-id="ec5f0-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ec5f0-114">Получение</span><span class="sxs-lookup"><span data-stu-id="ec5f0-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="ec5f0-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="ec5f0-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="ec5f0-116">Чтение свойств, связей или необработанного содержимого объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="ec5f0-116">Read the properties, relationships, or raw contents of a fileAttachment object.</span></span>|
|<span data-ttu-id="ec5f0-117">[удаление](../api/attachment-delete.md);</span><span class="sxs-lookup"><span data-stu-id="ec5f0-117">[Delete](../api/attachment-delete.md)</span></span> | <span data-ttu-id="ec5f0-118">Нет</span><span class="sxs-lookup"><span data-stu-id="ec5f0-118">None</span></span> |<span data-ttu-id="ec5f0-119">Удаление объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="ec5f0-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ec5f0-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec5f0-120">Properties</span></span>
| <span data-ttu-id="ec5f0-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec5f0-121">Property</span></span>     | <span data-ttu-id="ec5f0-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ec5f0-122">Type</span></span>   |<span data-ttu-id="ec5f0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ec5f0-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec5f0-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="ec5f0-124">contentBytes</span></span>|<span data-ttu-id="ec5f0-125">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="ec5f0-125">Edm.Binary</span></span>|<span data-ttu-id="ec5f0-126">Содержимое файла в кодировке base64.</span><span class="sxs-lookup"><span data-stu-id="ec5f0-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="ec5f0-127">contentId</span><span class="sxs-lookup"><span data-stu-id="ec5f0-127">contentId</span></span>|<span data-ttu-id="ec5f0-128">String</span><span class="sxs-lookup"><span data-stu-id="ec5f0-128">String</span></span>|<span data-ttu-id="ec5f0-129">Идентификатор вложения в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec5f0-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="ec5f0-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="ec5f0-130">contentLocation</span></span>|<span data-ttu-id="ec5f0-131">String</span><span class="sxs-lookup"><span data-stu-id="ec5f0-131">String</span></span>|<span data-ttu-id="ec5f0-132">Не используйте это свойство, так как оно не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec5f0-132">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="ec5f0-133">contentType</span><span class="sxs-lookup"><span data-stu-id="ec5f0-133">contentType</span></span>|<span data-ttu-id="ec5f0-134">String</span><span class="sxs-lookup"><span data-stu-id="ec5f0-134">String</span></span>|<span data-ttu-id="ec5f0-135">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="ec5f0-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="ec5f0-136">id</span><span class="sxs-lookup"><span data-stu-id="ec5f0-136">id</span></span>|<span data-ttu-id="ec5f0-137">Строка</span><span class="sxs-lookup"><span data-stu-id="ec5f0-137">String</span></span>|<span data-ttu-id="ec5f0-138">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="ec5f0-138">The attachment ID.</span></span>|
|<span data-ttu-id="ec5f0-139">isInline</span><span class="sxs-lookup"><span data-stu-id="ec5f0-139">isInline</span></span>|<span data-ttu-id="ec5f0-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec5f0-140">Boolean</span></span>|<span data-ttu-id="ec5f0-141">Задано значение true, если это встроенное вложение.</span><span class="sxs-lookup"><span data-stu-id="ec5f0-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="ec5f0-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec5f0-142">lastModifiedDateTime</span></span>|<span data-ttu-id="ec5f0-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec5f0-143">DateTimeOffset</span></span>|<span data-ttu-id="ec5f0-144">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="ec5f0-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="ec5f0-145">name</span><span class="sxs-lookup"><span data-stu-id="ec5f0-145">name</span></span>|<span data-ttu-id="ec5f0-146">String</span><span class="sxs-lookup"><span data-stu-id="ec5f0-146">String</span></span>|<span data-ttu-id="ec5f0-147">Имя, представляющее текст, который отображается под значком, представляющим внедренное вложение. Оно может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="ec5f0-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="ec5f0-148">size</span><span class="sxs-lookup"><span data-stu-id="ec5f0-148">size</span></span>|<span data-ttu-id="ec5f0-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ec5f0-149">Int32</span></span>|<span data-ttu-id="ec5f0-150">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="ec5f0-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec5f0-151">Связи</span><span class="sxs-lookup"><span data-stu-id="ec5f0-151">Relationships</span></span>
<span data-ttu-id="ec5f0-152">Нет</span><span class="sxs-lookup"><span data-stu-id="ec5f0-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ec5f0-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ec5f0-153">JSON representation</span></span>

<span data-ttu-id="ec5f0-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec5f0-154">Here is a JSON representation of the resource</span></span>

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
