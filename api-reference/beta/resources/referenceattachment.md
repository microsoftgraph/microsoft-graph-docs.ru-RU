---
title: Тип ресурса referenceAttachment
description: 'Ссылка на папку или файл (например, текстовый файл или документ Word) на OneDrive для бизнеса облачных диска и других местах, поддерживаемые хранилища, подключенного к '
ms.openlocfilehash: e9885c3a0e5c7f723303d7d6461f4c07dbed6bf6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080586"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="18a0e-103">Тип ресурса referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="18a0e-103">referenceAttachment resource type</span></span>

> <span data-ttu-id="18a0e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="18a0e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18a0e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18a0e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18a0e-106">Ссылка на папку или файл (например, текстовый файл или документ Word) на OneDrive для Business cloud диска или другие поддерживаемые места хранения, подключенного к [события](../resources/event.md), [сообщения](../resources/message.md), [задачи Outlook](../resources/outlooktask.md)или [публикации](../resources/post.md) .</span><span class="sxs-lookup"><span data-stu-id="18a0e-106">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="18a0e-107">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="18a0e-107">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="18a0e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="18a0e-108">Methods</span></span>

| <span data-ttu-id="18a0e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="18a0e-109">Method</span></span>       | <span data-ttu-id="18a0e-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="18a0e-110">Return Type</span></span>  |<span data-ttu-id="18a0e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="18a0e-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="18a0e-112">Get</span><span class="sxs-lookup"><span data-stu-id="18a0e-112">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="18a0e-113">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="18a0e-113">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="18a0e-114">Чтение свойств и связей объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="18a0e-114">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="18a0e-115">Delete</span><span class="sxs-lookup"><span data-stu-id="18a0e-115">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="18a0e-116">Нет</span><span class="sxs-lookup"><span data-stu-id="18a0e-116">None</span></span> |<span data-ttu-id="18a0e-117">Удаление объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="18a0e-117">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="18a0e-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="18a0e-118">Properties</span></span>
| <span data-ttu-id="18a0e-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="18a0e-119">Property</span></span>     | <span data-ttu-id="18a0e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="18a0e-120">Type</span></span>   |<span data-ttu-id="18a0e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="18a0e-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18a0e-122">contentType</span><span class="sxs-lookup"><span data-stu-id="18a0e-122">contentType</span></span>|<span data-ttu-id="18a0e-123">String</span><span class="sxs-lookup"><span data-stu-id="18a0e-123">String</span></span>|<span data-ttu-id="18a0e-124">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="18a0e-124">The content type of the attachment.</span></span> <span data-ttu-id="18a0e-125">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="18a0e-125">Optional.</span></span>|
|<span data-ttu-id="18a0e-126">id</span><span class="sxs-lookup"><span data-stu-id="18a0e-126">id</span></span>|<span data-ttu-id="18a0e-127">String</span><span class="sxs-lookup"><span data-stu-id="18a0e-127">String</span></span>|<span data-ttu-id="18a0e-p103">Идентификатор вложения.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18a0e-p103">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="18a0e-130">isFolder</span><span class="sxs-lookup"><span data-stu-id="18a0e-130">isFolder</span></span>|<span data-ttu-id="18a0e-131">Логический</span><span class="sxs-lookup"><span data-stu-id="18a0e-131">Boolean</span></span>|<span data-ttu-id="18a0e-132">Указывает, является ли вложение ссылок в папку.</span><span class="sxs-lookup"><span data-stu-id="18a0e-132">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="18a0e-133">Необходимо установить это значение true, если **sourceUrl** — это ссылка на папку.</span><span class="sxs-lookup"><span data-stu-id="18a0e-133">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="18a0e-134">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="18a0e-134">Optional.</span></span>|
|<span data-ttu-id="18a0e-135">isInline</span><span class="sxs-lookup"><span data-stu-id="18a0e-135">isInline</span></span>|<span data-ttu-id="18a0e-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="18a0e-136">Boolean</span></span>|<span data-ttu-id="18a0e-137">Значение true указывает, что вложение встроено в содержимое объекта.</span><span class="sxs-lookup"><span data-stu-id="18a0e-137">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="18a0e-138">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="18a0e-138">Optional.</span></span>|
|<span data-ttu-id="18a0e-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18a0e-139">lastModifiedDateTime</span></span>|<span data-ttu-id="18a0e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18a0e-140">DateTimeOffset</span></span>|<span data-ttu-id="18a0e-141">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="18a0e-141">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="18a0e-142">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="18a0e-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="18a0e-143">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="18a0e-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="18a0e-144">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="18a0e-144">Optional.</span></span>|
|<span data-ttu-id="18a0e-145">name</span><span class="sxs-lookup"><span data-stu-id="18a0e-145">name</span></span>|<span data-ttu-id="18a0e-146">String</span><span class="sxs-lookup"><span data-stu-id="18a0e-146">String</span></span>|<span data-ttu-id="18a0e-147">Текст, который отображается под значок, обозначающий внедренного вложения.</span><span class="sxs-lookup"><span data-stu-id="18a0e-147">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="18a0e-148">Она не обязательно должна находиться фактическое имя файла.</span><span class="sxs-lookup"><span data-stu-id="18a0e-148">This does not need to be the actual file name.</span></span> <span data-ttu-id="18a0e-149">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="18a0e-149">Required.</span></span>|
|<span data-ttu-id="18a0e-150">разрешение</span><span class="sxs-lookup"><span data-stu-id="18a0e-150">permission</span></span>|<span data-ttu-id="18a0e-151">ReferenceAttachmentPermissions</span><span class="sxs-lookup"><span data-stu-id="18a0e-151">ReferenceAttachmentPermissions</span></span>|<span data-ttu-id="18a0e-152">Задает разрешения, предоставленные вложения по типу поставщика в **providerType**.</span><span class="sxs-lookup"><span data-stu-id="18a0e-152">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="18a0e-153">Возможные значения: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span><span class="sxs-lookup"><span data-stu-id="18a0e-153">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="18a0e-154">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="18a0e-154">Optional.</span></span>|
|<span data-ttu-id="18a0e-155">previewUrl</span><span class="sxs-lookup"><span data-stu-id="18a0e-155">previewUrl</span></span>|<span data-ttu-id="18a0e-156">String</span><span class="sxs-lookup"><span data-stu-id="18a0e-156">String</span></span>|<span data-ttu-id="18a0e-157">Применяется только вложения ссылку объекта на изображении - URL-адрес для получения изображения для предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="18a0e-157">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="18a0e-158">Используйте **thumbnailUrl** и **previewUrl** только в том случае, когда **sourceUrl** определяет файл изображения.</span><span class="sxs-lookup"><span data-stu-id="18a0e-158">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="18a0e-159">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="18a0e-159">Optional.</span></span>|
|<span data-ttu-id="18a0e-160">providerType</span><span class="sxs-lookup"><span data-stu-id="18a0e-160">providerType</span></span>|<span data-ttu-id="18a0e-161">ReferenceAttachmentProviders</span><span class="sxs-lookup"><span data-stu-id="18a0e-161">ReferenceAttachmentProviders</span></span>|<span data-ttu-id="18a0e-162">Тип поставщика, который поддерживает вложение в этом contentType.</span><span class="sxs-lookup"><span data-stu-id="18a0e-162">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="18a0e-163">Возможные значения: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span><span class="sxs-lookup"><span data-stu-id="18a0e-163">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="18a0e-164">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="18a0e-164">Optional.</span></span>|
|<span data-ttu-id="18a0e-165">size</span><span class="sxs-lookup"><span data-stu-id="18a0e-165">size</span></span>|<span data-ttu-id="18a0e-166">Int32</span><span class="sxs-lookup"><span data-stu-id="18a0e-166">Int32</span></span>|<span data-ttu-id="18a0e-167">Размер метаданных в байтах, которые хранятся на сообщение для вложения ссылку.</span><span class="sxs-lookup"><span data-stu-id="18a0e-167">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="18a0e-168">Это значение не отображает фактический размер файла.</span><span class="sxs-lookup"><span data-stu-id="18a0e-168">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="18a0e-169">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="18a0e-169">Optional.</span></span>|
|<span data-ttu-id="18a0e-170">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="18a0e-170">sourceUrl</span></span>|<span data-ttu-id="18a0e-171">String</span><span class="sxs-lookup"><span data-stu-id="18a0e-171">String</span></span>|<span data-ttu-id="18a0e-172">URL-адрес для получения содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="18a0e-172">URL to get the attachment content.</span></span> <span data-ttu-id="18a0e-173">Если это URL-адрес в папку, для папки для правильного отображения в Outlook или Outlook в Интернете, задайте его **isFolder** имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="18a0e-173">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="18a0e-174">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="18a0e-174">Required.</span></span>|
|<span data-ttu-id="18a0e-175">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="18a0e-175">thumbnailUrl</span></span>|<span data-ttu-id="18a0e-176">String</span><span class="sxs-lookup"><span data-stu-id="18a0e-176">String</span></span>|<span data-ttu-id="18a0e-177">Применяется только вложения ссылку объекта на изображении - URL-адрес для получения эскизное изображение.</span><span class="sxs-lookup"><span data-stu-id="18a0e-177">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="18a0e-178">Используйте **thumbnailUrl** и **previewUrl** только в том случае, когда **sourceUrl** определяет файл изображения.</span><span class="sxs-lookup"><span data-stu-id="18a0e-178">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="18a0e-179">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="18a0e-179">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18a0e-180">Связи</span><span class="sxs-lookup"><span data-stu-id="18a0e-180">Relationships</span></span>
<span data-ttu-id="18a0e-181">Нет</span><span class="sxs-lookup"><span data-stu-id="18a0e-181">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="18a0e-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18a0e-182">JSON representation</span></span>

<span data-ttu-id="18a0e-183">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18a0e-183">Here is a JSON representation of the resource</span></span>

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
