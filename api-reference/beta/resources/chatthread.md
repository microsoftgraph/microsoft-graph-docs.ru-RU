---
title: Тип ресурса chatThread
description: chatThread — это коллекция ресурсов chatMessages в Microsoft Teams.
localization_priority: Priority
ms.openlocfilehash: a85b6aea6c48c9295fe88a7412fa7e6b96ee1d3f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521343"
---
# <a name="chatthread-resource-type"></a><span data-ttu-id="e65f4-103">Тип ресурса chatThread</span><span class="sxs-lookup"><span data-stu-id="e65f4-103">chatThread resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e65f4-104">chatThread — это коллекция ресурсов [chatMessages](chatmessage.md) в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e65f4-104">A chatThread is a collection of [chatMessages](chatmessage.md) in Microsoft Teams.</span></span>

> <span data-ttu-id="e65f4-105">В настоящее время chatThreads можно [создавать в каналах](../api/channel-post-chatthreads.md).</span><span class="sxs-lookup"><span data-stu-id="e65f4-105">Currently, chatThreads can be [created in channels](../api/channel-post-chatthreads.md).</span></span>  <span data-ttu-id="e65f4-106">Будущие выпуски API будут поддерживать чтение существующих chatThreads, а также чтение и запись прямых чатов между пользователями за пределами группы или канала.</span><span class="sxs-lookup"><span data-stu-id="e65f4-106">Future API releases will support reading existing chatThreads, as well as reading/writing direct chats between users that are outside the scope of a team or channel.</span></span>

## <a name="methods"></a><span data-ttu-id="e65f4-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e65f4-107">Methods</span></span>

| <span data-ttu-id="e65f4-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e65f4-108">Method</span></span>       | <span data-ttu-id="e65f4-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e65f4-109">Return Type</span></span>  |<span data-ttu-id="e65f4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e65f4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e65f4-111">Создание цепочки</span><span class="sxs-lookup"><span data-stu-id="e65f4-111">Create thread</span></span>](../api/channel-post-chatthreads.md) | [<span data-ttu-id="e65f4-112">chatThread</span><span class="sxs-lookup"><span data-stu-id="e65f4-112">chatThread</span></span>](chatthread.md) |<span data-ttu-id="e65f4-113">Начало новой цепочки беседы в указанном канале путем предоставления первого сообщения.</span><span class="sxs-lookup"><span data-stu-id="e65f4-113">Start a new thread in the specified channel, providing the first message.</span></span>|

## <a name="properties"></a><span data-ttu-id="e65f4-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="e65f4-114">Properties</span></span>
| <span data-ttu-id="e65f4-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="e65f4-115">Property</span></span>     | <span data-ttu-id="e65f4-116">Тип</span><span class="sxs-lookup"><span data-stu-id="e65f4-116">Type</span></span>   |<span data-ttu-id="e65f4-117">Описание</span><span class="sxs-lookup"><span data-stu-id="e65f4-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e65f4-118">id</span><span class="sxs-lookup"><span data-stu-id="e65f4-118">id</span></span>|<span data-ttu-id="e65f4-119">String</span><span class="sxs-lookup"><span data-stu-id="e65f4-119">String</span></span>| <span data-ttu-id="e65f4-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e65f4-120">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e65f4-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="e65f4-121">Relationships</span></span>
| <span data-ttu-id="e65f4-122">Связь</span><span class="sxs-lookup"><span data-stu-id="e65f4-122">Relationship</span></span> | <span data-ttu-id="e65f4-123">Тип</span><span class="sxs-lookup"><span data-stu-id="e65f4-123">Type</span></span>   |<span data-ttu-id="e65f4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e65f4-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e65f4-125">rootMessage</span><span class="sxs-lookup"><span data-stu-id="e65f4-125">rootMessage</span></span>|[<span data-ttu-id="e65f4-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="e65f4-126">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="e65f4-127">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e65f4-127">Nullable.</span></span>|
|<span data-ttu-id="e65f4-128">chatMessages</span><span class="sxs-lookup"><span data-stu-id="e65f4-128">chatMessages</span></span>|<span data-ttu-id="e65f4-129">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="e65f4-129">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="e65f4-130">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e65f4-130">Nullable.</span></span>|

> <span data-ttu-id="e65f4-131">В настоящее время эти отношения неявно существуют, но их нельзя прочитать или записать.</span><span class="sxs-lookup"><span data-stu-id="e65f4-131">Currently these relationships exist implicitly, but cannot read or written.</span></span>  <span data-ttu-id="e65f4-132">Эта возможность появится в будущих бета-выпусках API.</span><span class="sxs-lookup"><span data-stu-id="e65f4-132">Future beta API releases will support this.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e65f4-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e65f4-133">JSON representation</span></span>

<span data-ttu-id="e65f4-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e65f4-134">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatThread"
}-->

```json
{
  "id": "string (identifier)"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatthread.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
