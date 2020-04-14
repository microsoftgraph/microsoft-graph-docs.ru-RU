---
title: Тип ресурса referenceAttachment
description: 'Ссылка на папку или файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или других поддерживаемых местах хранения, подключенных к '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 426d746305b2a8418fb30515720d888226d3da74
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462214"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="c8384-103">Тип ресурса referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="c8384-103">referenceAttachment resource type</span></span>

<span data-ttu-id="c8384-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8384-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8384-105">Ссылка на папку или файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или других поддерживаемых местах хранения, прикрепленных к [событию](../resources/event.md), [сообщению](../resources/message.md)или [записи](../resources/post.md) .</span><span class="sxs-lookup"><span data-stu-id="c8384-105">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="c8384-106">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="c8384-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c8384-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c8384-107">Methods</span></span>

| <span data-ttu-id="c8384-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c8384-108">Method</span></span>       | <span data-ttu-id="c8384-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c8384-109">Return Type</span></span>  |<span data-ttu-id="c8384-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c8384-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8384-111">[получение](../api/attachment-get.md);</span><span class="sxs-lookup"><span data-stu-id="c8384-111">[Get](../api/attachment-get.md)</span></span> | [<span data-ttu-id="c8384-112">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="c8384-112">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="c8384-113">Чтение свойств и связей объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="c8384-113">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="c8384-114">Удаление</span><span class="sxs-lookup"><span data-stu-id="c8384-114">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="c8384-115">Нет</span><span class="sxs-lookup"><span data-stu-id="c8384-115">None</span></span> |<span data-ttu-id="c8384-116">Удаление объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="c8384-116">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c8384-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8384-117">Properties</span></span>
| <span data-ttu-id="c8384-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8384-118">Property</span></span>     | <span data-ttu-id="c8384-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c8384-119">Type</span></span>   |<span data-ttu-id="c8384-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c8384-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8384-121">contentType</span><span class="sxs-lookup"><span data-stu-id="c8384-121">contentType</span></span>|<span data-ttu-id="c8384-122">String</span><span class="sxs-lookup"><span data-stu-id="c8384-122">String</span></span>|<span data-ttu-id="c8384-123">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="c8384-123">The content type of the attachment.</span></span> <span data-ttu-id="c8384-124">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c8384-124">Optional.</span></span>|
|<span data-ttu-id="c8384-125">id</span><span class="sxs-lookup"><span data-stu-id="c8384-125">id</span></span>|<span data-ttu-id="c8384-126">Строка</span><span class="sxs-lookup"><span data-stu-id="c8384-126">String</span></span>|<span data-ttu-id="c8384-p102">Идентификатор вложения.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c8384-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="c8384-129">isFolder</span><span class="sxs-lookup"><span data-stu-id="c8384-129">isFolder</span></span>|<span data-ttu-id="c8384-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8384-130">Boolean</span></span>|<span data-ttu-id="c8384-131">Указывает, является ли вложение ссылкой на папку.</span><span class="sxs-lookup"><span data-stu-id="c8384-131">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="c8384-132">Если **sourceUrl** является ссылкой на папку, необходимо задать для этого параметра значение true.</span><span class="sxs-lookup"><span data-stu-id="c8384-132">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="c8384-133">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c8384-133">Optional.</span></span>|
|<span data-ttu-id="c8384-134">isInline</span><span class="sxs-lookup"><span data-stu-id="c8384-134">isInline</span></span>|<span data-ttu-id="c8384-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8384-135">Boolean</span></span>|<span data-ttu-id="c8384-136">Значение true указывает, что вложение встроено в содержимое объекта.</span><span class="sxs-lookup"><span data-stu-id="c8384-136">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="c8384-137">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c8384-137">Optional.</span></span>|
|<span data-ttu-id="c8384-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8384-138">lastModifiedDateTime</span></span>|<span data-ttu-id="c8384-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8384-139">DateTimeOffset</span></span>|<span data-ttu-id="c8384-140">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="c8384-140">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="c8384-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c8384-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c8384-142">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c8384-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="c8384-143">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c8384-143">Optional.</span></span>|
|<span data-ttu-id="c8384-144">name</span><span class="sxs-lookup"><span data-stu-id="c8384-144">name</span></span>|<span data-ttu-id="c8384-145">String</span><span class="sxs-lookup"><span data-stu-id="c8384-145">String</span></span>|<span data-ttu-id="c8384-146">Текст, который отображается под значком, представляет внедренное вложение.</span><span class="sxs-lookup"><span data-stu-id="c8384-146">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="c8384-147">Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="c8384-147">This does not need to be the actual file name.</span></span> <span data-ttu-id="c8384-148">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c8384-148">Required.</span></span>|
|<span data-ttu-id="c8384-149">права</span><span class="sxs-lookup"><span data-stu-id="c8384-149">permission</span></span>|<span data-ttu-id="c8384-150">referenceAttachmentPermission</span><span class="sxs-lookup"><span data-stu-id="c8384-150">referenceAttachmentPermission</span></span>|<span data-ttu-id="c8384-151">Задает разрешения, предоставленные для вложения, по типу поставщика в **ProviderType**.</span><span class="sxs-lookup"><span data-stu-id="c8384-151">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="c8384-152">Возможные значения: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span><span class="sxs-lookup"><span data-stu-id="c8384-152">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="c8384-153">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c8384-153">Optional.</span></span>|
|<span data-ttu-id="c8384-154">previewUrl</span><span class="sxs-lookup"><span data-stu-id="c8384-154">previewUrl</span></span>|<span data-ttu-id="c8384-155">String</span><span class="sxs-lookup"><span data-stu-id="c8384-155">String</span></span>|<span data-ttu-id="c8384-156">Применяется только к вложению ссылки на URL-адрес изображения для получения изображения предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="c8384-156">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="c8384-157">Используйте **thumbnailUrl** и **previewUrl** только в том случае, если **sourceUrl** определяет файл изображения.</span><span class="sxs-lookup"><span data-stu-id="c8384-157">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="c8384-158">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c8384-158">Optional.</span></span>|
|<span data-ttu-id="c8384-159">providerType</span><span class="sxs-lookup"><span data-stu-id="c8384-159">providerType</span></span>|<span data-ttu-id="c8384-160">Перечислений — referenceattachmentprovider</span><span class="sxs-lookup"><span data-stu-id="c8384-160">referenceAttachmentProvider</span></span>|<span data-ttu-id="c8384-161">Тип поставщика, который поддерживает вложение этого contentType.</span><span class="sxs-lookup"><span data-stu-id="c8384-161">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="c8384-162">Возможные значения: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span><span class="sxs-lookup"><span data-stu-id="c8384-162">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="c8384-163">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c8384-163">Optional.</span></span>|
|<span data-ttu-id="c8384-164">size</span><span class="sxs-lookup"><span data-stu-id="c8384-164">size</span></span>|<span data-ttu-id="c8384-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c8384-165">Int32</span></span>|<span data-ttu-id="c8384-166">Размер метаданных в байтах, хранящихся в сообщении для вложения ссылки.</span><span class="sxs-lookup"><span data-stu-id="c8384-166">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="c8384-167">Это значение не отображает фактический размер файла.</span><span class="sxs-lookup"><span data-stu-id="c8384-167">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="c8384-168">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c8384-168">Optional.</span></span>|
|<span data-ttu-id="c8384-169">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="c8384-169">sourceUrl</span></span>|<span data-ttu-id="c8384-170">String</span><span class="sxs-lookup"><span data-stu-id="c8384-170">String</span></span>|<span data-ttu-id="c8384-171">URL-адрес для получения содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="c8384-171">URL to get the attachment content.</span></span> <span data-ttu-id="c8384-172">Если это URL-адрес папки, то для правильного отображения папки в Outlook или Outlook в **Интернете установите для параметра IsTrue значение true** .</span><span class="sxs-lookup"><span data-stu-id="c8384-172">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="c8384-173">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c8384-173">Required.</span></span>|
|<span data-ttu-id="c8384-174">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="c8384-174">thumbnailUrl</span></span>|<span data-ttu-id="c8384-175">String</span><span class="sxs-lookup"><span data-stu-id="c8384-175">String</span></span>|<span data-ttu-id="c8384-176">Применяется только к вложению ссылки на URL-адрес изображения для получения эскиза.</span><span class="sxs-lookup"><span data-stu-id="c8384-176">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="c8384-177">Используйте **thumbnailUrl** и **previewUrl** только в том случае, если **sourceUrl** определяет файл изображения.</span><span class="sxs-lookup"><span data-stu-id="c8384-177">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="c8384-178">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c8384-178">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8384-179">Отношения</span><span class="sxs-lookup"><span data-stu-id="c8384-179">Relationships</span></span>
<span data-ttu-id="c8384-180">Нет</span><span class="sxs-lookup"><span data-stu-id="c8384-180">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="c8384-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c8384-181">JSON representation</span></span>

<span data-ttu-id="c8384-182">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8384-182">Here is a JSON representation of the resource</span></span>

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
