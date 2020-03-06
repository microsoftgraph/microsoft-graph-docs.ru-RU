---
title: Тип ресурса fileAttachment
description: 'Файл (например, текстовый файл или документ Word), вложенный в сведения о событии, сообщение или запись. **contentBytes** '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ad8c1a9ffd4a4b5cc68554505464173a40aafd29
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531433"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="51c1f-104">Тип ресурса fileAttachment</span><span class="sxs-lookup"><span data-stu-id="51c1f-104">fileAttachment resource type</span></span>

<span data-ttu-id="51c1f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51c1f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="51c1f-p102">Файл (например, текстовый файл или документ Word), вложенный в сведения о пользовательском [событии](../resources/event.md), [сообщение](../resources/message.md) или [запись](../resources/post.md). Свойство **contentBytes** включает содержимое файла в кодировке base64.</span><span class="sxs-lookup"><span data-stu-id="51c1f-p102">A file (such as a text file or Word document) attached to a user [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md). The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="51c1f-108">При создании вложенного файла включите в текст запроса следующее:</span><span class="sxs-lookup"><span data-stu-id="51c1f-108">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="51c1f-109">Обязательные свойства **name** и **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="51c1f-109">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="51c1f-110">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="51c1f-110">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="51c1f-111">Методы</span><span class="sxs-lookup"><span data-stu-id="51c1f-111">Methods</span></span>

| <span data-ttu-id="51c1f-112">Метод</span><span class="sxs-lookup"><span data-stu-id="51c1f-112">Method</span></span>       | <span data-ttu-id="51c1f-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="51c1f-113">Return Type</span></span>  |<span data-ttu-id="51c1f-114">Описание</span><span class="sxs-lookup"><span data-stu-id="51c1f-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="51c1f-115">Получение</span><span class="sxs-lookup"><span data-stu-id="51c1f-115">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="51c1f-116">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="51c1f-116">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="51c1f-117">Чтение свойств, связей или необработанного содержимого объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="51c1f-117">Read properties, relationships, or raw contents of a fileAttachment object.</span></span>|
|[<span data-ttu-id="51c1f-118">Удаление</span><span class="sxs-lookup"><span data-stu-id="51c1f-118">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="51c1f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="51c1f-119">None</span></span> |<span data-ttu-id="51c1f-120">Удаление объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="51c1f-120">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="51c1f-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="51c1f-121">Properties</span></span>
| <span data-ttu-id="51c1f-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="51c1f-122">Property</span></span>     | <span data-ttu-id="51c1f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="51c1f-123">Type</span></span>   |<span data-ttu-id="51c1f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="51c1f-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51c1f-125">contentBytes</span><span class="sxs-lookup"><span data-stu-id="51c1f-125">contentBytes</span></span>|<span data-ttu-id="51c1f-126">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="51c1f-126">Edm.Binary</span></span>|<span data-ttu-id="51c1f-127">Содержимое файла в кодировке base64.</span><span class="sxs-lookup"><span data-stu-id="51c1f-127">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="51c1f-128">contentId</span><span class="sxs-lookup"><span data-stu-id="51c1f-128">contentId</span></span>|<span data-ttu-id="51c1f-129">String</span><span class="sxs-lookup"><span data-stu-id="51c1f-129">String</span></span>|<span data-ttu-id="51c1f-130">Идентификатор вложения в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="51c1f-130">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="51c1f-131">contentLocation</span><span class="sxs-lookup"><span data-stu-id="51c1f-131">contentLocation</span></span>|<span data-ttu-id="51c1f-132">String</span><span class="sxs-lookup"><span data-stu-id="51c1f-132">String</span></span>|<span data-ttu-id="51c1f-133">Не используйте это свойство, так как оно не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51c1f-133">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="51c1f-134">contentType</span><span class="sxs-lookup"><span data-stu-id="51c1f-134">contentType</span></span>|<span data-ttu-id="51c1f-135">String</span><span class="sxs-lookup"><span data-stu-id="51c1f-135">String</span></span>|<span data-ttu-id="51c1f-136">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="51c1f-136">The content type of the attachment.</span></span>|
|<span data-ttu-id="51c1f-137">id</span><span class="sxs-lookup"><span data-stu-id="51c1f-137">id</span></span>|<span data-ttu-id="51c1f-138">String</span><span class="sxs-lookup"><span data-stu-id="51c1f-138">String</span></span>|<span data-ttu-id="51c1f-139">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="51c1f-139">The attachment ID.</span></span>|
|<span data-ttu-id="51c1f-140">isInline</span><span class="sxs-lookup"><span data-stu-id="51c1f-140">isInline</span></span>|<span data-ttu-id="51c1f-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="51c1f-141">Boolean</span></span>|<span data-ttu-id="51c1f-142">Задано значение true, если это встроенное вложение.</span><span class="sxs-lookup"><span data-stu-id="51c1f-142">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="51c1f-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51c1f-143">lastModifiedDateTime</span></span>|<span data-ttu-id="51c1f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51c1f-144">DateTimeOffset</span></span>|<span data-ttu-id="51c1f-145">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="51c1f-145">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="51c1f-146">name</span><span class="sxs-lookup"><span data-stu-id="51c1f-146">name</span></span>|<span data-ttu-id="51c1f-147">String</span><span class="sxs-lookup"><span data-stu-id="51c1f-147">String</span></span>|<span data-ttu-id="51c1f-148">Имя, представляющее текст, который отображается под значком, представляющим внедренное вложение. Оно может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="51c1f-148">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="51c1f-149">size</span><span class="sxs-lookup"><span data-stu-id="51c1f-149">size</span></span>|<span data-ttu-id="51c1f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="51c1f-150">Int32</span></span>|<span data-ttu-id="51c1f-151">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="51c1f-151">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51c1f-152">Связи</span><span class="sxs-lookup"><span data-stu-id="51c1f-152">Relationships</span></span>
<span data-ttu-id="51c1f-153">Нет</span><span class="sxs-lookup"><span data-stu-id="51c1f-153">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="51c1f-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51c1f-154">JSON representation</span></span>

<span data-ttu-id="51c1f-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51c1f-155">Here is a JSON representation of the resource</span></span>

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
