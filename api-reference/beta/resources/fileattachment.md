---
title: Тип ресурса fileAttachment
description: Файл (например, текстовый файл или документ Word), вложенный в событие,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 1ef32e91897ac322b84922012df47c168094f57d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135648"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="e87c4-103">Тип ресурса fileAttachment</span><span class="sxs-lookup"><span data-stu-id="e87c4-103">fileAttachment resource type</span></span>

<span data-ttu-id="e87c4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e87c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="e87c4-105">Файл (например, текстовый файл или документ Word), вложенный в событие [пользователя,](../resources/event.md) [сообщение,](../resources/message.md) [задачу Outlook](../resources/outlooktask.md)или [post.](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="e87c4-105">A file (such as a text file or Word document) attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="e87c4-106">При создании вложенного файла включите в текст запроса следующее:</span><span class="sxs-lookup"><span data-stu-id="e87c4-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="e87c4-107">Обязательные свойства **name** и **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="e87c4-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="e87c4-108">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="e87c4-108">Derived from [attachment](attachment.md).</span></span>

> [!NOTE]
> <span data-ttu-id="e87c4-109">Не забудьте закодировать содержимое файла в base64 перед назначением его **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="e87c4-109">Make sure to encode the file content in base64 before assigning it to **contentBytes**.</span></span>

## <a name="methods"></a><span data-ttu-id="e87c4-110">Методы</span><span class="sxs-lookup"><span data-stu-id="e87c4-110">Methods</span></span>

| <span data-ttu-id="e87c4-111">Метод</span><span class="sxs-lookup"><span data-stu-id="e87c4-111">Method</span></span>       | <span data-ttu-id="e87c4-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e87c4-112">Return Type</span></span>  |<span data-ttu-id="e87c4-113">Описание</span><span class="sxs-lookup"><span data-stu-id="e87c4-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e87c4-114">Получение</span><span class="sxs-lookup"><span data-stu-id="e87c4-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="e87c4-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="e87c4-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="e87c4-116">Чтение свойств, связей или необработанных содержимого объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="e87c4-116">Read the properties, relationships, or raw contents of a fileAttachment object.</span></span>|
|[<span data-ttu-id="e87c4-117">Delete</span><span class="sxs-lookup"><span data-stu-id="e87c4-117">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="e87c4-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e87c4-118">None</span></span> |<span data-ttu-id="e87c4-119">Удаление объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="e87c4-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e87c4-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="e87c4-120">Properties</span></span>
| <span data-ttu-id="e87c4-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="e87c4-121">Property</span></span>     | <span data-ttu-id="e87c4-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e87c4-122">Type</span></span>   |<span data-ttu-id="e87c4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e87c4-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e87c4-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="e87c4-124">contentBytes</span></span>|<span data-ttu-id="e87c4-125">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="e87c4-125">Edm.Binary</span></span>|<span data-ttu-id="e87c4-126">Содержимое файла в кодировке base64.</span><span class="sxs-lookup"><span data-stu-id="e87c4-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="e87c4-127">contentId</span><span class="sxs-lookup"><span data-stu-id="e87c4-127">contentId</span></span>|<span data-ttu-id="e87c4-128">String</span><span class="sxs-lookup"><span data-stu-id="e87c4-128">String</span></span>|<span data-ttu-id="e87c4-129">Идентификатор вложения в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e87c4-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="e87c4-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="e87c4-130">contentLocation</span></span>|<span data-ttu-id="e87c4-131">String</span><span class="sxs-lookup"><span data-stu-id="e87c4-131">String</span></span>|<span data-ttu-id="e87c4-132">Не используйте это свойство, так как оно не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e87c4-132">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="e87c4-133">contentType</span><span class="sxs-lookup"><span data-stu-id="e87c4-133">contentType</span></span>|<span data-ttu-id="e87c4-134">String</span><span class="sxs-lookup"><span data-stu-id="e87c4-134">String</span></span>|<span data-ttu-id="e87c4-135">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="e87c4-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="e87c4-136">id</span><span class="sxs-lookup"><span data-stu-id="e87c4-136">id</span></span>|<span data-ttu-id="e87c4-137">String</span><span class="sxs-lookup"><span data-stu-id="e87c4-137">String</span></span>|<span data-ttu-id="e87c4-138">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="e87c4-138">The attachment ID.</span></span>|
|<span data-ttu-id="e87c4-139">isInline</span><span class="sxs-lookup"><span data-stu-id="e87c4-139">isInline</span></span>|<span data-ttu-id="e87c4-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="e87c4-140">Boolean</span></span>|<span data-ttu-id="e87c4-141">Задано значение true, если это встроенное вложение.</span><span class="sxs-lookup"><span data-stu-id="e87c4-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="e87c4-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e87c4-142">lastModifiedDateTime</span></span>|<span data-ttu-id="e87c4-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e87c4-143">DateTimeOffset</span></span>|<span data-ttu-id="e87c4-144">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="e87c4-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="e87c4-145">name</span><span class="sxs-lookup"><span data-stu-id="e87c4-145">name</span></span>|<span data-ttu-id="e87c4-146">String</span><span class="sxs-lookup"><span data-stu-id="e87c4-146">String</span></span>|<span data-ttu-id="e87c4-147">Имя, представляющее текст, который отображается под значком, представляющим внедренное вложение. Оно может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="e87c4-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="e87c4-148">size</span><span class="sxs-lookup"><span data-stu-id="e87c4-148">size</span></span>|<span data-ttu-id="e87c4-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e87c4-149">Int32</span></span>|<span data-ttu-id="e87c4-150">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="e87c4-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e87c4-151">Связи</span><span class="sxs-lookup"><span data-stu-id="e87c4-151">Relationships</span></span>
<span data-ttu-id="e87c4-152">Нет</span><span class="sxs-lookup"><span data-stu-id="e87c4-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e87c4-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e87c4-153">JSON representation</span></span>

<span data-ttu-id="e87c4-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e87c4-154">Here is a JSON representation of the resource</span></span>

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


