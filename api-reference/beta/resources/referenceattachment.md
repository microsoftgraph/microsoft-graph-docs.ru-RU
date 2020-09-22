---
title: Тип ресурса referenceAttachment
description: 'Ссылка на папку или файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или других поддерживаемых местах хранения, подключенных к '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 976b2156e5d420302a473c4c6ef0c1e0e538f52d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073506"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="2daa7-103">Тип ресурса referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="2daa7-103">referenceAttachment resource type</span></span>

<span data-ttu-id="2daa7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2daa7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2daa7-105">Ссылка на папку или файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или других поддерживаемых местах хранения, прикрепленных к [событию](../resources/event.md), [сообщению](../resources/message.md)или [записи](../resources/post.md) .</span><span class="sxs-lookup"><span data-stu-id="2daa7-105">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="2daa7-106">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="2daa7-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2daa7-107">Методы</span><span class="sxs-lookup"><span data-stu-id="2daa7-107">Methods</span></span>

| <span data-ttu-id="2daa7-108">Метод</span><span class="sxs-lookup"><span data-stu-id="2daa7-108">Method</span></span>       | <span data-ttu-id="2daa7-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2daa7-109">Return Type</span></span>  |<span data-ttu-id="2daa7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2daa7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2daa7-111">[получение](../api/attachment-get.md);</span><span class="sxs-lookup"><span data-stu-id="2daa7-111">[Get](../api/attachment-get.md)</span></span> | [<span data-ttu-id="2daa7-112">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="2daa7-112">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="2daa7-113">Чтение свойств и связей объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="2daa7-113">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="2daa7-114">Удаление</span><span class="sxs-lookup"><span data-stu-id="2daa7-114">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="2daa7-115">Нет</span><span class="sxs-lookup"><span data-stu-id="2daa7-115">None</span></span> |<span data-ttu-id="2daa7-116">Удаление объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="2daa7-116">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2daa7-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="2daa7-117">Properties</span></span>
| <span data-ttu-id="2daa7-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="2daa7-118">Property</span></span>     | <span data-ttu-id="2daa7-119">Тип</span><span class="sxs-lookup"><span data-stu-id="2daa7-119">Type</span></span>   |<span data-ttu-id="2daa7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2daa7-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2daa7-121">contentType</span><span class="sxs-lookup"><span data-stu-id="2daa7-121">contentType</span></span>|<span data-ttu-id="2daa7-122">String</span><span class="sxs-lookup"><span data-stu-id="2daa7-122">String</span></span>|<span data-ttu-id="2daa7-123">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="2daa7-123">The content type of the attachment.</span></span> <span data-ttu-id="2daa7-124">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="2daa7-124">Optional.</span></span>|
|<span data-ttu-id="2daa7-125">id</span><span class="sxs-lookup"><span data-stu-id="2daa7-125">id</span></span>|<span data-ttu-id="2daa7-126">String</span><span class="sxs-lookup"><span data-stu-id="2daa7-126">String</span></span>|<span data-ttu-id="2daa7-p102">Идентификатор вложения.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2daa7-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="2daa7-129">isFolder</span><span class="sxs-lookup"><span data-stu-id="2daa7-129">isFolder</span></span>|<span data-ttu-id="2daa7-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="2daa7-130">Boolean</span></span>|<span data-ttu-id="2daa7-131">Указывает, является ли вложение ссылкой на папку.</span><span class="sxs-lookup"><span data-stu-id="2daa7-131">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="2daa7-132">Если **sourceUrl** является ссылкой на папку, необходимо задать для этого параметра значение true.</span><span class="sxs-lookup"><span data-stu-id="2daa7-132">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="2daa7-133">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="2daa7-133">Optional.</span></span>|
|<span data-ttu-id="2daa7-134">isInline</span><span class="sxs-lookup"><span data-stu-id="2daa7-134">isInline</span></span>|<span data-ttu-id="2daa7-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="2daa7-135">Boolean</span></span>|<span data-ttu-id="2daa7-136">Значение true указывает, что вложение встроено в содержимое объекта.</span><span class="sxs-lookup"><span data-stu-id="2daa7-136">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="2daa7-137">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="2daa7-137">Optional.</span></span>|
|<span data-ttu-id="2daa7-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2daa7-138">lastModifiedDateTime</span></span>|<span data-ttu-id="2daa7-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2daa7-139">DateTimeOffset</span></span>|<span data-ttu-id="2daa7-140">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="2daa7-140">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="2daa7-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="2daa7-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2daa7-142">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2daa7-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="2daa7-143">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="2daa7-143">Optional.</span></span>|
|<span data-ttu-id="2daa7-144">name</span><span class="sxs-lookup"><span data-stu-id="2daa7-144">name</span></span>|<span data-ttu-id="2daa7-145">String</span><span class="sxs-lookup"><span data-stu-id="2daa7-145">String</span></span>|<span data-ttu-id="2daa7-146">Текст, который отображается под значком, представляет внедренное вложение.</span><span class="sxs-lookup"><span data-stu-id="2daa7-146">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="2daa7-147">Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="2daa7-147">This does not need to be the actual file name.</span></span> <span data-ttu-id="2daa7-148">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="2daa7-148">Required.</span></span>|
|<span data-ttu-id="2daa7-149">права</span><span class="sxs-lookup"><span data-stu-id="2daa7-149">permission</span></span>|<span data-ttu-id="2daa7-150">referenceAttachmentPermission</span><span class="sxs-lookup"><span data-stu-id="2daa7-150">referenceAttachmentPermission</span></span>|<span data-ttu-id="2daa7-151">Задает разрешения, предоставленные для вложения, по типу поставщика в **ProviderType**.</span><span class="sxs-lookup"><span data-stu-id="2daa7-151">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="2daa7-152">Возможные значения: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span><span class="sxs-lookup"><span data-stu-id="2daa7-152">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="2daa7-153">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="2daa7-153">Optional.</span></span>|
|<span data-ttu-id="2daa7-154">previewUrl</span><span class="sxs-lookup"><span data-stu-id="2daa7-154">previewUrl</span></span>|<span data-ttu-id="2daa7-155">String</span><span class="sxs-lookup"><span data-stu-id="2daa7-155">String</span></span>|<span data-ttu-id="2daa7-156">Применяется только к вложению ссылки на URL-адрес изображения для получения изображения предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="2daa7-156">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="2daa7-157">Используйте **thumbnailUrl** и **previewUrl** только в том случае, если **sourceUrl** определяет файл изображения.</span><span class="sxs-lookup"><span data-stu-id="2daa7-157">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="2daa7-158">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="2daa7-158">Optional.</span></span>|
|<span data-ttu-id="2daa7-159">providerType</span><span class="sxs-lookup"><span data-stu-id="2daa7-159">providerType</span></span>|<span data-ttu-id="2daa7-160">Перечислений — referenceattachmentprovider</span><span class="sxs-lookup"><span data-stu-id="2daa7-160">referenceAttachmentProvider</span></span>|<span data-ttu-id="2daa7-161">Тип поставщика, который поддерживает вложение этого contentType.</span><span class="sxs-lookup"><span data-stu-id="2daa7-161">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="2daa7-162">Возможные значения: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span><span class="sxs-lookup"><span data-stu-id="2daa7-162">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="2daa7-163">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="2daa7-163">Optional.</span></span>|
|<span data-ttu-id="2daa7-164">size</span><span class="sxs-lookup"><span data-stu-id="2daa7-164">size</span></span>|<span data-ttu-id="2daa7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2daa7-165">Int32</span></span>|<span data-ttu-id="2daa7-166">Размер метаданных в байтах, хранящихся в сообщении для вложения ссылки.</span><span class="sxs-lookup"><span data-stu-id="2daa7-166">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="2daa7-167">Это значение не отображает фактический размер файла.</span><span class="sxs-lookup"><span data-stu-id="2daa7-167">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="2daa7-168">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="2daa7-168">Optional.</span></span>|
|<span data-ttu-id="2daa7-169">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="2daa7-169">sourceUrl</span></span>|<span data-ttu-id="2daa7-170">String</span><span class="sxs-lookup"><span data-stu-id="2daa7-170">String</span></span>|<span data-ttu-id="2daa7-171">URL-адрес для получения содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="2daa7-171">URL to get the attachment content.</span></span> <span data-ttu-id="2daa7-172">Если это URL-адрес папки, то для правильного отображения папки в Outlook или Outlook в **Интернете установите для параметра IsTrue значение true** .</span><span class="sxs-lookup"><span data-stu-id="2daa7-172">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="2daa7-173">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="2daa7-173">Required.</span></span>|
|<span data-ttu-id="2daa7-174">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="2daa7-174">thumbnailUrl</span></span>|<span data-ttu-id="2daa7-175">String</span><span class="sxs-lookup"><span data-stu-id="2daa7-175">String</span></span>|<span data-ttu-id="2daa7-176">Применяется только к вложению ссылки на URL-адрес изображения для получения эскиза.</span><span class="sxs-lookup"><span data-stu-id="2daa7-176">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="2daa7-177">Используйте **thumbnailUrl** и **previewUrl** только в том случае, если **sourceUrl** определяет файл изображения.</span><span class="sxs-lookup"><span data-stu-id="2daa7-177">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="2daa7-178">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="2daa7-178">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2daa7-179">Отношения</span><span class="sxs-lookup"><span data-stu-id="2daa7-179">Relationships</span></span>
<span data-ttu-id="2daa7-180">Нет</span><span class="sxs-lookup"><span data-stu-id="2daa7-180">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="2daa7-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2daa7-181">JSON representation</span></span>

<span data-ttu-id="2daa7-182">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2daa7-182">Here is a JSON representation of the resource</span></span>

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


