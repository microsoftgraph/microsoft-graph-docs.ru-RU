---
title: Тип ресурса referenceAttachment
description: 'Ссылка на папку или файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или других поддерживаемых местах хранения, подключенных к '
localization_priority: Normal
ms.openlocfilehash: 59ebb0af10a64195643cb7073d1206790ae6a875
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563105"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="9b65a-103">Тип ресурса referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="9b65a-103">referenceAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b65a-104">Ссылка на папку или файл (например, текстовый файл или документ Word) на облачном диске OneDrive для бизнеса или других поддерживаемых местах хранения, прикрепленных к [событию](../resources/event.md), сообщению, [](../resources/message.md)задаче [Outlook](../resources/outlooktask.md)или [POST](../resources/post.md) .</span><span class="sxs-lookup"><span data-stu-id="9b65a-104">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="9b65a-105">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="9b65a-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9b65a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9b65a-106">Methods</span></span>

| <span data-ttu-id="9b65a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9b65a-107">Method</span></span>       | <span data-ttu-id="9b65a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9b65a-108">Return Type</span></span>  |<span data-ttu-id="9b65a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9b65a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9b65a-110">Get</span><span class="sxs-lookup"><span data-stu-id="9b65a-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="9b65a-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="9b65a-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="9b65a-112">Чтение свойств и связей объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="9b65a-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="9b65a-113">Удаление</span><span class="sxs-lookup"><span data-stu-id="9b65a-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="9b65a-114">Нет</span><span class="sxs-lookup"><span data-stu-id="9b65a-114">None</span></span> |<span data-ttu-id="9b65a-115">Удаление объекта referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="9b65a-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9b65a-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b65a-116">Properties</span></span>
| <span data-ttu-id="9b65a-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b65a-117">Property</span></span>     | <span data-ttu-id="9b65a-118">Тип</span><span class="sxs-lookup"><span data-stu-id="9b65a-118">Type</span></span>   |<span data-ttu-id="9b65a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9b65a-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b65a-120">contentType</span><span class="sxs-lookup"><span data-stu-id="9b65a-120">contentType</span></span>|<span data-ttu-id="9b65a-121">String</span><span class="sxs-lookup"><span data-stu-id="9b65a-121">String</span></span>|<span data-ttu-id="9b65a-122">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="9b65a-122">The content type of the attachment.</span></span> <span data-ttu-id="9b65a-123">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9b65a-123">Optional.</span></span>|
|<span data-ttu-id="9b65a-124">id</span><span class="sxs-lookup"><span data-stu-id="9b65a-124">id</span></span>|<span data-ttu-id="9b65a-125">Строка</span><span class="sxs-lookup"><span data-stu-id="9b65a-125">String</span></span>|<span data-ttu-id="9b65a-p102">Идентификатор вложения.  Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9b65a-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="9b65a-128">isFolder</span><span class="sxs-lookup"><span data-stu-id="9b65a-128">isFolder</span></span>|<span data-ttu-id="9b65a-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b65a-129">Boolean</span></span>|<span data-ttu-id="9b65a-130">Указывает, является ли вложение ссылкой на папку.</span><span class="sxs-lookup"><span data-stu-id="9b65a-130">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="9b65a-131">Если **sourceUrl** является ссылкой на папку, необходимо задать для этого параметра значение true.</span><span class="sxs-lookup"><span data-stu-id="9b65a-131">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="9b65a-132">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9b65a-132">Optional.</span></span>|
|<span data-ttu-id="9b65a-133">isInline</span><span class="sxs-lookup"><span data-stu-id="9b65a-133">isInline</span></span>|<span data-ttu-id="9b65a-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b65a-134">Boolean</span></span>|<span data-ttu-id="9b65a-135">Значение true указывает, что вложение встроено в содержимое объекта.</span><span class="sxs-lookup"><span data-stu-id="9b65a-135">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="9b65a-136">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9b65a-136">Optional.</span></span>|
|<span data-ttu-id="9b65a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b65a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9b65a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b65a-138">DateTimeOffset</span></span>|<span data-ttu-id="9b65a-139">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="9b65a-139">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="9b65a-140">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9b65a-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9b65a-141">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9b65a-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9b65a-142">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9b65a-142">Optional.</span></span>|
|<span data-ttu-id="9b65a-143">name</span><span class="sxs-lookup"><span data-stu-id="9b65a-143">name</span></span>|<span data-ttu-id="9b65a-144">String</span><span class="sxs-lookup"><span data-stu-id="9b65a-144">String</span></span>|<span data-ttu-id="9b65a-145">Текст, который отображается под значком, представляет внедренное вложение.</span><span class="sxs-lookup"><span data-stu-id="9b65a-145">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="9b65a-146">Он может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="9b65a-146">This does not need to be the actual file name.</span></span> <span data-ttu-id="9b65a-147">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b65a-147">Required.</span></span>|
|<span data-ttu-id="9b65a-148">права</span><span class="sxs-lookup"><span data-stu-id="9b65a-148">permission</span></span>|<span data-ttu-id="9b65a-149">Референцеаттачментпермиссионс</span><span class="sxs-lookup"><span data-stu-id="9b65a-149">ReferenceAttachmentPermissions</span></span>|<span data-ttu-id="9b65a-150">Задает разрешения, предоставленные для вложения, по типу поставщика в **ProviderType**.</span><span class="sxs-lookup"><span data-stu-id="9b65a-150">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="9b65a-151">Возможные значения: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span><span class="sxs-lookup"><span data-stu-id="9b65a-151">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="9b65a-152">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9b65a-152">Optional.</span></span>|
|<span data-ttu-id="9b65a-153">previewUrl</span><span class="sxs-lookup"><span data-stu-id="9b65a-153">previewUrl</span></span>|<span data-ttu-id="9b65a-154">String</span><span class="sxs-lookup"><span data-stu-id="9b65a-154">String</span></span>|<span data-ttu-id="9b65a-155">Применяется только к вложению ссылки на URL-адрес изображения для получения изображения предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="9b65a-155">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="9b65a-156">Используйте **thumbnailUrl** и **previewUrl** только в том случае, если **sourceUrl** определяет файл изображения.</span><span class="sxs-lookup"><span data-stu-id="9b65a-156">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="9b65a-157">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9b65a-157">Optional.</span></span>|
|<span data-ttu-id="9b65a-158">providerType</span><span class="sxs-lookup"><span data-stu-id="9b65a-158">providerType</span></span>|<span data-ttu-id="9b65a-159">Референцеаттачментпровидерс</span><span class="sxs-lookup"><span data-stu-id="9b65a-159">ReferenceAttachmentProviders</span></span>|<span data-ttu-id="9b65a-160">Тип поставщика, который поддерживает вложение этого contentType.</span><span class="sxs-lookup"><span data-stu-id="9b65a-160">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="9b65a-161">Возможные значения: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span><span class="sxs-lookup"><span data-stu-id="9b65a-161">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="9b65a-162">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9b65a-162">Optional.</span></span>|
|<span data-ttu-id="9b65a-163">size</span><span class="sxs-lookup"><span data-stu-id="9b65a-163">size</span></span>|<span data-ttu-id="9b65a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9b65a-164">Int32</span></span>|<span data-ttu-id="9b65a-165">Размер метаданных в байтах, хранящихся в сообщении для вложения ссылки.</span><span class="sxs-lookup"><span data-stu-id="9b65a-165">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="9b65a-166">Это значение не отображает фактический размер файла.</span><span class="sxs-lookup"><span data-stu-id="9b65a-166">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="9b65a-167">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9b65a-167">Optional.</span></span>|
|<span data-ttu-id="9b65a-168">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="9b65a-168">sourceUrl</span></span>|<span data-ttu-id="9b65a-169">String</span><span class="sxs-lookup"><span data-stu-id="9b65a-169">String</span></span>|<span data-ttu-id="9b65a-170">URL-адрес для получения содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="9b65a-170">URL to get the attachment content.</span></span> <span data-ttu-id="9b65a-171">Если это URL-адрес папки, то для правильного отображения папки в Outlook или Outlook в Интернете установите для параметра IsTrue значение true. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="9b65a-171">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="9b65a-172">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b65a-172">Required.</span></span>|
|<span data-ttu-id="9b65a-173">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="9b65a-173">thumbnailUrl</span></span>|<span data-ttu-id="9b65a-174">String</span><span class="sxs-lookup"><span data-stu-id="9b65a-174">String</span></span>|<span data-ttu-id="9b65a-175">Применяется только к вложению ссылки на URL-адрес изображения для получения эскиза.</span><span class="sxs-lookup"><span data-stu-id="9b65a-175">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="9b65a-176">Используйте **thumbnailUrl** и **previewUrl** только в том случае, если **sourceUrl** определяет файл изображения.</span><span class="sxs-lookup"><span data-stu-id="9b65a-176">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="9b65a-177">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9b65a-177">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b65a-178">Отношения</span><span class="sxs-lookup"><span data-stu-id="9b65a-178">Relationships</span></span>
<span data-ttu-id="9b65a-179">Нет</span><span class="sxs-lookup"><span data-stu-id="9b65a-179">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="9b65a-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b65a-180">JSON representation</span></span>

<span data-ttu-id="9b65a-181">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b65a-181">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/referenceattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
