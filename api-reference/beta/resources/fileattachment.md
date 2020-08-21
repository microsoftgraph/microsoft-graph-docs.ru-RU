---
title: Тип ресурса fileAttachment
description: Файл (например, текстовый файл или документ Word), вложенный в событие,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 770cb2750df46243d6050832feeca301549b2c76
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849489"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="1a4c0-103">Тип ресурса fileAttachment</span><span class="sxs-lookup"><span data-stu-id="1a4c0-103">fileAttachment resource type</span></span>

<span data-ttu-id="1a4c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a4c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="1a4c0-105">Файл (например, текстовый файл или документ Word), вложенный в [событие](../resources/event.md)пользователя, [сообщение,](../resources/message.md) [задачу Outlook](../resources/outlooktask.md)или [запись.](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="1a4c0-105">A file (such as a text file or Word document) attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="1a4c0-106">При создании вложенного файла включите в текст запроса следующее:</span><span class="sxs-lookup"><span data-stu-id="1a4c0-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="1a4c0-107">Обязательные свойства **name** и **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="1a4c0-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="1a4c0-108">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="1a4c0-108">Derived from [attachment](attachment.md).</span></span>

> [!NOTE]
> <span data-ttu-id="1a4c0-109">Не забудьте закодировать содержимое файла в base64 перед назначением его **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="1a4c0-109">Make sure to encode the file content in base64 before assigning it to **contentBytes**.</span></span>

## <a name="methods"></a><span data-ttu-id="1a4c0-110">Методы</span><span class="sxs-lookup"><span data-stu-id="1a4c0-110">Methods</span></span>

| <span data-ttu-id="1a4c0-111">Метод</span><span class="sxs-lookup"><span data-stu-id="1a4c0-111">Method</span></span>       | <span data-ttu-id="1a4c0-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1a4c0-112">Return Type</span></span>  |<span data-ttu-id="1a4c0-113">Описание</span><span class="sxs-lookup"><span data-stu-id="1a4c0-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1a4c0-114">Получение</span><span class="sxs-lookup"><span data-stu-id="1a4c0-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="1a4c0-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="1a4c0-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="1a4c0-116">Чтение свойств, связей или необработанного содержимого объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="1a4c0-116">Read the properties, relationships, or raw contents of a fileAttachment object.</span></span>|
|<span data-ttu-id="1a4c0-117">[удаление](../api/attachment-delete.md);</span><span class="sxs-lookup"><span data-stu-id="1a4c0-117">[Delete](../api/attachment-delete.md)</span></span> | <span data-ttu-id="1a4c0-118">Нет</span><span class="sxs-lookup"><span data-stu-id="1a4c0-118">None</span></span> |<span data-ttu-id="1a4c0-119">Удаление объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="1a4c0-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1a4c0-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a4c0-120">Properties</span></span>
| <span data-ttu-id="1a4c0-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a4c0-121">Property</span></span>     | <span data-ttu-id="1a4c0-122">Тип</span><span class="sxs-lookup"><span data-stu-id="1a4c0-122">Type</span></span>   |<span data-ttu-id="1a4c0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1a4c0-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a4c0-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="1a4c0-124">contentBytes</span></span>|<span data-ttu-id="1a4c0-125">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="1a4c0-125">Edm.Binary</span></span>|<span data-ttu-id="1a4c0-126">Содержимое файла в кодировке base64.</span><span class="sxs-lookup"><span data-stu-id="1a4c0-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="1a4c0-127">contentId</span><span class="sxs-lookup"><span data-stu-id="1a4c0-127">contentId</span></span>|<span data-ttu-id="1a4c0-128">String</span><span class="sxs-lookup"><span data-stu-id="1a4c0-128">String</span></span>|<span data-ttu-id="1a4c0-129">Идентификатор вложения в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a4c0-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="1a4c0-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="1a4c0-130">contentLocation</span></span>|<span data-ttu-id="1a4c0-131">String</span><span class="sxs-lookup"><span data-stu-id="1a4c0-131">String</span></span>|<span data-ttu-id="1a4c0-132">Не используйте это свойство, так как оно не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a4c0-132">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="1a4c0-133">contentType</span><span class="sxs-lookup"><span data-stu-id="1a4c0-133">contentType</span></span>|<span data-ttu-id="1a4c0-134">String</span><span class="sxs-lookup"><span data-stu-id="1a4c0-134">String</span></span>|<span data-ttu-id="1a4c0-135">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="1a4c0-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="1a4c0-136">id</span><span class="sxs-lookup"><span data-stu-id="1a4c0-136">id</span></span>|<span data-ttu-id="1a4c0-137">String</span><span class="sxs-lookup"><span data-stu-id="1a4c0-137">String</span></span>|<span data-ttu-id="1a4c0-138">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="1a4c0-138">The attachment ID.</span></span>|
|<span data-ttu-id="1a4c0-139">isInline</span><span class="sxs-lookup"><span data-stu-id="1a4c0-139">isInline</span></span>|<span data-ttu-id="1a4c0-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a4c0-140">Boolean</span></span>|<span data-ttu-id="1a4c0-141">Задано значение true, если это встроенное вложение.</span><span class="sxs-lookup"><span data-stu-id="1a4c0-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="1a4c0-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a4c0-142">lastModifiedDateTime</span></span>|<span data-ttu-id="1a4c0-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a4c0-143">DateTimeOffset</span></span>|<span data-ttu-id="1a4c0-144">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="1a4c0-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="1a4c0-145">name</span><span class="sxs-lookup"><span data-stu-id="1a4c0-145">name</span></span>|<span data-ttu-id="1a4c0-146">String</span><span class="sxs-lookup"><span data-stu-id="1a4c0-146">String</span></span>|<span data-ttu-id="1a4c0-147">Имя, представляющее текст, который отображается под значком, представляющим внедренное вложение. Оно может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="1a4c0-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="1a4c0-148">size</span><span class="sxs-lookup"><span data-stu-id="1a4c0-148">size</span></span>|<span data-ttu-id="1a4c0-149">Int32</span><span class="sxs-lookup"><span data-stu-id="1a4c0-149">Int32</span></span>|<span data-ttu-id="1a4c0-150">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="1a4c0-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a4c0-151">Связи</span><span class="sxs-lookup"><span data-stu-id="1a4c0-151">Relationships</span></span>
<span data-ttu-id="1a4c0-152">Нет</span><span class="sxs-lookup"><span data-stu-id="1a4c0-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1a4c0-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a4c0-153">JSON representation</span></span>

<span data-ttu-id="1a4c0-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a4c0-154">Here is a JSON representation of the resource</span></span>

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
