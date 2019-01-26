---
title: Тип ресурса referenceAttachment
description: 'Ссылка на папку или файл (например, текстовый файл или документ Word) на OneDrive для бизнеса облачных диска и других местах, поддерживаемые хранилища, подключенного к '
localization_priority: Normal
ms.openlocfilehash: adf078f7ba678a4fe90a51972c5e4be4788c9c0c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574560"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="78f0b-103">Тип ресурса referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="78f0b-103">referenceAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78f0b-104">Ссылка на папку или файл (например, текстовый файл или документ Word) на OneDrive для Business cloud диска или другие поддерживаемые места хранения, подключенного к [события](../resources/event.md), [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [публикации](../resources/post.md) .</span><span class="sxs-lookup"><span data-stu-id="78f0b-104">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="78f0b-105">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="78f0b-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="78f0b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="78f0b-106">Methods</span></span>

| <span data-ttu-id="78f0b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="78f0b-107">Method</span></span>       | <span data-ttu-id="78f0b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="78f0b-108">Return Type</span></span>  |<span data-ttu-id="78f0b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="78f0b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="78f0b-110">Get</span><span class="sxs-lookup"><span data-stu-id="78f0b-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="78f0b-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="78f0b-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="78f0b-112">Чтение свойств и связей объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="78f0b-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="78f0b-113">Delete</span><span class="sxs-lookup"><span data-stu-id="78f0b-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="78f0b-114">Нет</span><span class="sxs-lookup"><span data-stu-id="78f0b-114">None</span></span> |<span data-ttu-id="78f0b-115">Удаление объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="78f0b-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="78f0b-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="78f0b-116">Properties</span></span>
| <span data-ttu-id="78f0b-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="78f0b-117">Property</span></span>     | <span data-ttu-id="78f0b-118">Тип</span><span class="sxs-lookup"><span data-stu-id="78f0b-118">Type</span></span>   |<span data-ttu-id="78f0b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="78f0b-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78f0b-120">contentType</span><span class="sxs-lookup"><span data-stu-id="78f0b-120">contentType</span></span>|<span data-ttu-id="78f0b-121">String</span><span class="sxs-lookup"><span data-stu-id="78f0b-121">String</span></span>|<span data-ttu-id="78f0b-122">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="78f0b-122">The content type of the attachment.</span></span> <span data-ttu-id="78f0b-123">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="78f0b-123">Optional.</span></span>|
|<span data-ttu-id="78f0b-124">id</span><span class="sxs-lookup"><span data-stu-id="78f0b-124">id</span></span>|<span data-ttu-id="78f0b-125">String</span><span class="sxs-lookup"><span data-stu-id="78f0b-125">String</span></span>|<span data-ttu-id="78f0b-p102">Идентификатор вложения.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="78f0b-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="78f0b-128">isFolder</span><span class="sxs-lookup"><span data-stu-id="78f0b-128">isFolder</span></span>|<span data-ttu-id="78f0b-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="78f0b-129">Boolean</span></span>|<span data-ttu-id="78f0b-130">Указывает, является ли вложение ссылок в папку.</span><span class="sxs-lookup"><span data-stu-id="78f0b-130">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="78f0b-131">Необходимо установить это значение true, если **sourceUrl** — это ссылка на папку.</span><span class="sxs-lookup"><span data-stu-id="78f0b-131">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="78f0b-132">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="78f0b-132">Optional.</span></span>|
|<span data-ttu-id="78f0b-133">isInline</span><span class="sxs-lookup"><span data-stu-id="78f0b-133">isInline</span></span>|<span data-ttu-id="78f0b-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="78f0b-134">Boolean</span></span>|<span data-ttu-id="78f0b-135">Значение true указывает, что вложение встроено в содержимое объекта.</span><span class="sxs-lookup"><span data-stu-id="78f0b-135">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="78f0b-136">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="78f0b-136">Optional.</span></span>|
|<span data-ttu-id="78f0b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78f0b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="78f0b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78f0b-138">DateTimeOffset</span></span>|<span data-ttu-id="78f0b-139">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="78f0b-139">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="78f0b-140">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="78f0b-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="78f0b-141">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="78f0b-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="78f0b-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="78f0b-142">Optional.</span></span>|
|<span data-ttu-id="78f0b-143">name</span><span class="sxs-lookup"><span data-stu-id="78f0b-143">name</span></span>|<span data-ttu-id="78f0b-144">Строка</span><span class="sxs-lookup"><span data-stu-id="78f0b-144">String</span></span>|<span data-ttu-id="78f0b-145">Текст, который отображается под значок, обозначающий внедренного вложения.</span><span class="sxs-lookup"><span data-stu-id="78f0b-145">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="78f0b-146">Она не обязательно должна находиться фактическое имя файла.</span><span class="sxs-lookup"><span data-stu-id="78f0b-146">This does not need to be the actual file name.</span></span> <span data-ttu-id="78f0b-147">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78f0b-147">Required.</span></span>|
|<span data-ttu-id="78f0b-148">разрешение</span><span class="sxs-lookup"><span data-stu-id="78f0b-148">permission</span></span>|<span data-ttu-id="78f0b-149">referenceAttachmentPermission</span><span class="sxs-lookup"><span data-stu-id="78f0b-149">referenceAttachmentPermission</span></span>|<span data-ttu-id="78f0b-150">Задает разрешения, предоставленные вложения по типу поставщика в **providerType**.</span><span class="sxs-lookup"><span data-stu-id="78f0b-150">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="78f0b-151">Возможные значения: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span><span class="sxs-lookup"><span data-stu-id="78f0b-151">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="78f0b-152">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="78f0b-152">Optional.</span></span>|
|<span data-ttu-id="78f0b-153">previewUrl</span><span class="sxs-lookup"><span data-stu-id="78f0b-153">previewUrl</span></span>|<span data-ttu-id="78f0b-154">Строка</span><span class="sxs-lookup"><span data-stu-id="78f0b-154">String</span></span>|<span data-ttu-id="78f0b-155">Применяется только вложения ссылку объекта на изображении - URL-адрес для получения изображения для предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="78f0b-155">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="78f0b-156">Используйте **thumbnailUrl** и **previewUrl** только в том случае, когда **sourceUrl** определяет файл изображения.</span><span class="sxs-lookup"><span data-stu-id="78f0b-156">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="78f0b-157">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="78f0b-157">Optional.</span></span>|
|<span data-ttu-id="78f0b-158">providerType</span><span class="sxs-lookup"><span data-stu-id="78f0b-158">providerType</span></span>| <span data-ttu-id="78f0b-159">referenceAttachmentProvider</span><span class="sxs-lookup"><span data-stu-id="78f0b-159">referenceAttachmentProvider</span></span> |<span data-ttu-id="78f0b-160">Тип поставщика, который поддерживает вложение в этом contentType.</span><span class="sxs-lookup"><span data-stu-id="78f0b-160">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="78f0b-161">Возможные значения: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span><span class="sxs-lookup"><span data-stu-id="78f0b-161">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="78f0b-162">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="78f0b-162">Optional.</span></span>|
|<span data-ttu-id="78f0b-163">size</span><span class="sxs-lookup"><span data-stu-id="78f0b-163">size</span></span>|<span data-ttu-id="78f0b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="78f0b-164">Int32</span></span>|<span data-ttu-id="78f0b-165">Размер метаданных в байтах, которые хранятся на сообщение для вложения ссылку.</span><span class="sxs-lookup"><span data-stu-id="78f0b-165">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="78f0b-166">Это значение не отображает фактический размер файла.</span><span class="sxs-lookup"><span data-stu-id="78f0b-166">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="78f0b-167">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="78f0b-167">Optional.</span></span>|
|<span data-ttu-id="78f0b-168">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="78f0b-168">sourceUrl</span></span>|<span data-ttu-id="78f0b-169">Строка</span><span class="sxs-lookup"><span data-stu-id="78f0b-169">String</span></span>|<span data-ttu-id="78f0b-170">URL-адрес для получения содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="78f0b-170">URL to get the attachment content.</span></span> <span data-ttu-id="78f0b-171">Если это URL-адрес в папку, для папки для правильного отображения в Outlook или Outlook в Интернете, задайте его **isFolder** имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="78f0b-171">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="78f0b-172">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="78f0b-172">Required.</span></span>|
|<span data-ttu-id="78f0b-173">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="78f0b-173">thumbnailUrl</span></span>|<span data-ttu-id="78f0b-174">Строка</span><span class="sxs-lookup"><span data-stu-id="78f0b-174">String</span></span>|<span data-ttu-id="78f0b-175">Применяется только вложения ссылку объекта на изображении - URL-адрес для получения эскизное изображение.</span><span class="sxs-lookup"><span data-stu-id="78f0b-175">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="78f0b-176">Используйте **thumbnailUrl** и **previewUrl** только в том случае, когда **sourceUrl** определяет файл изображения.</span><span class="sxs-lookup"><span data-stu-id="78f0b-176">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="78f0b-177">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="78f0b-177">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78f0b-178">Связи</span><span class="sxs-lookup"><span data-stu-id="78f0b-178">Relationships</span></span>
<span data-ttu-id="78f0b-179">Нет</span><span class="sxs-lookup"><span data-stu-id="78f0b-179">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="78f0b-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78f0b-180">JSON representation</span></span>

<span data-ttu-id="78f0b-181">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78f0b-181">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isFolder": true,
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "permission": "referenceAttachmentPermission",
  "previewUrl": "string",
  "providerType": "referenceAttachmentProvider",
  "size": 1024,
  "sourceUrl": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/referenceattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
