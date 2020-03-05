---
title: Тип ресурса Коммсоператион
description: Состояние определенных длительных операций.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 7a73777ae8477275e9071645ce092ca1a4187527
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507592"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="5db19-103">Тип ресурса Коммсоператион</span><span class="sxs-lookup"><span data-stu-id="5db19-103">commsOperation resource type</span></span>

<span data-ttu-id="5db19-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5db19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5db19-105">Представляет состояние определенных длительных операций.</span><span class="sxs-lookup"><span data-stu-id="5db19-105">Represents the status of certain long-running operations.</span></span>

<span data-ttu-id="5db19-106">Этот ресурс может быть возвращен в качестве ответа на действие или в качестве содержимого [коммснотификатион](commsNotification.md).</span><span class="sxs-lookup"><span data-stu-id="5db19-106">This resource can be returned as the response to an action, or as the content of a [commsNotification](commsNotification.md).</span></span>  

<span data-ttu-id="5db19-107">При возвращении в качестве ответа на действие состояние указывает, будут ли отображаться последующие уведомления.</span><span class="sxs-lookup"><span data-stu-id="5db19-107">When it is returned as a response to an action, the status indicates whether there will be subsequent notifications.</span></span> <span data-ttu-id="5db19-108">Если, например, операция со статусом `completed` или `failed` возвращена, дальнейшая операция с каналом уведомлений не будет выполняться.</span><span class="sxs-lookup"><span data-stu-id="5db19-108">If, for example, an operation with status of `completed` or `failed` is returned,  there will not be any subsequent operation via the notification channel.</span></span> 

<span data-ttu-id="5db19-109">Если `null` операция или операция со статусом `notStarted` или `running` возвращены, последующие обновления будут поступать через канал уведомлений.</span><span class="sxs-lookup"><span data-stu-id="5db19-109">If a `null` operation, or an operation with a status of `notStarted` or `running` is returned, subsequent updates will come via the notification channel.</span></span>

## <a name="properties"></a><span data-ttu-id="5db19-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="5db19-110">Properties</span></span>

| <span data-ttu-id="5db19-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="5db19-111">Property</span></span>           | <span data-ttu-id="5db19-112">Тип</span><span class="sxs-lookup"><span data-stu-id="5db19-112">Type</span></span>                        | <span data-ttu-id="5db19-113">Описание</span><span class="sxs-lookup"><span data-stu-id="5db19-113">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="5db19-114">Контекст</span><span class="sxs-lookup"><span data-stu-id="5db19-114">clientContext</span></span>      | <span data-ttu-id="5db19-115">String</span><span class="sxs-lookup"><span data-stu-id="5db19-115">String</span></span>                      | <span data-ttu-id="5db19-116">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="5db19-116">Unique Client Context string.</span></span> <span data-ttu-id="5db19-117">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="5db19-117">Max limit is 256 chars.</span></span>                           |
| <span data-ttu-id="5db19-118">id</span><span class="sxs-lookup"><span data-stu-id="5db19-118">id</span></span>                 | <span data-ttu-id="5db19-119">Строка</span><span class="sxs-lookup"><span data-stu-id="5db19-119">String</span></span>                      | <span data-ttu-id="5db19-120">ИДЕНТИФИКАТОР операции.</span><span class="sxs-lookup"><span data-stu-id="5db19-120">The operation ID.</span></span> <span data-ttu-id="5db19-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5db19-121">Read-only.</span></span>                                                    |
| <span data-ttu-id="5db19-122">resultInfo</span><span class="sxs-lookup"><span data-stu-id="5db19-122">resultInfo</span></span>         | [<span data-ttu-id="5db19-123">resultInfo</span><span class="sxs-lookup"><span data-stu-id="5db19-123">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="5db19-124">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="5db19-124">The result information.</span></span> <span data-ttu-id="5db19-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5db19-125">Read-only.</span></span>                                              |
| <span data-ttu-id="5db19-126">status</span><span class="sxs-lookup"><span data-stu-id="5db19-126">status</span></span>             | <span data-ttu-id="5db19-127">String</span><span class="sxs-lookup"><span data-stu-id="5db19-127">String</span></span>                      | <span data-ttu-id="5db19-128">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="5db19-128">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="5db19-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5db19-129">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5db19-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="5db19-130">Relationships</span></span>
<span data-ttu-id="5db19-131">Нет</span><span class="sxs-lookup"><span data-stu-id="5db19-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5db19-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5db19-132">JSON representation</span></span>

<span data-ttu-id="5db19-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5db19-133">The following is a JSON representation of the resource.</span></span>

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
