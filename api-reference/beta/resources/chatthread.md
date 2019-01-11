---
title: Тип ресурса chatThread
description: ChatThread — это коллекция chatMessages в группах Майкрософт.
localization_priority: Priority
ms.openlocfilehash: 5060d7ea846f5aedec5551aaf247642a36f73c1c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833245"
---
# <a name="chatthread-resource-type"></a><span data-ttu-id="89614-103">Тип ресурса chatThread</span><span class="sxs-lookup"><span data-stu-id="89614-103">chatThread resource type</span></span>

> <span data-ttu-id="89614-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="89614-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89614-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89614-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="89614-106">ChatThread — это коллекция [chatMessages](chatmessage.md) в группах Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="89614-106">A chatThread is a collection of [chatMessages](chatmessage.md) in Microsoft Teams.</span></span>

> <span data-ttu-id="89614-107">На данный момент chatThreads может быть [создано в каналы](../api/channel-post-chatthreads.md).</span><span class="sxs-lookup"><span data-stu-id="89614-107">Currently, chatThreads can be [created in channels](../api/channel-post-chatthreads.md).</span></span>  <span data-ttu-id="89614-108">Выпуски будущее API поддерживает чтения существующих chatThreads, а также чтения/записи прямого чаты между пользователями, которые являются выходят за рамки группы или канала.</span><span class="sxs-lookup"><span data-stu-id="89614-108">Future API releases will support reading existing chatThreads, as well as reading/writing direct chats between users that are outside the scope of a team or channel.</span></span>

## <a name="methods"></a><span data-ttu-id="89614-109">Методы</span><span class="sxs-lookup"><span data-stu-id="89614-109">Methods</span></span>

| <span data-ttu-id="89614-110">Метод</span><span class="sxs-lookup"><span data-stu-id="89614-110">Method</span></span>       | <span data-ttu-id="89614-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="89614-111">Return Type</span></span>  |<span data-ttu-id="89614-112">Описание</span><span class="sxs-lookup"><span data-stu-id="89614-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="89614-113">Создание цепочки</span><span class="sxs-lookup"><span data-stu-id="89614-113">Create thread</span></span>](../api/channel-post-chatthreads.md) | [<span data-ttu-id="89614-114">chatThread</span><span class="sxs-lookup"><span data-stu-id="89614-114">chatThread</span></span>](chatthread.md) |<span data-ttu-id="89614-115">Запустите новый поток в указанный канал, предоставляя первого сообщения.</span><span class="sxs-lookup"><span data-stu-id="89614-115">Start a new thread in the specified channel, providing the first message.</span></span>|

## <a name="properties"></a><span data-ttu-id="89614-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="89614-116">Properties</span></span>
| <span data-ttu-id="89614-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="89614-117">Property</span></span>     | <span data-ttu-id="89614-118">Тип</span><span class="sxs-lookup"><span data-stu-id="89614-118">Type</span></span>   |<span data-ttu-id="89614-119">Описание</span><span class="sxs-lookup"><span data-stu-id="89614-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89614-120">id</span><span class="sxs-lookup"><span data-stu-id="89614-120">id</span></span>|<span data-ttu-id="89614-121">Строка</span><span class="sxs-lookup"><span data-stu-id="89614-121">String</span></span>| <span data-ttu-id="89614-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89614-122">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89614-123">Связи</span><span class="sxs-lookup"><span data-stu-id="89614-123">Relationships</span></span>
| <span data-ttu-id="89614-124">Связь</span><span class="sxs-lookup"><span data-stu-id="89614-124">Relationship</span></span> | <span data-ttu-id="89614-125">Тип</span><span class="sxs-lookup"><span data-stu-id="89614-125">Type</span></span>   |<span data-ttu-id="89614-126">Описание</span><span class="sxs-lookup"><span data-stu-id="89614-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89614-127">rootMessage</span><span class="sxs-lookup"><span data-stu-id="89614-127">rootMessage</span></span>|[<span data-ttu-id="89614-128">chatMessage</span><span class="sxs-lookup"><span data-stu-id="89614-128">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="89614-129">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="89614-129">Nullable.</span></span>|
|<span data-ttu-id="89614-130">chatMessages</span><span class="sxs-lookup"><span data-stu-id="89614-130">chatMessages</span></span>|<span data-ttu-id="89614-131">[chatMessage](chatmessage.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="89614-131">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="89614-132">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="89614-132">Nullable.</span></span>|

> <span data-ttu-id="89614-133">В настоящее время эти связи неявно, существует, но не может читать или записи.</span><span class="sxs-lookup"><span data-stu-id="89614-133">Currently these relationships exist implicitly, but cannot read or written.</span></span>  <span data-ttu-id="89614-134">Выпуски будущих бета-версии API будут поддерживать это.</span><span class="sxs-lookup"><span data-stu-id="89614-134">Future beta API releases will support this.</span></span>

## <a name="json-representation"></a><span data-ttu-id="89614-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89614-135">JSON representation</span></span>

<span data-ttu-id="89614-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89614-136">Here is a JSON representation of the resource</span></span>

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
