---
title: Тип ресурса fileAttachment
description: Файл (например, текстовый файл или документ Word), подключенного к событию
ms.openlocfilehash: 2a43ebbc78d831e907bfd19d647e4b7e398abe90
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079007"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="b066e-103">Тип ресурса fileAttachment</span><span class="sxs-lookup"><span data-stu-id="b066e-103">fileAttachment resource type</span></span>

> <span data-ttu-id="b066e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b066e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b066e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b066e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b066e-106">Файл (например, текстовый файл или документ Word) подключенного к [события](../resources/event.md), [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [публикации](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="b066e-106">A file (such as a text file or Word document) attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="b066e-107">Свойство **contentBytes** содержит кодировки Base64 содержимое файла.</span><span class="sxs-lookup"><span data-stu-id="b066e-107">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="b066e-108">При создании вложенного файла включите в текст запроса следующее:</span><span class="sxs-lookup"><span data-stu-id="b066e-108">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="b066e-109">Обязательные свойства **name** и **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="b066e-109">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="b066e-110">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="b066e-110">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b066e-111">Методы</span><span class="sxs-lookup"><span data-stu-id="b066e-111">Methods</span></span>

| <span data-ttu-id="b066e-112">Метод</span><span class="sxs-lookup"><span data-stu-id="b066e-112">Method</span></span>       | <span data-ttu-id="b066e-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b066e-113">Return Type</span></span>  |<span data-ttu-id="b066e-114">Описание</span><span class="sxs-lookup"><span data-stu-id="b066e-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b066e-115">Получение</span><span class="sxs-lookup"><span data-stu-id="b066e-115">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="b066e-116">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="b066e-116">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="b066e-117">Чтение свойств и связей объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="b066e-117">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="b066e-118">Удаление</span><span class="sxs-lookup"><span data-stu-id="b066e-118">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="b066e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b066e-119">None</span></span> |<span data-ttu-id="b066e-120">Удаление объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="b066e-120">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b066e-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="b066e-121">Properties</span></span>
| <span data-ttu-id="b066e-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="b066e-122">Property</span></span>     | <span data-ttu-id="b066e-123">Тип</span><span class="sxs-lookup"><span data-stu-id="b066e-123">Type</span></span>   |<span data-ttu-id="b066e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b066e-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b066e-125">contentBytes</span><span class="sxs-lookup"><span data-stu-id="b066e-125">contentBytes</span></span>|<span data-ttu-id="b066e-126">Двоичный</span><span class="sxs-lookup"><span data-stu-id="b066e-126">Binary</span></span>|<span data-ttu-id="b066e-127">Содержимое файла в кодировке base64.</span><span class="sxs-lookup"><span data-stu-id="b066e-127">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="b066e-128">contentId</span><span class="sxs-lookup"><span data-stu-id="b066e-128">contentId</span></span>|<span data-ttu-id="b066e-129">String</span><span class="sxs-lookup"><span data-stu-id="b066e-129">String</span></span>|<span data-ttu-id="b066e-130">Идентификатор вложения в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="b066e-130">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="b066e-131">contentLocation</span><span class="sxs-lookup"><span data-stu-id="b066e-131">contentLocation</span></span>|<span data-ttu-id="b066e-132">String</span><span class="sxs-lookup"><span data-stu-id="b066e-132">String</span></span>|<span data-ttu-id="b066e-133">Универсальный код ресурса (URI), который соответствует расположению содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="b066e-133">The Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>|
|<span data-ttu-id="b066e-134">contentType</span><span class="sxs-lookup"><span data-stu-id="b066e-134">contentType</span></span>|<span data-ttu-id="b066e-135">String</span><span class="sxs-lookup"><span data-stu-id="b066e-135">String</span></span>|<span data-ttu-id="b066e-136">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="b066e-136">The content type of the attachment.</span></span>|
|<span data-ttu-id="b066e-137">id</span><span class="sxs-lookup"><span data-stu-id="b066e-137">id</span></span>|<span data-ttu-id="b066e-138">String</span><span class="sxs-lookup"><span data-stu-id="b066e-138">String</span></span>|<span data-ttu-id="b066e-139">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="b066e-139">The attachment ID.</span></span>|
|<span data-ttu-id="b066e-140">isInline</span><span class="sxs-lookup"><span data-stu-id="b066e-140">isInline</span></span>|<span data-ttu-id="b066e-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="b066e-141">Boolean</span></span>|<span data-ttu-id="b066e-142">Задано значение true, если это встроенное вложение.</span><span class="sxs-lookup"><span data-stu-id="b066e-142">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="b066e-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b066e-143">lastModifiedDateTime</span></span>|<span data-ttu-id="b066e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b066e-144">DateTimeOffset</span></span>|<span data-ttu-id="b066e-145">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="b066e-145">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="b066e-146">name</span><span class="sxs-lookup"><span data-stu-id="b066e-146">name</span></span>|<span data-ttu-id="b066e-147">String</span><span class="sxs-lookup"><span data-stu-id="b066e-147">String</span></span>|<span data-ttu-id="b066e-148">Имя, представляющее текст, который отображается под значком, представляющим внедренное вложение. Оно может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="b066e-148">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="b066e-149">size</span><span class="sxs-lookup"><span data-stu-id="b066e-149">size</span></span>|<span data-ttu-id="b066e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b066e-150">Int32</span></span>|<span data-ttu-id="b066e-151">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="b066e-151">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b066e-152">Связи</span><span class="sxs-lookup"><span data-stu-id="b066e-152">Relationships</span></span>
<span data-ttu-id="b066e-153">Нет</span><span class="sxs-lookup"><span data-stu-id="b066e-153">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b066e-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b066e-154">JSON representation</span></span>

<span data-ttu-id="b066e-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b066e-155">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
