---
title: Тип ресурса fileAttachment
description: 'Файл (например, текстовый файл или документ Word), вложенный в сведения о событии, сообщение или запись. **contentBytes** '
localization_priority: Priority
ms.openlocfilehash: 07dcdac0497caa106eac38d1248661218a7fcc5e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564766"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="184e1-104">Тип ресурса fileAttachment</span><span class="sxs-lookup"><span data-stu-id="184e1-104">fileAttachment resource type</span></span>

<span data-ttu-id="184e1-p102">Файл (например, текстовый файл или документ Word), вложенный в сведения о событии, сообщение или запись. Свойство **contentBytes** включает содержимое файла в кодировке Base 64.</span><span class="sxs-lookup"><span data-stu-id="184e1-p102">A file (such as a text file or Word document) attached to an event, message or post. The  **contentBytes** property contains the base64-encoded contents of the file.</span></span>  

<span data-ttu-id="184e1-107">При создании вложенного файла включите в текст запроса следующее:</span><span class="sxs-lookup"><span data-stu-id="184e1-107">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="184e1-108">Обязательные свойства **name** и **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="184e1-108">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="184e1-109">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="184e1-109">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="184e1-110">Методы</span><span class="sxs-lookup"><span data-stu-id="184e1-110">Methods</span></span>

| <span data-ttu-id="184e1-111">Метод</span><span class="sxs-lookup"><span data-stu-id="184e1-111">Method</span></span>       | <span data-ttu-id="184e1-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="184e1-112">Return Type</span></span>  |<span data-ttu-id="184e1-113">Описание</span><span class="sxs-lookup"><span data-stu-id="184e1-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="184e1-114">Получение</span><span class="sxs-lookup"><span data-stu-id="184e1-114">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="184e1-115">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="184e1-115">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="184e1-116">Чтение свойств и связей объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="184e1-116">Read properties and relationships of fileAttachment object.</span></span>|
|[<span data-ttu-id="184e1-117">Удаление</span><span class="sxs-lookup"><span data-stu-id="184e1-117">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="184e1-118">Нет</span><span class="sxs-lookup"><span data-stu-id="184e1-118">None</span></span> |<span data-ttu-id="184e1-119">Удаление объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="184e1-119">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="184e1-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="184e1-120">Properties</span></span>
| <span data-ttu-id="184e1-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="184e1-121">Property</span></span>     | <span data-ttu-id="184e1-122">Тип</span><span class="sxs-lookup"><span data-stu-id="184e1-122">Type</span></span>   |<span data-ttu-id="184e1-123">Описание</span><span class="sxs-lookup"><span data-stu-id="184e1-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="184e1-124">contentBytes</span><span class="sxs-lookup"><span data-stu-id="184e1-124">contentBytes</span></span>|<span data-ttu-id="184e1-125">Двоичный</span><span class="sxs-lookup"><span data-stu-id="184e1-125">Binary</span></span>|<span data-ttu-id="184e1-126">Содержимое файла в кодировке base64.</span><span class="sxs-lookup"><span data-stu-id="184e1-126">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="184e1-127">contentId</span><span class="sxs-lookup"><span data-stu-id="184e1-127">contentId</span></span>|<span data-ttu-id="184e1-128">String</span><span class="sxs-lookup"><span data-stu-id="184e1-128">String</span></span>|<span data-ttu-id="184e1-129">Идентификатор вложения в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="184e1-129">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="184e1-130">contentLocation</span><span class="sxs-lookup"><span data-stu-id="184e1-130">contentLocation</span></span>|<span data-ttu-id="184e1-131">String</span><span class="sxs-lookup"><span data-stu-id="184e1-131">String</span></span>|<span data-ttu-id="184e1-132">Не используйте это свойство, так как оно не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="184e1-132">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="184e1-133">contentType</span><span class="sxs-lookup"><span data-stu-id="184e1-133">contentType</span></span>|<span data-ttu-id="184e1-134">String</span><span class="sxs-lookup"><span data-stu-id="184e1-134">String</span></span>|<span data-ttu-id="184e1-135">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="184e1-135">The content type of the attachment.</span></span>|
|<span data-ttu-id="184e1-136">id</span><span class="sxs-lookup"><span data-stu-id="184e1-136">id</span></span>|<span data-ttu-id="184e1-137">String</span><span class="sxs-lookup"><span data-stu-id="184e1-137">String</span></span>|<span data-ttu-id="184e1-138">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="184e1-138">The attachment ID.</span></span>|
|<span data-ttu-id="184e1-139">isInline</span><span class="sxs-lookup"><span data-stu-id="184e1-139">isInline</span></span>|<span data-ttu-id="184e1-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="184e1-140">Boolean</span></span>|<span data-ttu-id="184e1-141">Задано значение true, если это встроенное вложение.</span><span class="sxs-lookup"><span data-stu-id="184e1-141">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="184e1-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="184e1-142">lastModifiedDateTime</span></span>|<span data-ttu-id="184e1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="184e1-143">DateTimeOffset</span></span>|<span data-ttu-id="184e1-144">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="184e1-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="184e1-145">name</span><span class="sxs-lookup"><span data-stu-id="184e1-145">name</span></span>|<span data-ttu-id="184e1-146">String</span><span class="sxs-lookup"><span data-stu-id="184e1-146">String</span></span>|<span data-ttu-id="184e1-147">Имя, представляющее текст, который отображается под значком, представляющим внедренное вложение. Оно может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="184e1-147">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="184e1-148">size</span><span class="sxs-lookup"><span data-stu-id="184e1-148">size</span></span>|<span data-ttu-id="184e1-149">Int32</span><span class="sxs-lookup"><span data-stu-id="184e1-149">Int32</span></span>|<span data-ttu-id="184e1-150">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="184e1-150">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="184e1-151">Связи</span><span class="sxs-lookup"><span data-stu-id="184e1-151">Relationships</span></span>
<span data-ttu-id="184e1-152">Нет</span><span class="sxs-lookup"><span data-stu-id="184e1-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="184e1-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="184e1-153">JSON representation</span></span>

<span data-ttu-id="184e1-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="184e1-154">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
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
<!-- {
  "type": "#page.annotation",
  "description": "fileAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
