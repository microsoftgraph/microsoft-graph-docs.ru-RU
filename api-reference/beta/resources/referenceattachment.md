---
title: Тип ресурса referenceAttachment
description: 'Ссылка на папку или файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или других поддерживаемых местах хранения, подключенных к '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: d4e9616d1430c3c3789f42cb023583dfdb452d6d
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/09/2020
ms.locfileid: "40995023"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="cc5f6-103">Тип ресурса referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="cc5f6-103">referenceAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc5f6-104">Ссылка на папку или файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или других поддерживаемых местах хранения, прикрепленных к [событию](../resources/event.md), [сообщению](../resources/message.md)или [записи](../resources/post.md) .</span><span class="sxs-lookup"><span data-stu-id="cc5f6-104">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="cc5f6-105">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="cc5f6-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="cc5f6-106">Методы</span><span class="sxs-lookup"><span data-stu-id="cc5f6-106">Methods</span></span>

| <span data-ttu-id="cc5f6-107">Метод</span><span class="sxs-lookup"><span data-stu-id="cc5f6-107">Method</span></span>       | <span data-ttu-id="cc5f6-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cc5f6-108">Return Type</span></span>  |<span data-ttu-id="cc5f6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cc5f6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc5f6-110">[получение](../api/attachment-get.md);</span><span class="sxs-lookup"><span data-stu-id="cc5f6-110">[Get](../api/attachment-get.md)</span></span> | [<span data-ttu-id="cc5f6-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="cc5f6-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="cc5f6-112">Чтение свойств и связей объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-112">Read properties and relationships of referenceAttachment object.</span></span>|
|<span data-ttu-id="cc5f6-113">[удаление](../api/attachment-delete.md);</span><span class="sxs-lookup"><span data-stu-id="cc5f6-113">[Delete](../api/attachment-delete.md)</span></span> | <span data-ttu-id="cc5f6-114">Нет</span><span class="sxs-lookup"><span data-stu-id="cc5f6-114">None</span></span> |<span data-ttu-id="cc5f6-115">Удаление объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cc5f6-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc5f6-116">Properties</span></span>
| <span data-ttu-id="cc5f6-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc5f6-117">Property</span></span>     | <span data-ttu-id="cc5f6-118">Тип</span><span class="sxs-lookup"><span data-stu-id="cc5f6-118">Type</span></span>   |<span data-ttu-id="cc5f6-119">Описание</span><span class="sxs-lookup"><span data-stu-id="cc5f6-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc5f6-120">contentType</span><span class="sxs-lookup"><span data-stu-id="cc5f6-120">contentType</span></span>|<span data-ttu-id="cc5f6-121">String</span><span class="sxs-lookup"><span data-stu-id="cc5f6-121">String</span></span>|<span data-ttu-id="cc5f6-122">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-122">The content type of the attachment.</span></span> <span data-ttu-id="cc5f6-123">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-123">Optional.</span></span>|
|<span data-ttu-id="cc5f6-124">id</span><span class="sxs-lookup"><span data-stu-id="cc5f6-124">id</span></span>|<span data-ttu-id="cc5f6-125">Строка</span><span class="sxs-lookup"><span data-stu-id="cc5f6-125">String</span></span>|<span data-ttu-id="cc5f6-p102">Идентификатор вложения.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="cc5f6-128">isFolder</span><span class="sxs-lookup"><span data-stu-id="cc5f6-128">isFolder</span></span>|<span data-ttu-id="cc5f6-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc5f6-129">Boolean</span></span>|<span data-ttu-id="cc5f6-130">Указывает, является ли вложение ссылкой на папку.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-130">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="cc5f6-131">Если **sourceUrl** является ссылкой на папку, необходимо задать для этого параметра значение true.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-131">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="cc5f6-132">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-132">Optional.</span></span>|
|<span data-ttu-id="cc5f6-133">isInline</span><span class="sxs-lookup"><span data-stu-id="cc5f6-133">isInline</span></span>|<span data-ttu-id="cc5f6-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc5f6-134">Boolean</span></span>|<span data-ttu-id="cc5f6-135">Значение true указывает, что вложение встроено в содержимое объекта.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-135">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="cc5f6-136">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-136">Optional.</span></span>|
|<span data-ttu-id="cc5f6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc5f6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="cc5f6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc5f6-138">DateTimeOffset</span></span>|<span data-ttu-id="cc5f6-139">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-139">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="cc5f6-140">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="cc5f6-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cc5f6-141">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="cc5f6-142">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-142">Optional.</span></span>|
|<span data-ttu-id="cc5f6-143">name</span><span class="sxs-lookup"><span data-stu-id="cc5f6-143">name</span></span>|<span data-ttu-id="cc5f6-144">String</span><span class="sxs-lookup"><span data-stu-id="cc5f6-144">String</span></span>|<span data-ttu-id="cc5f6-145">Текст, который отображается под значком, представляет внедренное вложение.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-145">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="cc5f6-146">Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-146">This does not need to be the actual file name.</span></span> <span data-ttu-id="cc5f6-147">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-147">Required.</span></span>|
|<span data-ttu-id="cc5f6-148">права</span><span class="sxs-lookup"><span data-stu-id="cc5f6-148">permission</span></span>|<span data-ttu-id="cc5f6-149">referenceAttachmentPermission</span><span class="sxs-lookup"><span data-stu-id="cc5f6-149">referenceAttachmentPermission</span></span>|<span data-ttu-id="cc5f6-150">Задает разрешения, предоставленные для вложения, по типу поставщика в **ProviderType**.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-150">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="cc5f6-151">Возможные значения: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-151">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="cc5f6-152">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-152">Optional.</span></span>|
|<span data-ttu-id="cc5f6-153">previewUrl</span><span class="sxs-lookup"><span data-stu-id="cc5f6-153">previewUrl</span></span>|<span data-ttu-id="cc5f6-154">String</span><span class="sxs-lookup"><span data-stu-id="cc5f6-154">String</span></span>|<span data-ttu-id="cc5f6-155">Применяется только к вложению ссылки на URL-адрес изображения для получения изображения предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-155">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="cc5f6-156">Используйте **thumbnailUrl** и **previewUrl** только в том случае, если **sourceUrl** определяет файл изображения.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-156">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="cc5f6-157">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-157">Optional.</span></span>|
|<span data-ttu-id="cc5f6-158">providerType</span><span class="sxs-lookup"><span data-stu-id="cc5f6-158">providerType</span></span>|<span data-ttu-id="cc5f6-159">Перечислений — referenceattachmentprovider</span><span class="sxs-lookup"><span data-stu-id="cc5f6-159">referenceAttachmentProvider</span></span>|<span data-ttu-id="cc5f6-160">Тип поставщика, который поддерживает вложение этого contentType.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-160">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="cc5f6-161">Возможные значения: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-161">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="cc5f6-162">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-162">Optional.</span></span>|
|<span data-ttu-id="cc5f6-163">size</span><span class="sxs-lookup"><span data-stu-id="cc5f6-163">size</span></span>|<span data-ttu-id="cc5f6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="cc5f6-164">Int32</span></span>|<span data-ttu-id="cc5f6-165">Размер метаданных в байтах, хранящихся в сообщении для вложения ссылки.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-165">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="cc5f6-166">Это значение не отображает фактический размер файла.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-166">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="cc5f6-167">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-167">Optional.</span></span>|
|<span data-ttu-id="cc5f6-168">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="cc5f6-168">sourceUrl</span></span>|<span data-ttu-id="cc5f6-169">String</span><span class="sxs-lookup"><span data-stu-id="cc5f6-169">String</span></span>|<span data-ttu-id="cc5f6-170">URL-адрес для получения содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-170">URL to get the attachment content.</span></span> <span data-ttu-id="cc5f6-171">Если это URL-адрес папки, то для правильного отображения папки в Outlook или Outlook в **Интернете установите для параметра IsTrue значение true** .</span><span class="sxs-lookup"><span data-stu-id="cc5f6-171">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="cc5f6-172">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-172">Required.</span></span>|
|<span data-ttu-id="cc5f6-173">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="cc5f6-173">thumbnailUrl</span></span>|<span data-ttu-id="cc5f6-174">String</span><span class="sxs-lookup"><span data-stu-id="cc5f6-174">String</span></span>|<span data-ttu-id="cc5f6-175">Применяется только к вложению ссылки на URL-адрес изображения для получения эскиза.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-175">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="cc5f6-176">Используйте **thumbnailUrl** и **previewUrl** только в том случае, если **sourceUrl** определяет файл изображения.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-176">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="cc5f6-177">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-177">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc5f6-178">Отношения</span><span class="sxs-lookup"><span data-stu-id="cc5f6-178">Relationships</span></span>
<span data-ttu-id="cc5f6-179">Нет</span><span class="sxs-lookup"><span data-stu-id="cc5f6-179">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="cc5f6-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc5f6-180">JSON representation</span></span>

<span data-ttu-id="cc5f6-181">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc5f6-181">Here is a JSON representation of the resource</span></span>

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
