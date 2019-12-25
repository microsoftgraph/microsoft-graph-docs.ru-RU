---
title: Тип ресурса Коммсоператион
description: Состояние определенных длительных операций.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 47937d059f9a624ca5b9c58333275081d5a68400
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866275"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="66b70-103">Тип ресурса Коммсоператион</span><span class="sxs-lookup"><span data-stu-id="66b70-103">commsOperation resource type</span></span>

<span data-ttu-id="66b70-104">Представляет состояние определенных длительных операций.</span><span class="sxs-lookup"><span data-stu-id="66b70-104">Represents the status of certain long-running operations.</span></span>

<span data-ttu-id="66b70-105">Этот ресурс может быть возвращен в качестве ответа на действие или в качестве содержимого [коммснотификатион](commsNotification.md).</span><span class="sxs-lookup"><span data-stu-id="66b70-105">This resource can be returned as the response to an action, or as the content of a [commsNotification](commsNotification.md).</span></span>  

<span data-ttu-id="66b70-106">При возвращении в качестве ответа на действие состояние указывает, будут ли отображаться последующие уведомления.</span><span class="sxs-lookup"><span data-stu-id="66b70-106">When it is returned as a response to an action, the status indicates whether there will be subsequent notifications.</span></span> <span data-ttu-id="66b70-107">Если, например, операция со статусом `completed` или `failed` возвращена, дальнейшая операция с каналом уведомлений не будет выполняться.</span><span class="sxs-lookup"><span data-stu-id="66b70-107">If, for example, an operation with status of `completed` or `failed` is returned,  there will not be any subsequent operation via the notification channel.</span></span> 

<span data-ttu-id="66b70-108">Если `null` операция или операция со статусом `notStarted` или `running` возвращены, последующие обновления будут поступать через канал уведомлений.</span><span class="sxs-lookup"><span data-stu-id="66b70-108">If a `null` operation, or an operation with a status of `notStarted` or `running` is returned, subsequent updates will come via the notification channel.</span></span>

## <a name="properties"></a><span data-ttu-id="66b70-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="66b70-109">Properties</span></span>

| <span data-ttu-id="66b70-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="66b70-110">Property</span></span>           | <span data-ttu-id="66b70-111">Тип</span><span class="sxs-lookup"><span data-stu-id="66b70-111">Type</span></span>                        | <span data-ttu-id="66b70-112">Описание</span><span class="sxs-lookup"><span data-stu-id="66b70-112">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="66b70-113">Контекст</span><span class="sxs-lookup"><span data-stu-id="66b70-113">clientContext</span></span>      | <span data-ttu-id="66b70-114">String</span><span class="sxs-lookup"><span data-stu-id="66b70-114">String</span></span>                      | <span data-ttu-id="66b70-115">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="66b70-115">Unique Client Context string.</span></span> <span data-ttu-id="66b70-116">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="66b70-116">Max limit is 256 chars.</span></span>                           |
| <span data-ttu-id="66b70-117">id</span><span class="sxs-lookup"><span data-stu-id="66b70-117">id</span></span>                 | <span data-ttu-id="66b70-118">Строка</span><span class="sxs-lookup"><span data-stu-id="66b70-118">String</span></span>                      | <span data-ttu-id="66b70-119">ИДЕНТИФИКАТОР операции.</span><span class="sxs-lookup"><span data-stu-id="66b70-119">The operation ID.</span></span> <span data-ttu-id="66b70-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="66b70-120">Read-only.</span></span>                                                    |
| <span data-ttu-id="66b70-121">resultInfo</span><span class="sxs-lookup"><span data-stu-id="66b70-121">resultInfo</span></span>         | [<span data-ttu-id="66b70-122">resultInfo</span><span class="sxs-lookup"><span data-stu-id="66b70-122">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="66b70-123">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="66b70-123">The result information.</span></span> <span data-ttu-id="66b70-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="66b70-124">Read-only.</span></span>                                              |
| <span data-ttu-id="66b70-125">status</span><span class="sxs-lookup"><span data-stu-id="66b70-125">status</span></span>             | <span data-ttu-id="66b70-126">String</span><span class="sxs-lookup"><span data-stu-id="66b70-126">String</span></span>                      | <span data-ttu-id="66b70-127">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="66b70-127">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="66b70-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="66b70-128">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="66b70-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="66b70-129">Relationships</span></span>
<span data-ttu-id="66b70-130">Нет</span><span class="sxs-lookup"><span data-stu-id="66b70-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66b70-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66b70-131">JSON representation</span></span>

<span data-ttu-id="66b70-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66b70-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
