---
title: Тип ресурса referenceAttachment
description: 'Ссылка на папку или файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или других поддерживаемых хранилищах, присоединенных к '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: e0c3723648710fb1640927fad10e0847e1e155a6
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721322"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="8f619-103">Тип ресурса referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="8f619-103">referenceAttachment resource type</span></span>

<span data-ttu-id="8f619-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f619-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f619-105">Ссылка на папку или файл (например, текстовый файл или документ Word) на облачном диске OneDrive для [](../resources/message.md)бизнеса или других поддерживаемых хранилищах, присоединенных к событию, [](../resources/event.md)сообщению или сообщению. [](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="8f619-105">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="8f619-106">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="8f619-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8f619-107">Методы</span><span class="sxs-lookup"><span data-stu-id="8f619-107">Methods</span></span>

| <span data-ttu-id="8f619-108">Метод</span><span class="sxs-lookup"><span data-stu-id="8f619-108">Method</span></span>       | <span data-ttu-id="8f619-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8f619-109">Return Type</span></span>  |<span data-ttu-id="8f619-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8f619-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f619-111">[получение](../api/attachment-get.md);</span><span class="sxs-lookup"><span data-stu-id="8f619-111">[Get](../api/attachment-get.md)</span></span> | [<span data-ttu-id="8f619-112">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="8f619-112">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="8f619-113">Чтение свойств и связей объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="8f619-113">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="8f619-114">Удаление</span><span class="sxs-lookup"><span data-stu-id="8f619-114">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="8f619-115">Нет</span><span class="sxs-lookup"><span data-stu-id="8f619-115">None</span></span> |<span data-ttu-id="8f619-116">Удаление объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="8f619-116">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8f619-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f619-117">Properties</span></span>
| <span data-ttu-id="8f619-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f619-118">Property</span></span>     | <span data-ttu-id="8f619-119">Тип</span><span class="sxs-lookup"><span data-stu-id="8f619-119">Type</span></span>   |<span data-ttu-id="8f619-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8f619-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f619-121">contentType</span><span class="sxs-lookup"><span data-stu-id="8f619-121">contentType</span></span>|<span data-ttu-id="8f619-122">String</span><span class="sxs-lookup"><span data-stu-id="8f619-122">String</span></span>|<span data-ttu-id="8f619-123">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="8f619-123">The content type of the attachment.</span></span> <span data-ttu-id="8f619-124">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="8f619-124">Optional.</span></span>|
|<span data-ttu-id="8f619-125">id</span><span class="sxs-lookup"><span data-stu-id="8f619-125">id</span></span>|<span data-ttu-id="8f619-126">String</span><span class="sxs-lookup"><span data-stu-id="8f619-126">String</span></span>|<span data-ttu-id="8f619-p102">Идентификатор вложения.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8f619-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="8f619-129">isFolder</span><span class="sxs-lookup"><span data-stu-id="8f619-129">isFolder</span></span>|<span data-ttu-id="8f619-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f619-130">Boolean</span></span>|<span data-ttu-id="8f619-131">Указывает, является ли вложение ссылкой на папку.</span><span class="sxs-lookup"><span data-stu-id="8f619-131">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="8f619-132">Необходимо установить это, если **sourceUrl** является ссылкой на папку.</span><span class="sxs-lookup"><span data-stu-id="8f619-132">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="8f619-133">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="8f619-133">Optional.</span></span>|
|<span data-ttu-id="8f619-134">isInline</span><span class="sxs-lookup"><span data-stu-id="8f619-134">isInline</span></span>|<span data-ttu-id="8f619-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f619-135">Boolean</span></span>|<span data-ttu-id="8f619-136">Значение true указывает, что вложение встроено в содержимое объекта.</span><span class="sxs-lookup"><span data-stu-id="8f619-136">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="8f619-137">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="8f619-137">Optional.</span></span>|
|<span data-ttu-id="8f619-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f619-138">lastModifiedDateTime</span></span>|<span data-ttu-id="8f619-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f619-139">DateTimeOffset</span></span>|<span data-ttu-id="8f619-140">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="8f619-140">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="8f619-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8f619-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8f619-142">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8f619-142">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="8f619-143">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="8f619-143">Optional.</span></span>|
|<span data-ttu-id="8f619-144">name</span><span class="sxs-lookup"><span data-stu-id="8f619-144">name</span></span>|<span data-ttu-id="8f619-145">String</span><span class="sxs-lookup"><span data-stu-id="8f619-145">String</span></span>|<span data-ttu-id="8f619-146">Текст, который отображается под значком, представляет внедренное вложение.</span><span class="sxs-lookup"><span data-stu-id="8f619-146">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="8f619-147">Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="8f619-147">This does not need to be the actual file name.</span></span> <span data-ttu-id="8f619-148">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="8f619-148">Required.</span></span>|
|<span data-ttu-id="8f619-149">разрешение</span><span class="sxs-lookup"><span data-stu-id="8f619-149">permission</span></span>|<span data-ttu-id="8f619-150">referenceAttachmentPermission</span><span class="sxs-lookup"><span data-stu-id="8f619-150">referenceAttachmentPermission</span></span>|<span data-ttu-id="8f619-151">Указывает разрешения, предоставленные для вложения типом поставщика в **providerType.**</span><span class="sxs-lookup"><span data-stu-id="8f619-151">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="8f619-152">Возможные значения: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span><span class="sxs-lookup"><span data-stu-id="8f619-152">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="8f619-153">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="8f619-153">Optional.</span></span>|
|<span data-ttu-id="8f619-154">previewUrl</span><span class="sxs-lookup"><span data-stu-id="8f619-154">previewUrl</span></span>|<span data-ttu-id="8f619-155">String</span><span class="sxs-lookup"><span data-stu-id="8f619-155">String</span></span>|<span data-ttu-id="8f619-156">Применяется только к ссылке на вложение изображения — URL-адрес для получения изображения предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="8f619-156">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="8f619-157">Используйте **thumbnailUrl и** **previewUrl** только тогда, когда **sourceUrl** идентифицирует файл изображений.</span><span class="sxs-lookup"><span data-stu-id="8f619-157">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="8f619-158">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="8f619-158">Optional.</span></span>|
|<span data-ttu-id="8f619-159">providerType</span><span class="sxs-lookup"><span data-stu-id="8f619-159">providerType</span></span>|<span data-ttu-id="8f619-160">referenceAttachmentProvider</span><span class="sxs-lookup"><span data-stu-id="8f619-160">referenceAttachmentProvider</span></span>|<span data-ttu-id="8f619-161">Тип поставщика, который поддерживает вложение этого contentType.</span><span class="sxs-lookup"><span data-stu-id="8f619-161">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="8f619-162">Возможные значения: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span><span class="sxs-lookup"><span data-stu-id="8f619-162">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="8f619-163">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="8f619-163">Optional.</span></span>|
|<span data-ttu-id="8f619-164">size</span><span class="sxs-lookup"><span data-stu-id="8f619-164">size</span></span>|<span data-ttu-id="8f619-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8f619-165">Int32</span></span>|<span data-ttu-id="8f619-166">Размер метаданных в bytes, хранимых в сообщении для эталонного вложения.</span><span class="sxs-lookup"><span data-stu-id="8f619-166">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="8f619-167">Это значение не отображает фактический размер файла.</span><span class="sxs-lookup"><span data-stu-id="8f619-167">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="8f619-168">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="8f619-168">Optional.</span></span>|
|<span data-ttu-id="8f619-169">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="8f619-169">sourceUrl</span></span>|<span data-ttu-id="8f619-170">String</span><span class="sxs-lookup"><span data-stu-id="8f619-170">String</span></span>|<span data-ttu-id="8f619-171">URL-адрес для получения содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="8f619-171">URL to get the attachment content.</span></span> <span data-ttu-id="8f619-172">Если это URL-адрес папки, то для правильного отображения папки в Outlook или Outlook в Интернете заданной **являетсяFolder** to true.</span><span class="sxs-lookup"><span data-stu-id="8f619-172">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="8f619-173">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="8f619-173">Required.</span></span>|
|<span data-ttu-id="8f619-174">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="8f619-174">thumbnailUrl</span></span>|<span data-ttu-id="8f619-175">String</span><span class="sxs-lookup"><span data-stu-id="8f619-175">String</span></span>|<span data-ttu-id="8f619-176">Применяется только к ссылке на вложение изображения — URL-адрес для получения эскизного изображения.</span><span class="sxs-lookup"><span data-stu-id="8f619-176">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="8f619-177">Используйте **thumbnailUrl и** **previewUrl** только тогда, когда **sourceUrl** идентифицирует файл изображений.</span><span class="sxs-lookup"><span data-stu-id="8f619-177">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="8f619-178">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="8f619-178">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f619-179">Связи</span><span class="sxs-lookup"><span data-stu-id="8f619-179">Relationships</span></span>
<span data-ttu-id="8f619-180">Нет</span><span class="sxs-lookup"><span data-stu-id="8f619-180">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="8f619-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f619-181">JSON representation</span></span>

<span data-ttu-id="8f619-182">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f619-182">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
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
<!--
{
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


