---
title: Тип ресурса chatThread
description: chatThread — это коллекция ресурсов chatMessages в Microsoft Teams.
localization_priority: Priority
ms.openlocfilehash: 19365109c2008d52d3597b3d23fc1baefa5cfd1c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399607"
---
# <a name="chatthread-resource-type"></a><span data-ttu-id="4dca2-103">Тип ресурса chatThread</span><span class="sxs-lookup"><span data-stu-id="4dca2-103">chatThread resource type</span></span>

> <span data-ttu-id="4dca2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4dca2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4dca2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4dca2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4dca2-106">chatThread — это коллекция ресурсов [chatMessages](chatmessage.md) в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4dca2-106">A chatThread is a collection of [chatMessages](chatmessage.md) in Microsoft Teams.</span></span>

> <span data-ttu-id="4dca2-107">В настоящее время chatThreads можно [создавать в каналах](../api/channel-post-chatthreads.md).</span><span class="sxs-lookup"><span data-stu-id="4dca2-107">Currently, chatThreads can be [created in channels](../api/channel-post-chatthreads.md).</span></span>  <span data-ttu-id="4dca2-108">Будущие выпуски API будут поддерживать чтение существующих chatThreads, а также чтение и запись прямых чатов между пользователями за пределами группы или канала.</span><span class="sxs-lookup"><span data-stu-id="4dca2-108">Future API releases will support reading existing chatThreads, as well as reading/writing direct chats between users that are outside the scope of a team or channel.</span></span>

## <a name="methods"></a><span data-ttu-id="4dca2-109">Методы</span><span class="sxs-lookup"><span data-stu-id="4dca2-109">Methods</span></span>

| <span data-ttu-id="4dca2-110">Метод</span><span class="sxs-lookup"><span data-stu-id="4dca2-110">Method</span></span>       | <span data-ttu-id="4dca2-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4dca2-111">Return Type</span></span>  |<span data-ttu-id="4dca2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4dca2-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4dca2-113">Создание цепочки</span><span class="sxs-lookup"><span data-stu-id="4dca2-113">Create thread</span></span>](../api/channel-post-chatthreads.md) | [<span data-ttu-id="4dca2-114">chatThread</span><span class="sxs-lookup"><span data-stu-id="4dca2-114">chatThread</span></span>](chatthread.md) |<span data-ttu-id="4dca2-115">Начало новой цепочки беседы в указанном канале путем предоставления первого сообщения.</span><span class="sxs-lookup"><span data-stu-id="4dca2-115">Start a new thread in the specified channel, providing the first message.</span></span>|

## <a name="properties"></a><span data-ttu-id="4dca2-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="4dca2-116">Properties</span></span>
| <span data-ttu-id="4dca2-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="4dca2-117">Property</span></span>     | <span data-ttu-id="4dca2-118">Тип</span><span class="sxs-lookup"><span data-stu-id="4dca2-118">Type</span></span>   |<span data-ttu-id="4dca2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4dca2-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4dca2-120">id</span><span class="sxs-lookup"><span data-stu-id="4dca2-120">id</span></span>|<span data-ttu-id="4dca2-121">String</span><span class="sxs-lookup"><span data-stu-id="4dca2-121">String</span></span>| <span data-ttu-id="4dca2-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4dca2-122">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4dca2-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="4dca2-123">Relationships</span></span>
| <span data-ttu-id="4dca2-124">Связь</span><span class="sxs-lookup"><span data-stu-id="4dca2-124">Relationship</span></span> | <span data-ttu-id="4dca2-125">Тип</span><span class="sxs-lookup"><span data-stu-id="4dca2-125">Type</span></span>   |<span data-ttu-id="4dca2-126">Описание</span><span class="sxs-lookup"><span data-stu-id="4dca2-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4dca2-127">rootMessage</span><span class="sxs-lookup"><span data-stu-id="4dca2-127">rootMessage</span></span>|[<span data-ttu-id="4dca2-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="4dca2-128">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="4dca2-129">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4dca2-129">Nullable.</span></span>|
|<span data-ttu-id="4dca2-130">chatMessages</span><span class="sxs-lookup"><span data-stu-id="4dca2-130">chatMessages</span></span>|<span data-ttu-id="4dca2-131">Коллекция [chatMessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="4dca2-131">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="4dca2-132">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4dca2-132">Nullable.</span></span>|

> <span data-ttu-id="4dca2-133">В настоящее время эти отношения неявно существуют, но их нельзя прочитать или записать.</span><span class="sxs-lookup"><span data-stu-id="4dca2-133">Currently these relationships exist implicitly, but cannot read or written.</span></span>  <span data-ttu-id="4dca2-134">Эта возможность появится в будущих бета-выпусках API.</span><span class="sxs-lookup"><span data-stu-id="4dca2-134">Future beta API releases will support this.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4dca2-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4dca2-135">JSON representation</span></span>

<span data-ttu-id="4dca2-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4dca2-136">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
