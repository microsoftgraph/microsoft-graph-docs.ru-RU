---
title: Тип ресурса Чатмессажехостедимаже
description: Представляет размещенное изображение в chatMessage.
localization_priority: Normal
author: clearab
ms.openlocfilehash: 1f7ce24dfae680937ecb1c43f9a34f6b9bb35646
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/20/2019
ms.locfileid: "35085846"
---
# <a name="chatmessagehostedimage-resource-type"></a><span data-ttu-id="96f5f-103">Тип ресурса Чатмессажехостедимаже</span><span class="sxs-lookup"><span data-stu-id="96f5f-103">chatMessageHostedImage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96f5f-104">Представляет размещенное изображение в [chatMessage](../resources/chatmessage.md).</span><span class="sxs-lookup"><span data-stu-id="96f5f-104">Represents a hosted image inside a [chatMessage](../resources/chatmessage.md).</span></span>

<span data-ttu-id="96f5f-105">Размещенные изображения — это изображения, которые отображаются в **теле сообщения. содержимое** тега> \<IMG с атрибутом src, начинающимся с `https://graph.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="96f5f-105">Hosted images are the images that appear in the message's **body.content** in an \<img> tag with a src attribute that starts with `https://graph.microsoft.com`.</span></span>

<span data-ttu-id="96f5f-106">Не все изображения в сообщении являются размещенными изображениями, Microsoft Teams также поддерживает общедоступные изображения (в которых атрибут img src указывает на общедоступный веб-сайт).</span><span class="sxs-lookup"><span data-stu-id="96f5f-106">Not all images in a message are hosted images, Microsoft Teams also supports public images (where the img src attribute points to a public website).</span></span>

## <a name="methods"></a><span data-ttu-id="96f5f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="96f5f-107">Methods</span></span>

| <span data-ttu-id="96f5f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="96f5f-108">Method</span></span>       | <span data-ttu-id="96f5f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="96f5f-109">Return Type</span></span>  |<span data-ttu-id="96f5f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="96f5f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="96f5f-111">Перечисление Чатмессажехостедимажес в chatMessage</span><span class="sxs-lookup"><span data-stu-id="96f5f-111">List chatMessageHostedImages in a chatMessage</span></span>](../api/chatmessagehostedimage-list-hostedimages.md) | <span data-ttu-id="96f5f-112">Коллекция [чатмессажехостедимаже](chatmessagehostedimage.md)</span><span class="sxs-lookup"><span data-stu-id="96f5f-112">[chatMessageHostedImage](chatmessagehostedimage.md) collection</span></span> | <span data-ttu-id="96f5f-113">Список всех размещенных изображений в **chatMessage**.</span><span class="sxs-lookup"><span data-stu-id="96f5f-113">List of all hosted images in a **chatMessage**.</span></span>|
|[<span data-ttu-id="96f5f-114">Получение Чатмессажехостедимаже</span><span class="sxs-lookup"><span data-stu-id="96f5f-114">Get chatMessageHostedImage</span></span>](../api/chatmessagehostedimage-get.md) | [<span data-ttu-id="96f5f-115">Чатмессажехостедимаже</span><span class="sxs-lookup"><span data-stu-id="96f5f-115">chatMessageHostedImage</span></span>](chatmessagehostedimage.md) | <span data-ttu-id="96f5f-116">Получение отдельного размещенного изображения.</span><span class="sxs-lookup"><span data-stu-id="96f5f-116">Get a single hosted image.</span></span>|
|[<span data-ttu-id="96f5f-117">Чатмессажехостедимаже: GetBytes</span><span class="sxs-lookup"><span data-stu-id="96f5f-117">chatMessageHostedImage: getBytes</span></span>](../api/chatmessagehostedimage-getbytes.md) | <span data-ttu-id="96f5f-118">Content-Type: Image/JPEG</span><span class="sxs-lookup"><span data-stu-id="96f5f-118">Content-type: image/jpeg</span></span> | <span data-ttu-id="96f5f-119">Получение необработанных байтов размещаемого изображения.</span><span class="sxs-lookup"><span data-stu-id="96f5f-119">Get the raw bytes of the hosted image.</span></span>|

## <a name="properties"></a><span data-ttu-id="96f5f-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="96f5f-120">Properties</span></span>

| <span data-ttu-id="96f5f-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="96f5f-121">Property</span></span>     | <span data-ttu-id="96f5f-122">Тип</span><span class="sxs-lookup"><span data-stu-id="96f5f-122">Type</span></span>   |<span data-ttu-id="96f5f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="96f5f-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96f5f-124">id</span><span class="sxs-lookup"><span data-stu-id="96f5f-124">id</span></span>|<span data-ttu-id="96f5f-125">String</span><span class="sxs-lookup"><span data-stu-id="96f5f-125">String</span></span>| <span data-ttu-id="96f5f-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="96f5f-126">Read-only.</span></span> <span data-ttu-id="96f5f-127">Уникальный идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="96f5f-127">Unique ID of the message.</span></span>|
|<span data-ttu-id="96f5f-128">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="96f5f-128">URL</span></span>| <span data-ttu-id="96f5f-129">string</span><span class="sxs-lookup"><span data-stu-id="96f5f-129">string</span></span> | <span data-ttu-id="96f5f-130">URL-адрес, из которого извлекается содержимое изображения.</span><span class="sxs-lookup"><span data-stu-id="96f5f-130">The url to retrieve the image contents from.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="96f5f-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="96f5f-131">JSON representation</span></span>

<span data-ttu-id="96f5f-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96f5f-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageHostedImage"
}-->

```json
{
  "id": "string (identifier)",
  "url": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
