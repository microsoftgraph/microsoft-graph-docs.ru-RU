---
title: тип ресурса chatMessageAttachment
description: Представляет вложение в объект сообщения чата.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: RamjotSingh
ms.openlocfilehash: b4660e92643d868fbd09c693187a486fc3937584
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582573"
---
# <a name="chatmessageattachment-resource-type"></a><span data-ttu-id="1df08-103">тип ресурса chatMessageAttachment</span><span class="sxs-lookup"><span data-stu-id="1df08-103">chatMessageAttachment resource type</span></span>

<span data-ttu-id="1df08-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1df08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1df08-105">Представляет вложение в объект сообщения чата.</span><span class="sxs-lookup"><span data-stu-id="1df08-105">Represents an attachment to a chat message entity.</span></span>

<span data-ttu-id="1df08-106">Объект типа возвращается в рамках API сообщений get channel, как часть `chatMessageAttachment` [сущности chatMessage.](chatmessage.md) [](../api/channel-list-messages.md)</span><span class="sxs-lookup"><span data-stu-id="1df08-106">An entity of type `chatMessageAttachment` is returned as part of the [Get channel messages](../api/channel-list-messages.md) API, as a part of [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="1df08-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1df08-107">Properties</span></span>
| <span data-ttu-id="1df08-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1df08-108">Property</span></span>     | <span data-ttu-id="1df08-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1df08-109">Type</span></span>   |<span data-ttu-id="1df08-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1df08-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1df08-111">id</span><span class="sxs-lookup"><span data-stu-id="1df08-111">id</span></span>|<span data-ttu-id="1df08-112">string</span><span class="sxs-lookup"><span data-stu-id="1df08-112">string</span></span>| <span data-ttu-id="1df08-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1df08-113">Read-only.</span></span> <span data-ttu-id="1df08-114">Уникальный id вложения.</span><span class="sxs-lookup"><span data-stu-id="1df08-114">Unique id of the attachment.</span></span>|
|<span data-ttu-id="1df08-115">contentType</span><span class="sxs-lookup"><span data-stu-id="1df08-115">contentType</span></span>| <span data-ttu-id="1df08-116">string</span><span class="sxs-lookup"><span data-stu-id="1df08-116">string</span></span> | <span data-ttu-id="1df08-117">Тип мультимедиа вложения контента.</span><span class="sxs-lookup"><span data-stu-id="1df08-117">The media type of the content attachment.</span></span> <span data-ttu-id="1df08-118">Он может иметь следующие значения:</span><span class="sxs-lookup"><span data-stu-id="1df08-118">It can have the following values:</span></span> <br><ul><li><span data-ttu-id="1df08-119">`reference`: Вложение — это ссылка на другой файл.</span><span class="sxs-lookup"><span data-stu-id="1df08-119">`reference`: Attachment is a link to another file.</span></span> <span data-ttu-id="1df08-120">Заполнять contentURL ссылкой на объект.</span><span class="sxs-lookup"><span data-stu-id="1df08-120">Populate the contentURL with the link to the object.</span></span></li><li><span data-ttu-id="1df08-121">Любые contentTypes, поддерживаемые [](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?#attachment-object) объектом вложения Bot Framework</span><span class="sxs-lookup"><span data-stu-id="1df08-121">Any contentTypes supported by the Bot Framework's [Attachment object](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?#attachment-object)</span></span></li><li><span data-ttu-id="1df08-122">`application/vnd.microsoft.card.codesnippet`. Фрагмент кода.</span><span class="sxs-lookup"><span data-stu-id="1df08-122">`application/vnd.microsoft.card.codesnippet`: A code snippet.</span></span> </li><li><span data-ttu-id="1df08-123">`application/vnd.microsoft.card.announcement`: Заглавная ведерка объявления.</span><span class="sxs-lookup"><span data-stu-id="1df08-123">`application/vnd.microsoft.card.announcement`: An announcement header.</span></span> </li>|
|<span data-ttu-id="1df08-124">contentUrl</span><span class="sxs-lookup"><span data-stu-id="1df08-124">contentUrl</span></span>|<span data-ttu-id="1df08-125">string</span><span class="sxs-lookup"><span data-stu-id="1df08-125">string</span></span>|<span data-ttu-id="1df08-126">URL-адрес для содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="1df08-126">URL for the content of the attachment.</span></span> <span data-ttu-id="1df08-127">Поддерживаемые протоколы: http, https, file и data.</span><span class="sxs-lookup"><span data-stu-id="1df08-127">Supported protocols: http, https, file and data.</span></span>|
|<span data-ttu-id="1df08-128">содержимое</span><span class="sxs-lookup"><span data-stu-id="1df08-128">content</span></span>|<span data-ttu-id="1df08-129">string</span><span class="sxs-lookup"><span data-stu-id="1df08-129">string</span></span>|<span data-ttu-id="1df08-130">Содержимое вложения.</span><span class="sxs-lookup"><span data-stu-id="1df08-130">The content of the attachment.</span></span> <span data-ttu-id="1df08-131">Если вложение является [богатой картой,](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference)установите свойство объекту богатой карты.</span><span class="sxs-lookup"><span data-stu-id="1df08-131">If the attachment is a [rich card](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference), set the property to the rich card object.</span></span> <span data-ttu-id="1df08-132">Это свойство и contentUrl являются взаимоисключающими.</span><span class="sxs-lookup"><span data-stu-id="1df08-132">This property and contentUrl are mutually exclusive.</span></span>|
|<span data-ttu-id="1df08-133">name</span><span class="sxs-lookup"><span data-stu-id="1df08-133">name</span></span>|<span data-ttu-id="1df08-134">string</span><span class="sxs-lookup"><span data-stu-id="1df08-134">string</span></span>|<span data-ttu-id="1df08-135">Имя вложения.</span><span class="sxs-lookup"><span data-stu-id="1df08-135">Name of the attachment.</span></span>|
|<span data-ttu-id="1df08-136">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="1df08-136">thumbnailUrl</span></span>| <span data-ttu-id="1df08-137">string</span><span class="sxs-lookup"><span data-stu-id="1df08-137">string</span></span> |<span data-ttu-id="1df08-138">URL-адрес изображения эскиза, который канал может использовать, если поддерживает использование альтернативной, более мелкой формы контента или contentUrl.</span><span class="sxs-lookup"><span data-stu-id="1df08-138">URL to a thumbnail image that the channel can use if it supports using an alternative, smaller form of content or contentUrl.</span></span> <span data-ttu-id="1df08-139">Например, если вы установите contentType для приложения/слова и установите contentUrl к расположению документа Word, вы можете включить эскизное изображение, которое представляет документ.</span><span class="sxs-lookup"><span data-stu-id="1df08-139">For example, if you set contentType to application/word and set contentUrl to the location of the Word document, you might include a thumbnail image that represents the document.</span></span> <span data-ttu-id="1df08-140">Канал может отображать изображение эскиза вместо документа.</span><span class="sxs-lookup"><span data-stu-id="1df08-140">The channel could display the thumbnail image instead of the document.</span></span> <span data-ttu-id="1df08-141">Когда пользователь щелкает изображение, канал откроет документ.</span><span class="sxs-lookup"><span data-stu-id="1df08-141">When the user clicks the image, the channel would open the document.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1df08-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1df08-142">JSON representation</span></span>
 <span data-ttu-id="1df08-143">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1df08-143">The following is a JSON representation of the resource</span></span>

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


