---
title: Тип ресурса fileAttachment
description: Файл (например, текстовый файл или документ Word), подключенного к событию
localization_priority: Normal
ms.openlocfilehash: 7032bcd234d07f0f3fdce0787968d72530a0a442
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510766"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="53225-103">Тип ресурса fileAttachment</span><span class="sxs-lookup"><span data-stu-id="53225-103">fileAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53225-104">Файл (например, текстовый файл или документ Word) подключенного к [события](../resources/event.md), [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [публикации](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="53225-104">A file (such as a text file or Word document) attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="53225-105">Свойство **contentBytes** содержит кодировки Base64 содержимое файла.</span><span class="sxs-lookup"><span data-stu-id="53225-105">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="53225-106">При создании вложенного файла включите в текст запроса следующее:</span><span class="sxs-lookup"><span data-stu-id="53225-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="53225-107">Обязательные свойства **name** и **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="53225-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="53225-108">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="53225-108">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="53225-109">Методы</span><span class="sxs-lookup"><span data-stu-id="53225-109">Methods</span></span>

| <span data-ttu-id="53225-110">Метод</span><span class="sxs-lookup"><span data-stu-id="53225-110">Method</span></span>       | <span data-ttu-id="53225-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="53225-111">Return Type</span></span>  |<span data-ttu-id="53225-112">Описание</span><span class="sxs-lookup"><span data-stu-id="53225-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="53225-113">Получение</span><span class="sxs-lookup"><span data-stu-id="53225-113">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="53225-114">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="53225-114">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="53225-115">Чтение свойств и связей объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="53225-115">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="53225-116">Удаление</span><span class="sxs-lookup"><span data-stu-id="53225-116">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="53225-117">Нет</span><span class="sxs-lookup"><span data-stu-id="53225-117">None</span></span> |<span data-ttu-id="53225-118">Удаление объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="53225-118">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="53225-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="53225-119">Properties</span></span>
| <span data-ttu-id="53225-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="53225-120">Property</span></span>     | <span data-ttu-id="53225-121">Тип</span><span class="sxs-lookup"><span data-stu-id="53225-121">Type</span></span>   |<span data-ttu-id="53225-122">Описание</span><span class="sxs-lookup"><span data-stu-id="53225-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53225-123">contentBytes</span><span class="sxs-lookup"><span data-stu-id="53225-123">contentBytes</span></span>|<span data-ttu-id="53225-124">Двоичный</span><span class="sxs-lookup"><span data-stu-id="53225-124">Binary</span></span>|<span data-ttu-id="53225-125">Содержимое файла в кодировке base64.</span><span class="sxs-lookup"><span data-stu-id="53225-125">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="53225-126">contentId</span><span class="sxs-lookup"><span data-stu-id="53225-126">contentId</span></span>|<span data-ttu-id="53225-127">String</span><span class="sxs-lookup"><span data-stu-id="53225-127">String</span></span>|<span data-ttu-id="53225-128">Идентификатор вложения в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="53225-128">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="53225-129">contentLocation</span><span class="sxs-lookup"><span data-stu-id="53225-129">contentLocation</span></span>|<span data-ttu-id="53225-130">String</span><span class="sxs-lookup"><span data-stu-id="53225-130">String</span></span>|<span data-ttu-id="53225-131">Универсальный код ресурса (URI), который соответствует расположению содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="53225-131">The Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>|
|<span data-ttu-id="53225-132">contentType</span><span class="sxs-lookup"><span data-stu-id="53225-132">contentType</span></span>|<span data-ttu-id="53225-133">Строка</span><span class="sxs-lookup"><span data-stu-id="53225-133">String</span></span>|<span data-ttu-id="53225-134">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="53225-134">The content type of the attachment.</span></span>|
|<span data-ttu-id="53225-135">id</span><span class="sxs-lookup"><span data-stu-id="53225-135">id</span></span>|<span data-ttu-id="53225-136">String</span><span class="sxs-lookup"><span data-stu-id="53225-136">String</span></span>|<span data-ttu-id="53225-137">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="53225-137">The attachment ID.</span></span>|
|<span data-ttu-id="53225-138">isInline</span><span class="sxs-lookup"><span data-stu-id="53225-138">isInline</span></span>|<span data-ttu-id="53225-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="53225-139">Boolean</span></span>|<span data-ttu-id="53225-140">Задано значение true, если это встроенное вложение.</span><span class="sxs-lookup"><span data-stu-id="53225-140">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="53225-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53225-141">lastModifiedDateTime</span></span>|<span data-ttu-id="53225-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53225-142">DateTimeOffset</span></span>|<span data-ttu-id="53225-143">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="53225-143">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="53225-144">name</span><span class="sxs-lookup"><span data-stu-id="53225-144">name</span></span>|<span data-ttu-id="53225-145">String</span><span class="sxs-lookup"><span data-stu-id="53225-145">String</span></span>|<span data-ttu-id="53225-146">Имя, представляющее текст, который отображается под значком, представляющим внедренное вложение. Оно может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="53225-146">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="53225-147">size</span><span class="sxs-lookup"><span data-stu-id="53225-147">size</span></span>|<span data-ttu-id="53225-148">Int32</span><span class="sxs-lookup"><span data-stu-id="53225-148">Int32</span></span>|<span data-ttu-id="53225-149">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="53225-149">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53225-150">Связи</span><span class="sxs-lookup"><span data-stu-id="53225-150">Relationships</span></span>
<span data-ttu-id="53225-151">Нет</span><span class="sxs-lookup"><span data-stu-id="53225-151">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="53225-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53225-152">JSON representation</span></span>

<span data-ttu-id="53225-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53225-153">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/fileattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
