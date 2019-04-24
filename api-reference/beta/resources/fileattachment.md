---
title: Тип ресурса fileAttachment
description: Файл (например, текстовый файл или документ Word), присоединенный к событию,
localization_priority: Normal
ms.openlocfilehash: 7d9f92565e38aaf418691480b7f8f3187c57647c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506370"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="3fe0a-103">Тип ресурса fileAttachment</span><span class="sxs-lookup"><span data-stu-id="3fe0a-103">fileAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fe0a-104">Файл (например, текстовый файл или документ Word), присоединенный к событию, [сообщению](../resources/message.md), [задаче Outlook](../resources/outlooktask.md)или [POST](../resources/post.md). [](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="3fe0a-104">A file (such as a text file or Word document) attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span> <span data-ttu-id="3fe0a-105">Свойство **contentBytes** включает содержимое файла в кодировке Base 64.</span><span class="sxs-lookup"><span data-stu-id="3fe0a-105">The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="3fe0a-106">При создании вложенного файла включите в текст запроса следующее:</span><span class="sxs-lookup"><span data-stu-id="3fe0a-106">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="3fe0a-107">Обязательные свойства **name** и **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="3fe0a-107">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="3fe0a-108">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="3fe0a-108">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3fe0a-109">Методы</span><span class="sxs-lookup"><span data-stu-id="3fe0a-109">Methods</span></span>

| <span data-ttu-id="3fe0a-110">Метод</span><span class="sxs-lookup"><span data-stu-id="3fe0a-110">Method</span></span>       | <span data-ttu-id="3fe0a-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3fe0a-111">Return Type</span></span>  |<span data-ttu-id="3fe0a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3fe0a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3fe0a-113">Получение</span><span class="sxs-lookup"><span data-stu-id="3fe0a-113">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="3fe0a-114">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="3fe0a-114">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="3fe0a-115">Чтение свойств и связей объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="3fe0a-115">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="3fe0a-116">Удаление</span><span class="sxs-lookup"><span data-stu-id="3fe0a-116">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="3fe0a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="3fe0a-117">None</span></span> |<span data-ttu-id="3fe0a-118">Удаление объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="3fe0a-118">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3fe0a-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="3fe0a-119">Properties</span></span>
| <span data-ttu-id="3fe0a-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fe0a-120">Property</span></span>     | <span data-ttu-id="3fe0a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3fe0a-121">Type</span></span>   |<span data-ttu-id="3fe0a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3fe0a-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3fe0a-123">contentBytes</span><span class="sxs-lookup"><span data-stu-id="3fe0a-123">contentBytes</span></span>|<span data-ttu-id="3fe0a-124">Двоичный</span><span class="sxs-lookup"><span data-stu-id="3fe0a-124">Binary</span></span>|<span data-ttu-id="3fe0a-125">Содержимое файла в кодировке base64.</span><span class="sxs-lookup"><span data-stu-id="3fe0a-125">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="3fe0a-126">contentId</span><span class="sxs-lookup"><span data-stu-id="3fe0a-126">contentId</span></span>|<span data-ttu-id="3fe0a-127">String</span><span class="sxs-lookup"><span data-stu-id="3fe0a-127">String</span></span>|<span data-ttu-id="3fe0a-128">Идентификатор вложения в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3fe0a-128">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="3fe0a-129">contentLocation</span><span class="sxs-lookup"><span data-stu-id="3fe0a-129">contentLocation</span></span>|<span data-ttu-id="3fe0a-130">String</span><span class="sxs-lookup"><span data-stu-id="3fe0a-130">String</span></span>|<span data-ttu-id="3fe0a-131">Не используйте это свойство, так как оно не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fe0a-131">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="3fe0a-132">contentType</span><span class="sxs-lookup"><span data-stu-id="3fe0a-132">contentType</span></span>|<span data-ttu-id="3fe0a-133">String</span><span class="sxs-lookup"><span data-stu-id="3fe0a-133">String</span></span>|<span data-ttu-id="3fe0a-134">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="3fe0a-134">The content type of the attachment.</span></span>|
|<span data-ttu-id="3fe0a-135">id</span><span class="sxs-lookup"><span data-stu-id="3fe0a-135">id</span></span>|<span data-ttu-id="3fe0a-136">Строка</span><span class="sxs-lookup"><span data-stu-id="3fe0a-136">String</span></span>|<span data-ttu-id="3fe0a-137">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="3fe0a-137">The attachment ID.</span></span>|
|<span data-ttu-id="3fe0a-138">isInline</span><span class="sxs-lookup"><span data-stu-id="3fe0a-138">isInline</span></span>|<span data-ttu-id="3fe0a-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="3fe0a-139">Boolean</span></span>|<span data-ttu-id="3fe0a-140">Задано значение true, если это встроенное вложение.</span><span class="sxs-lookup"><span data-stu-id="3fe0a-140">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="3fe0a-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3fe0a-141">lastModifiedDateTime</span></span>|<span data-ttu-id="3fe0a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fe0a-142">DateTimeOffset</span></span>|<span data-ttu-id="3fe0a-143">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="3fe0a-143">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="3fe0a-144">name</span><span class="sxs-lookup"><span data-stu-id="3fe0a-144">name</span></span>|<span data-ttu-id="3fe0a-145">String</span><span class="sxs-lookup"><span data-stu-id="3fe0a-145">String</span></span>|<span data-ttu-id="3fe0a-146">Имя, представляющее текст, который отображается под значком, представляющим внедренное вложение. Оно может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="3fe0a-146">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="3fe0a-147">size</span><span class="sxs-lookup"><span data-stu-id="3fe0a-147">size</span></span>|<span data-ttu-id="3fe0a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="3fe0a-148">Int32</span></span>|<span data-ttu-id="3fe0a-149">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="3fe0a-149">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3fe0a-150">Отношения</span><span class="sxs-lookup"><span data-stu-id="3fe0a-150">Relationships</span></span>
<span data-ttu-id="3fe0a-151">Нет</span><span class="sxs-lookup"><span data-stu-id="3fe0a-151">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3fe0a-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3fe0a-152">JSON representation</span></span>

<span data-ttu-id="3fe0a-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3fe0a-153">Here is a JSON representation of the resource</span></span>

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
