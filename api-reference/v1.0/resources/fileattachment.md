---
title: Тип ресурса fileAttachment
description: 'Файл (например, текстовый файл или документ Word), вложенный в сведения о событии, сообщение или запись. **contentBytes** '
localization_priority: Priority
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 584685bd7857c7091b30fe13b6ce9c855d539ce2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018363"
---
# <a name="fileattachment-resource-type"></a><span data-ttu-id="9cab5-104">Тип ресурса fileAttachment</span><span class="sxs-lookup"><span data-stu-id="9cab5-104">fileAttachment resource type</span></span>

<span data-ttu-id="9cab5-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cab5-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9cab5-106">Файл (например, текстовый файл или документ Word), вложенный в [событие](../resources/event.md) пользователя, [сообщение](../resources/message.md) или [запись](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="9cab5-106">A file (such as a text file or Word document) attached to a user [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md).</span></span> 

<span data-ttu-id="9cab5-107">При создании вложенного файла включите в текст запроса следующее:</span><span class="sxs-lookup"><span data-stu-id="9cab5-107">When creating a file attachment, include the following in the request body:</span></span>

* `"@odata.type": "#microsoft.graph.fileAttachment"`
* <span data-ttu-id="9cab5-108">Обязательные свойства **name** и **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="9cab5-108">The required properties **name** and **contentBytes**.</span></span>

<span data-ttu-id="9cab5-109">Производный от типа [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="9cab5-109">Derived from [attachment](attachment.md).</span></span>

> [!NOTE]
> <span data-ttu-id="9cab5-110">Не забудьте закодировать содержимое файла в base64 перед назначением его **contentBytes**.</span><span class="sxs-lookup"><span data-stu-id="9cab5-110">Make sure to encode the file content in base64 before assigning it to **contentBytes**.</span></span>

## <a name="methods"></a><span data-ttu-id="9cab5-111">Методы</span><span class="sxs-lookup"><span data-stu-id="9cab5-111">Methods</span></span>

| <span data-ttu-id="9cab5-112">Метод</span><span class="sxs-lookup"><span data-stu-id="9cab5-112">Method</span></span>       | <span data-ttu-id="9cab5-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9cab5-113">Return Type</span></span>  |<span data-ttu-id="9cab5-114">Описание</span><span class="sxs-lookup"><span data-stu-id="9cab5-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9cab5-115">Получение</span><span class="sxs-lookup"><span data-stu-id="9cab5-115">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="9cab5-116">fileAttachment</span><span class="sxs-lookup"><span data-stu-id="9cab5-116">fileAttachment</span></span>](fileattachment.md) |<span data-ttu-id="9cab5-117">Чтение свойств, связей или необработанного содержимого объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="9cab5-117">Read properties, relationships, or raw contents of a fileAttachment object.</span></span>|
|[<span data-ttu-id="9cab5-118">Удаление</span><span class="sxs-lookup"><span data-stu-id="9cab5-118">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="9cab5-119">Нет</span><span class="sxs-lookup"><span data-stu-id="9cab5-119">None</span></span> |<span data-ttu-id="9cab5-120">Удаление объекта fileAttachment.</span><span class="sxs-lookup"><span data-stu-id="9cab5-120">Delete fileAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9cab5-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="9cab5-121">Properties</span></span>
| <span data-ttu-id="9cab5-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="9cab5-122">Property</span></span>     | <span data-ttu-id="9cab5-123">Тип</span><span class="sxs-lookup"><span data-stu-id="9cab5-123">Type</span></span>   |<span data-ttu-id="9cab5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9cab5-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9cab5-125">contentBytes</span><span class="sxs-lookup"><span data-stu-id="9cab5-125">contentBytes</span></span>|<span data-ttu-id="9cab5-126">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="9cab5-126">Edm.Binary</span></span>|<span data-ttu-id="9cab5-127">Содержимое файла в кодировке base64.</span><span class="sxs-lookup"><span data-stu-id="9cab5-127">The base64-encoded contents of the file.</span></span>|
|<span data-ttu-id="9cab5-128">contentId</span><span class="sxs-lookup"><span data-stu-id="9cab5-128">contentId</span></span>|<span data-ttu-id="9cab5-129">String</span><span class="sxs-lookup"><span data-stu-id="9cab5-129">String</span></span>|<span data-ttu-id="9cab5-130">Идентификатор вложения в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="9cab5-130">The ID of the attachment in the Exchange store.</span></span>|
|<span data-ttu-id="9cab5-131">contentLocation</span><span class="sxs-lookup"><span data-stu-id="9cab5-131">contentLocation</span></span>|<span data-ttu-id="9cab5-132">String</span><span class="sxs-lookup"><span data-stu-id="9cab5-132">String</span></span>|<span data-ttu-id="9cab5-133">Не используйте это свойство, так как оно не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cab5-133">Do not use this property as it is not supported.</span></span>|
|<span data-ttu-id="9cab5-134">contentType</span><span class="sxs-lookup"><span data-stu-id="9cab5-134">contentType</span></span>|<span data-ttu-id="9cab5-135">String</span><span class="sxs-lookup"><span data-stu-id="9cab5-135">String</span></span>|<span data-ttu-id="9cab5-136">Тип контента этого вложения.</span><span class="sxs-lookup"><span data-stu-id="9cab5-136">The content type of the attachment.</span></span>|
|<span data-ttu-id="9cab5-137">id</span><span class="sxs-lookup"><span data-stu-id="9cab5-137">id</span></span>|<span data-ttu-id="9cab5-138">String</span><span class="sxs-lookup"><span data-stu-id="9cab5-138">String</span></span>|<span data-ttu-id="9cab5-139">Идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="9cab5-139">The attachment ID.</span></span>|
|<span data-ttu-id="9cab5-140">isInline</span><span class="sxs-lookup"><span data-stu-id="9cab5-140">isInline</span></span>|<span data-ttu-id="9cab5-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cab5-141">Boolean</span></span>|<span data-ttu-id="9cab5-142">Задано значение true, если это встроенное вложение.</span><span class="sxs-lookup"><span data-stu-id="9cab5-142">Set to true if this is an inline attachment.</span></span>|
|<span data-ttu-id="9cab5-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9cab5-143">lastModifiedDateTime</span></span>|<span data-ttu-id="9cab5-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cab5-144">DateTimeOffset</span></span>|<span data-ttu-id="9cab5-145">Дата и время последнего изменения вложения.</span><span class="sxs-lookup"><span data-stu-id="9cab5-145">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="9cab5-146">name</span><span class="sxs-lookup"><span data-stu-id="9cab5-146">name</span></span>|<span data-ttu-id="9cab5-147">String</span><span class="sxs-lookup"><span data-stu-id="9cab5-147">String</span></span>|<span data-ttu-id="9cab5-148">Имя, представляющее текст, который отображается под значком, представляющим внедренное вложение. Оно может не быть фактическим именем файла.</span><span class="sxs-lookup"><span data-stu-id="9cab5-148">The name representing the text that is displayed below the icon representing the embedded attachment.This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="9cab5-149">size</span><span class="sxs-lookup"><span data-stu-id="9cab5-149">size</span></span>|<span data-ttu-id="9cab5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="9cab5-150">Int32</span></span>|<span data-ttu-id="9cab5-151">Размер вложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="9cab5-151">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cab5-152">Связи</span><span class="sxs-lookup"><span data-stu-id="9cab5-152">Relationships</span></span>
<span data-ttu-id="9cab5-153">Нет</span><span class="sxs-lookup"><span data-stu-id="9cab5-153">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9cab5-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9cab5-154">JSON representation</span></span>

<span data-ttu-id="9cab5-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9cab5-155">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAttachment"
}-->

```json
{
  "contentBytes": "string (binary)",
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

