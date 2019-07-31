---
title: Тип ресурса referenceAttachment
description: 'Ссылка на папку или файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или других поддерживаемых местах хранения, подключенных к '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ef3e2dd5292ee018c0b72c29c8bd6c33fed00f11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008714"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="febff-103">Тип ресурса referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="febff-103">referenceAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="febff-104">Ссылка на папку или файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или других поддерживаемых местах хранения, прикрепленных к [событию](../resources/event.md), сообщению, [](../resources/message.md)задаче [Outlook](../resources/outlooktask.md)или [POST](../resources/post.md) .</span><span class="sxs-lookup"><span data-stu-id="febff-104">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="febff-105">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="febff-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="febff-106">Методы</span><span class="sxs-lookup"><span data-stu-id="febff-106">Methods</span></span>

| <span data-ttu-id="febff-107">Метод</span><span class="sxs-lookup"><span data-stu-id="febff-107">Method</span></span>       | <span data-ttu-id="febff-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="febff-108">Return Type</span></span>  |<span data-ttu-id="febff-109">Описание</span><span class="sxs-lookup"><span data-stu-id="febff-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="febff-110">Получение</span><span class="sxs-lookup"><span data-stu-id="febff-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="febff-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="febff-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="febff-112">Чтение свойств и связей объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="febff-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="febff-113">Удаление</span><span class="sxs-lookup"><span data-stu-id="febff-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="febff-114">Нет</span><span class="sxs-lookup"><span data-stu-id="febff-114">None</span></span> |<span data-ttu-id="febff-115">Удаление объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="febff-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="febff-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="febff-116">Properties</span></span>
| <span data-ttu-id="febff-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="febff-117">Property</span></span>     | <span data-ttu-id="febff-118">Тип</span><span class="sxs-lookup"><span data-stu-id="febff-118">Type</span></span>   |<span data-ttu-id="febff-119">Описание</span><span class="sxs-lookup"><span data-stu-id="febff-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="febff-120">contentType</span><span class="sxs-lookup"><span data-stu-id="febff-120">contentType</span></span>|<span data-ttu-id="febff-121">String</span><span class="sxs-lookup"><span data-stu-id="febff-121">String</span></span>|<span data-ttu-id="febff-122">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="febff-122">The content type of the attachment.</span></span> <span data-ttu-id="febff-123">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="febff-123">Optional.</span></span>|
|<span data-ttu-id="febff-124">id</span><span class="sxs-lookup"><span data-stu-id="febff-124">id</span></span>|<span data-ttu-id="febff-125">Строка</span><span class="sxs-lookup"><span data-stu-id="febff-125">String</span></span>|<span data-ttu-id="febff-p102">Идентификатор вложения.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="febff-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="febff-128">isFolder</span><span class="sxs-lookup"><span data-stu-id="febff-128">isFolder</span></span>|<span data-ttu-id="febff-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="febff-129">Boolean</span></span>|<span data-ttu-id="febff-130">Указывает, является ли вложение ссылкой на папку.</span><span class="sxs-lookup"><span data-stu-id="febff-130">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="febff-131">Если **sourceUrl** является ссылкой на папку, необходимо задать для этого параметра значение true.</span><span class="sxs-lookup"><span data-stu-id="febff-131">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="febff-132">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="febff-132">Optional.</span></span>|
|<span data-ttu-id="febff-133">isInline</span><span class="sxs-lookup"><span data-stu-id="febff-133">isInline</span></span>|<span data-ttu-id="febff-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="febff-134">Boolean</span></span>|<span data-ttu-id="febff-135">Значение true указывает, что вложение встроено в содержимое объекта.</span><span class="sxs-lookup"><span data-stu-id="febff-135">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="febff-136">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="febff-136">Optional.</span></span>|
|<span data-ttu-id="febff-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="febff-137">lastModifiedDateTime</span></span>|<span data-ttu-id="febff-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="febff-138">DateTimeOffset</span></span>|<span data-ttu-id="febff-139">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="febff-139">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="febff-140">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="febff-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="febff-141">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="febff-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="febff-142">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="febff-142">Optional.</span></span>|
|<span data-ttu-id="febff-143">name</span><span class="sxs-lookup"><span data-stu-id="febff-143">name</span></span>|<span data-ttu-id="febff-144">String</span><span class="sxs-lookup"><span data-stu-id="febff-144">String</span></span>|<span data-ttu-id="febff-145">Текст, который отображается под значком, представляет внедренное вложение.</span><span class="sxs-lookup"><span data-stu-id="febff-145">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="febff-146">Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="febff-146">This does not need to be the actual file name.</span></span> <span data-ttu-id="febff-147">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="febff-147">Required.</span></span>|
|<span data-ttu-id="febff-148">permission</span><span class="sxs-lookup"><span data-stu-id="febff-148">permission</span></span>|<span data-ttu-id="febff-149">referenceAttachmentPermission</span><span class="sxs-lookup"><span data-stu-id="febff-149">referenceAttachmentPermission</span></span>|<span data-ttu-id="febff-150">Задает разрешения, предоставленные для вложения, по типу поставщика в **ProviderType**.</span><span class="sxs-lookup"><span data-stu-id="febff-150">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="febff-151">Возможные значения: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span><span class="sxs-lookup"><span data-stu-id="febff-151">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="febff-152">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="febff-152">Optional.</span></span>|
|<span data-ttu-id="febff-153">previewUrl</span><span class="sxs-lookup"><span data-stu-id="febff-153">previewUrl</span></span>|<span data-ttu-id="febff-154">String</span><span class="sxs-lookup"><span data-stu-id="febff-154">String</span></span>|<span data-ttu-id="febff-155">Применяется только к вложению ссылки на URL-адрес изображения для получения изображения предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="febff-155">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="febff-156">Используйте **thumbnailUrl** и **previewUrl** только в том случае, если **sourceUrl** определяет файл изображения.</span><span class="sxs-lookup"><span data-stu-id="febff-156">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="febff-157">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="febff-157">Optional.</span></span>|
|<span data-ttu-id="febff-158">providerType</span><span class="sxs-lookup"><span data-stu-id="febff-158">providerType</span></span>|<span data-ttu-id="febff-159">Перечислений — referenceattachmentprovider</span><span class="sxs-lookup"><span data-stu-id="febff-159">referenceAttachmentProvider</span></span>|<span data-ttu-id="febff-160">Тип поставщика, который поддерживает вложение этого contentType.</span><span class="sxs-lookup"><span data-stu-id="febff-160">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="febff-161">Возможные значения: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span><span class="sxs-lookup"><span data-stu-id="febff-161">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="febff-162">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="febff-162">Optional.</span></span>|
|<span data-ttu-id="febff-163">size</span><span class="sxs-lookup"><span data-stu-id="febff-163">size</span></span>|<span data-ttu-id="febff-164">Int32</span><span class="sxs-lookup"><span data-stu-id="febff-164">Int32</span></span>|<span data-ttu-id="febff-165">Размер метаданных в байтах, хранящихся в сообщении для вложения ссылки.</span><span class="sxs-lookup"><span data-stu-id="febff-165">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="febff-166">Это значение не отображает фактический размер файла.</span><span class="sxs-lookup"><span data-stu-id="febff-166">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="febff-167">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="febff-167">Optional.</span></span>|
|<span data-ttu-id="febff-168">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="febff-168">sourceUrl</span></span>|<span data-ttu-id="febff-169">String</span><span class="sxs-lookup"><span data-stu-id="febff-169">String</span></span>|<span data-ttu-id="febff-170">URL-адрес для получения содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="febff-170">URL to get the attachment content.</span></span> <span data-ttu-id="febff-171">Если это URL-адрес папки, то для правильного отображения папки в Outlook или Outlook в Интернете установите для параметра IsTrue значение true. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="febff-171">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="febff-172">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="febff-172">Required.</span></span>|
|<span data-ttu-id="febff-173">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="febff-173">thumbnailUrl</span></span>|<span data-ttu-id="febff-174">String</span><span class="sxs-lookup"><span data-stu-id="febff-174">String</span></span>|<span data-ttu-id="febff-175">Применяется только к вложению ссылки на URL-адрес изображения для получения эскиза.</span><span class="sxs-lookup"><span data-stu-id="febff-175">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="febff-176">Используйте **thumbnailUrl** и **previewUrl** только в том случае, если **sourceUrl** определяет файл изображения.</span><span class="sxs-lookup"><span data-stu-id="febff-176">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="febff-177">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="febff-177">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="febff-178">Отношения</span><span class="sxs-lookup"><span data-stu-id="febff-178">Relationships</span></span>
<span data-ttu-id="febff-179">Нет</span><span class="sxs-lookup"><span data-stu-id="febff-179">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="febff-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="febff-180">JSON representation</span></span>

<span data-ttu-id="febff-181">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="febff-181">Here is a JSON representation of the resource</span></span>

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
