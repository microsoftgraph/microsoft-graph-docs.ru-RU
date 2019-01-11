---
title: Тип ресурса referenceAttachment
description: 'Ссылка на папку или файл (например, текстовый файл или документ Word) на OneDrive для бизнеса облачных диска и других местах, поддерживаемые хранилища, подключенного к '
localization_priority: Normal
ms.openlocfilehash: 6a334b303bea7aff768733434b9ba882de237a12
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880054"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="eaa81-103">Тип ресурса referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="eaa81-103">referenceAttachment resource type</span></span>

> <span data-ttu-id="eaa81-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eaa81-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eaa81-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaa81-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eaa81-106">Ссылка на папку или файл (например, текстовый файл или документ Word) на OneDrive для Business cloud диска или другие поддерживаемые места хранения, подключенного к [события](../resources/event.md), [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [публикации](../resources/post.md) .</span><span class="sxs-lookup"><span data-stu-id="eaa81-106">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="eaa81-107">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="eaa81-107">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="eaa81-108">Методы</span><span class="sxs-lookup"><span data-stu-id="eaa81-108">Methods</span></span>

| <span data-ttu-id="eaa81-109">Метод</span><span class="sxs-lookup"><span data-stu-id="eaa81-109">Method</span></span>       | <span data-ttu-id="eaa81-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eaa81-110">Return Type</span></span>  |<span data-ttu-id="eaa81-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eaa81-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eaa81-112">Get</span><span class="sxs-lookup"><span data-stu-id="eaa81-112">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="eaa81-113">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="eaa81-113">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="eaa81-114">Чтение свойств и связей объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="eaa81-114">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="eaa81-115">Delete</span><span class="sxs-lookup"><span data-stu-id="eaa81-115">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="eaa81-116">Нет</span><span class="sxs-lookup"><span data-stu-id="eaa81-116">None</span></span> |<span data-ttu-id="eaa81-117">Удаление объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="eaa81-117">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="eaa81-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="eaa81-118">Properties</span></span>
| <span data-ttu-id="eaa81-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="eaa81-119">Property</span></span>     | <span data-ttu-id="eaa81-120">Тип</span><span class="sxs-lookup"><span data-stu-id="eaa81-120">Type</span></span>   |<span data-ttu-id="eaa81-121">Описание</span><span class="sxs-lookup"><span data-stu-id="eaa81-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eaa81-122">contentType</span><span class="sxs-lookup"><span data-stu-id="eaa81-122">contentType</span></span>|<span data-ttu-id="eaa81-123">String</span><span class="sxs-lookup"><span data-stu-id="eaa81-123">String</span></span>|<span data-ttu-id="eaa81-124">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="eaa81-124">The content type of the attachment.</span></span> <span data-ttu-id="eaa81-125">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="eaa81-125">Optional.</span></span>|
|<span data-ttu-id="eaa81-126">id</span><span class="sxs-lookup"><span data-stu-id="eaa81-126">id</span></span>|<span data-ttu-id="eaa81-127">String</span><span class="sxs-lookup"><span data-stu-id="eaa81-127">String</span></span>|<span data-ttu-id="eaa81-p103">Идентификатор вложения.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eaa81-p103">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="eaa81-130">isFolder</span><span class="sxs-lookup"><span data-stu-id="eaa81-130">isFolder</span></span>|<span data-ttu-id="eaa81-131">Логический</span><span class="sxs-lookup"><span data-stu-id="eaa81-131">Boolean</span></span>|<span data-ttu-id="eaa81-132">Указывает, является ли вложение ссылок в папку.</span><span class="sxs-lookup"><span data-stu-id="eaa81-132">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="eaa81-133">Необходимо установить это значение true, если **sourceUrl** — это ссылка на папку.</span><span class="sxs-lookup"><span data-stu-id="eaa81-133">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="eaa81-134">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="eaa81-134">Optional.</span></span>|
|<span data-ttu-id="eaa81-135">isInline</span><span class="sxs-lookup"><span data-stu-id="eaa81-135">isInline</span></span>|<span data-ttu-id="eaa81-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="eaa81-136">Boolean</span></span>|<span data-ttu-id="eaa81-137">Значение true указывает, что вложение встроено в содержимое объекта.</span><span class="sxs-lookup"><span data-stu-id="eaa81-137">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="eaa81-138">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="eaa81-138">Optional.</span></span>|
|<span data-ttu-id="eaa81-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eaa81-139">lastModifiedDateTime</span></span>|<span data-ttu-id="eaa81-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaa81-140">DateTimeOffset</span></span>|<span data-ttu-id="eaa81-141">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="eaa81-141">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="eaa81-142">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="eaa81-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eaa81-143">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="eaa81-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="eaa81-144">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="eaa81-144">Optional.</span></span>|
|<span data-ttu-id="eaa81-145">name</span><span class="sxs-lookup"><span data-stu-id="eaa81-145">name</span></span>|<span data-ttu-id="eaa81-146">Строка</span><span class="sxs-lookup"><span data-stu-id="eaa81-146">String</span></span>|<span data-ttu-id="eaa81-147">Текст, который отображается под значок, обозначающий внедренного вложения.</span><span class="sxs-lookup"><span data-stu-id="eaa81-147">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="eaa81-148">Она не обязательно должна находиться фактическое имя файла.</span><span class="sxs-lookup"><span data-stu-id="eaa81-148">This does not need to be the actual file name.</span></span> <span data-ttu-id="eaa81-149">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eaa81-149">Required.</span></span>|
|<span data-ttu-id="eaa81-150">разрешение</span><span class="sxs-lookup"><span data-stu-id="eaa81-150">permission</span></span>|<span data-ttu-id="eaa81-151">ReferenceAttachmentPermissions</span><span class="sxs-lookup"><span data-stu-id="eaa81-151">ReferenceAttachmentPermissions</span></span>|<span data-ttu-id="eaa81-152">Задает разрешения, предоставленные вложения по типу поставщика в **providerType**.</span><span class="sxs-lookup"><span data-stu-id="eaa81-152">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="eaa81-153">Возможные значения: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span><span class="sxs-lookup"><span data-stu-id="eaa81-153">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="eaa81-154">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="eaa81-154">Optional.</span></span>|
|<span data-ttu-id="eaa81-155">previewUrl</span><span class="sxs-lookup"><span data-stu-id="eaa81-155">previewUrl</span></span>|<span data-ttu-id="eaa81-156">Строка</span><span class="sxs-lookup"><span data-stu-id="eaa81-156">String</span></span>|<span data-ttu-id="eaa81-157">Применяется только вложения ссылку объекта на изображении - URL-адрес для получения изображения для предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="eaa81-157">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="eaa81-158">Используйте **thumbnailUrl** и **previewUrl** только в том случае, когда **sourceUrl** определяет файл изображения.</span><span class="sxs-lookup"><span data-stu-id="eaa81-158">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="eaa81-159">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="eaa81-159">Optional.</span></span>|
|<span data-ttu-id="eaa81-160">providerType</span><span class="sxs-lookup"><span data-stu-id="eaa81-160">providerType</span></span>|<span data-ttu-id="eaa81-161">ReferenceAttachmentProviders</span><span class="sxs-lookup"><span data-stu-id="eaa81-161">ReferenceAttachmentProviders</span></span>|<span data-ttu-id="eaa81-162">Тип поставщика, который поддерживает вложение в этом contentType.</span><span class="sxs-lookup"><span data-stu-id="eaa81-162">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="eaa81-163">Возможные значения: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span><span class="sxs-lookup"><span data-stu-id="eaa81-163">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="eaa81-164">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="eaa81-164">Optional.</span></span>|
|<span data-ttu-id="eaa81-165">size</span><span class="sxs-lookup"><span data-stu-id="eaa81-165">size</span></span>|<span data-ttu-id="eaa81-166">Int32</span><span class="sxs-lookup"><span data-stu-id="eaa81-166">Int32</span></span>|<span data-ttu-id="eaa81-167">Размер метаданных в байтах, которые хранятся на сообщение для вложения ссылку.</span><span class="sxs-lookup"><span data-stu-id="eaa81-167">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="eaa81-168">Это значение не отображает фактический размер файла.</span><span class="sxs-lookup"><span data-stu-id="eaa81-168">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="eaa81-169">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="eaa81-169">Optional.</span></span>|
|<span data-ttu-id="eaa81-170">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="eaa81-170">sourceUrl</span></span>|<span data-ttu-id="eaa81-171">Строка</span><span class="sxs-lookup"><span data-stu-id="eaa81-171">String</span></span>|<span data-ttu-id="eaa81-172">URL-адрес для получения содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="eaa81-172">URL to get the attachment content.</span></span> <span data-ttu-id="eaa81-173">Если это URL-адрес в папку, для папки для правильного отображения в Outlook или Outlook в Интернете, задайте его **isFolder** имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="eaa81-173">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="eaa81-174">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eaa81-174">Required.</span></span>|
|<span data-ttu-id="eaa81-175">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="eaa81-175">thumbnailUrl</span></span>|<span data-ttu-id="eaa81-176">Строка</span><span class="sxs-lookup"><span data-stu-id="eaa81-176">String</span></span>|<span data-ttu-id="eaa81-177">Применяется только вложения ссылку объекта на изображении - URL-адрес для получения эскизное изображение.</span><span class="sxs-lookup"><span data-stu-id="eaa81-177">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="eaa81-178">Используйте **thumbnailUrl** и **previewUrl** только в том случае, когда **sourceUrl** определяет файл изображения.</span><span class="sxs-lookup"><span data-stu-id="eaa81-178">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="eaa81-179">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="eaa81-179">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eaa81-180">Связи</span><span class="sxs-lookup"><span data-stu-id="eaa81-180">Relationships</span></span>
<span data-ttu-id="eaa81-181">Нет</span><span class="sxs-lookup"><span data-stu-id="eaa81-181">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="eaa81-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eaa81-182">JSON representation</span></span>

<span data-ttu-id="eaa81-183">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eaa81-183">Here is a JSON representation of the resource</span></span>

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
  "permission": "string",
  "previewUrl": "string",
  "providerType": "string",
  "size": 1024,
  "sourceUrl": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
