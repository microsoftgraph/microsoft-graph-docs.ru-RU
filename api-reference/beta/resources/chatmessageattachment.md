---
title: Тип ресурса Чатмессажеаттачмент
description: Представляет вложение для объекта сообщения чата.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 1b9ddbb0b8dac124370b1d20ac42e3ab1da7d1e3
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791085"
---
# <a name="chatmessageattachment-resource-type"></a><span data-ttu-id="489fc-103">Тип ресурса Чатмессажеаттачмент</span><span class="sxs-lookup"><span data-stu-id="489fc-103">chatMessageAttachment resource type</span></span>

<span data-ttu-id="489fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="489fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="489fc-105">Представляет вложение для объекта сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="489fc-105">Represents an attachment to a chat message entity.</span></span>

<span data-ttu-id="489fc-106">Сущность типа `chatMessageAttachment` возвращается в составе API [сообщений канала](../api/channel-list-messages.md) в составе объекта [chatMessage](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="489fc-106">An entity of type `chatMessageAttachment` is returned as part of the [Get channel messages](../api/channel-list-messages.md) API, as a part of [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="489fc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="489fc-107">Properties</span></span>
| <span data-ttu-id="489fc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="489fc-108">Property</span></span>     | <span data-ttu-id="489fc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="489fc-109">Type</span></span>   |<span data-ttu-id="489fc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="489fc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="489fc-111">id</span><span class="sxs-lookup"><span data-stu-id="489fc-111">id</span></span>|<span data-ttu-id="489fc-112">string</span><span class="sxs-lookup"><span data-stu-id="489fc-112">string</span></span>| <span data-ttu-id="489fc-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="489fc-113">Read-only.</span></span> <span data-ttu-id="489fc-114">Уникальный идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="489fc-114">Unique id of the attachment.</span></span>|
|<span data-ttu-id="489fc-115">contentType</span><span class="sxs-lookup"><span data-stu-id="489fc-115">contentType</span></span>| <span data-ttu-id="489fc-116">string</span><span class="sxs-lookup"><span data-stu-id="489fc-116">string</span></span> | <span data-ttu-id="489fc-117">Тип мультимедиа вложенного содержимого.</span><span class="sxs-lookup"><span data-stu-id="489fc-117">The media type of the content attachment.</span></span> <span data-ttu-id="489fc-118">Он может иметь следующие значения:</span><span class="sxs-lookup"><span data-stu-id="489fc-118">It can have the following values:</span></span> <br><ul><li><span data-ttu-id="489fc-119">`reference`: Вложение — это ссылка на другой файл.</span><span class="sxs-lookup"><span data-stu-id="489fc-119">`reference`: Attachment is a link to another file.</span></span> <span data-ttu-id="489fc-120">Заполните contentURL ссылкой на объект.</span><span class="sxs-lookup"><span data-stu-id="489fc-120">Populate the contentURL with the link to the object.</span></span></li><li><span data-ttu-id="489fc-121">Все типы контента, поддерживаемые [объектом приложения](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?view=azure-bot-service-4.0#attachment-object) Bot Framework</span><span class="sxs-lookup"><span data-stu-id="489fc-121">Any contentTypes supported by the Bot Framework's [Attachment object](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?view=azure-bot-service-4.0#attachment-object)</span></span></li><li><span data-ttu-id="489fc-122">`application/vnd.microsoft.card.codesnippet`: Фрагмент кода.</span><span class="sxs-lookup"><span data-stu-id="489fc-122">`application/vnd.microsoft.card.codesnippet`: A code snippet.</span></span> </li><li><span data-ttu-id="489fc-123">`application/vnd.microsoft.card.announcement`: Заголовок извещения.</span><span class="sxs-lookup"><span data-stu-id="489fc-123">`application/vnd.microsoft.card.announcement`: An announcement header.</span></span> </li>|
|<span data-ttu-id="489fc-124">contentUrl</span><span class="sxs-lookup"><span data-stu-id="489fc-124">contentUrl</span></span>|<span data-ttu-id="489fc-125">string</span><span class="sxs-lookup"><span data-stu-id="489fc-125">string</span></span>|<span data-ttu-id="489fc-126">URL-адрес содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="489fc-126">URL for the content of the attachment.</span></span> <span data-ttu-id="489fc-127">Поддерживаемые протоколы: HTTP, HTTPS, File и Data.</span><span class="sxs-lookup"><span data-stu-id="489fc-127">Supported protocols: http, https, file and data.</span></span>|
|<span data-ttu-id="489fc-128">содержимое</span><span class="sxs-lookup"><span data-stu-id="489fc-128">content</span></span>|<span data-ttu-id="489fc-129">string</span><span class="sxs-lookup"><span data-stu-id="489fc-129">string</span></span>|<span data-ttu-id="489fc-130">Содержимое вложения.</span><span class="sxs-lookup"><span data-stu-id="489fc-130">The content of the attachment.</span></span> <span data-ttu-id="489fc-131">Если вложение является [расширенной карточкой](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference), задайте свойству объект с богатыми карточками.</span><span class="sxs-lookup"><span data-stu-id="489fc-131">If the attachment is a [rich card](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference), set the property to the rich card object.</span></span> <span data-ttu-id="489fc-132">Это свойство и contentUrl являются взаимоисключающими.</span><span class="sxs-lookup"><span data-stu-id="489fc-132">This property and contentUrl are mutually exclusive.</span></span>|
|<span data-ttu-id="489fc-133">name</span><span class="sxs-lookup"><span data-stu-id="489fc-133">name</span></span>|<span data-ttu-id="489fc-134">string</span><span class="sxs-lookup"><span data-stu-id="489fc-134">string</span></span>|<span data-ttu-id="489fc-135">Имя вложения.</span><span class="sxs-lookup"><span data-stu-id="489fc-135">Name of the attachment.</span></span>|
|<span data-ttu-id="489fc-136">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="489fc-136">thumbnailUrl</span></span>| <span data-ttu-id="489fc-137">string</span><span class="sxs-lookup"><span data-stu-id="489fc-137">string</span></span> |<span data-ttu-id="489fc-138">URL-адрес эскиза, который может использоваться каналом, если он поддерживается в альтернативной, меньшей форме содержимого или contentUrl.</span><span class="sxs-lookup"><span data-stu-id="489fc-138">URL to a thumbnail image that the channel can use if it supports using an alternative, smaller form of content or contentUrl.</span></span> <span data-ttu-id="489fc-139">Например, если для объекта contentType задано значение Application/Word, а для параметра contentUrl задано расположение документа Word, можно включить эскиз изображения, представляющий документ.</span><span class="sxs-lookup"><span data-stu-id="489fc-139">For example, if you set contentType to application/word and set contentUrl to the location of the Word document, you might include a thumbnail image that represents the document.</span></span> <span data-ttu-id="489fc-140">Вместо документа в канале может отображаться миниатюрное изображение.</span><span class="sxs-lookup"><span data-stu-id="489fc-140">The channel could display the thumbnail image instead of the document.</span></span> <span data-ttu-id="489fc-141">Когда пользователь щелкает изображение, канал открывает документ.</span><span class="sxs-lookup"><span data-stu-id="489fc-141">When the user clicks the image, the channel would open the document.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="489fc-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="489fc-142">JSON representation</span></span>
 <span data-ttu-id="489fc-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="489fc-143">The following is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "thumbnailUrl",
    "content",
    "contentUrl"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessageAttachment"
}-->

```json
{
  "id": "string (identifier)",
  "contentType": "string",
  "contentUrl": "string",
  "content": "string",
  "name": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
