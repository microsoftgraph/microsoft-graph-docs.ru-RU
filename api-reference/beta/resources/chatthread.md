---
title: Тип ресурса chatThread
description: ChatThread — это коллекция chatMessages в группах Майкрософт.
ms.openlocfilehash: ef8f118ae4354a5e4197802708aecfa1fb6f8cb8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081634"
---
# <a name="chatthread-resource-type"></a><span data-ttu-id="fe237-103">Тип ресурса chatThread</span><span class="sxs-lookup"><span data-stu-id="fe237-103">chatThread resource type</span></span>

> <span data-ttu-id="fe237-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fe237-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe237-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe237-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe237-106">ChatThread — это коллекция [chatMessages](chatmessage.md) в группах Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="fe237-106">A chatThread is a collection of [chatMessages](chatmessage.md) in Microsoft Teams.</span></span>

> <span data-ttu-id="fe237-107">На данный момент chatThreads может быть [создано в каналы](../api/channel-post-chatthreads.md).</span><span class="sxs-lookup"><span data-stu-id="fe237-107">Currently, chatThreads can be [created in channels](../api/channel-post-chatthreads.md).</span></span>  <span data-ttu-id="fe237-108">Выпуски будущее API поддерживает чтения существующих chatThreads, а также чтения/записи прямого чаты между пользователями, которые являются выходят за рамки группы или канала.</span><span class="sxs-lookup"><span data-stu-id="fe237-108">Future API releases will support reading existing chatThreads, as well as reading/writing direct chats between users that are outside the scope of a team or channel.</span></span>

## <a name="methods"></a><span data-ttu-id="fe237-109">Методы</span><span class="sxs-lookup"><span data-stu-id="fe237-109">Methods</span></span>

| <span data-ttu-id="fe237-110">Метод</span><span class="sxs-lookup"><span data-stu-id="fe237-110">Method</span></span>       | <span data-ttu-id="fe237-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fe237-111">Return Type</span></span>  |<span data-ttu-id="fe237-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fe237-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fe237-113">Создание цепочки</span><span class="sxs-lookup"><span data-stu-id="fe237-113">Create thread</span></span>](../api/channel-post-chatthreads.md) | [<span data-ttu-id="fe237-114">chatThread</span><span class="sxs-lookup"><span data-stu-id="fe237-114">chatThread</span></span>](chatthread.md) |<span data-ttu-id="fe237-115">Запустите новый поток в указанный канал, предоставляя первого сообщения.</span><span class="sxs-lookup"><span data-stu-id="fe237-115">Start a new thread in the specified channel, providing the first message.</span></span>|

## <a name="properties"></a><span data-ttu-id="fe237-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe237-116">Properties</span></span>
| <span data-ttu-id="fe237-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe237-117">Property</span></span>     | <span data-ttu-id="fe237-118">Тип</span><span class="sxs-lookup"><span data-stu-id="fe237-118">Type</span></span>   |<span data-ttu-id="fe237-119">Описание</span><span class="sxs-lookup"><span data-stu-id="fe237-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe237-120">id</span><span class="sxs-lookup"><span data-stu-id="fe237-120">id</span></span>|<span data-ttu-id="fe237-121">String</span><span class="sxs-lookup"><span data-stu-id="fe237-121">String</span></span>| <span data-ttu-id="fe237-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe237-122">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe237-123">Связи</span><span class="sxs-lookup"><span data-stu-id="fe237-123">Relationships</span></span>
| <span data-ttu-id="fe237-124">Связь</span><span class="sxs-lookup"><span data-stu-id="fe237-124">Relationship</span></span> | <span data-ttu-id="fe237-125">Тип</span><span class="sxs-lookup"><span data-stu-id="fe237-125">Type</span></span>   |<span data-ttu-id="fe237-126">Description</span><span class="sxs-lookup"><span data-stu-id="fe237-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe237-127">rootMessage</span><span class="sxs-lookup"><span data-stu-id="fe237-127">rootMessage</span></span>|[<span data-ttu-id="fe237-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="fe237-128">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="fe237-129">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="fe237-129">Nullable.</span></span>|
|<span data-ttu-id="fe237-130">chatMessages</span><span class="sxs-lookup"><span data-stu-id="fe237-130">chatMessages</span></span>|<span data-ttu-id="fe237-131">[chatMessage](chatmessage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="fe237-131">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="fe237-132">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="fe237-132">Nullable.</span></span>|

> <span data-ttu-id="fe237-133">В настоящее время эти связи неявно, существует, но не может читать или записи.</span><span class="sxs-lookup"><span data-stu-id="fe237-133">Currently these relationships exist implicitly, but cannot read or written.</span></span>  <span data-ttu-id="fe237-134">Выпуски будущих бета-версии API будут поддерживать это.</span><span class="sxs-lookup"><span data-stu-id="fe237-134">Future beta API releases will support this.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe237-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe237-135">JSON representation</span></span>

<span data-ttu-id="fe237-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe237-136">Here is a JSON representation of the resource</span></span>

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
  "id": "string (identifier)",
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
