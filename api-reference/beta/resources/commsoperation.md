---
title: Тип ресурса Коммсоператион
description: Состояние определенных длительных операций.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 07be6f3b5cf9e3d5e7a1a1300a94da9b5204a68a
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006700"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="cd339-103">Тип ресурса Коммсоператион</span><span class="sxs-lookup"><span data-stu-id="cd339-103">commsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd339-104">Представляет состояние определенных длительных операций.</span><span class="sxs-lookup"><span data-stu-id="cd339-104">Represents the status of certain long-running operations.</span></span>

<span data-ttu-id="cd339-105">Этот ресурс может быть возвращен в качестве ответа на действие или в качестве содержимого [коммснотификатион](commsNotification.md).</span><span class="sxs-lookup"><span data-stu-id="cd339-105">This resource can be returned as the response to an action, or as the content of a [commsNotification](commsNotification.md).</span></span>  

<span data-ttu-id="cd339-106">При возвращении в качестве ответа на действие состояние указывает, будут ли отображаться последующие уведомления.</span><span class="sxs-lookup"><span data-stu-id="cd339-106">When it is returned as a response to an action, the status indicates whether there will be subsequent notifications.</span></span> <span data-ttu-id="cd339-107">Если, например, операция со статусом `completed` или `failed` возвращена, дальнейшая операция с каналом уведомлений не будет выполняться.</span><span class="sxs-lookup"><span data-stu-id="cd339-107">If, for example, an operation with status of `completed` or `failed` is returned,  there will not be any subsequent operation via the notification channel.</span></span> 

<span data-ttu-id="cd339-108">Если `null` операция или операция со статусом `notStarted` или `running` возвращены, последующие обновления будут поступать через канал уведомлений.</span><span class="sxs-lookup"><span data-stu-id="cd339-108">If a `null` operation, or an operation with a status of `notStarted` or `running` is returned, subsequent updates will come via the notification channel.</span></span>

## <a name="properties"></a><span data-ttu-id="cd339-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd339-109">Properties</span></span>

| <span data-ttu-id="cd339-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd339-110">Property</span></span>           | <span data-ttu-id="cd339-111">Тип</span><span class="sxs-lookup"><span data-stu-id="cd339-111">Type</span></span>                        | <span data-ttu-id="cd339-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cd339-112">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="cd339-113">Контекст</span><span class="sxs-lookup"><span data-stu-id="cd339-113">clientContext</span></span>      | <span data-ttu-id="cd339-114">String</span><span class="sxs-lookup"><span data-stu-id="cd339-114">String</span></span>                      | <span data-ttu-id="cd339-115">Уникальная строка контекста клиента.</span><span class="sxs-lookup"><span data-stu-id="cd339-115">Unique Client Context string.</span></span> <span data-ttu-id="cd339-116">Максимальный лимит — 256 символов.</span><span class="sxs-lookup"><span data-stu-id="cd339-116">Max limit is 256 chars.</span></span>                           |
| <span data-ttu-id="cd339-117">id</span><span class="sxs-lookup"><span data-stu-id="cd339-117">id</span></span>                 | <span data-ttu-id="cd339-118">Строка</span><span class="sxs-lookup"><span data-stu-id="cd339-118">String</span></span>                      | <span data-ttu-id="cd339-119">ИДЕНТИФИКАТОР операции.</span><span class="sxs-lookup"><span data-stu-id="cd339-119">The operation ID.</span></span> <span data-ttu-id="cd339-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd339-120">Read-only.</span></span>                                                    |
| <span data-ttu-id="cd339-121">resultInfo</span><span class="sxs-lookup"><span data-stu-id="cd339-121">resultInfo</span></span>         | [<span data-ttu-id="cd339-122">resultInfo</span><span class="sxs-lookup"><span data-stu-id="cd339-122">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="cd339-123">Сведения о результате.</span><span class="sxs-lookup"><span data-stu-id="cd339-123">The result information.</span></span> <span data-ttu-id="cd339-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd339-124">Read-only.</span></span>                                              |
| <span data-ttu-id="cd339-125">status</span><span class="sxs-lookup"><span data-stu-id="cd339-125">status</span></span>             | <span data-ttu-id="cd339-126">String</span><span class="sxs-lookup"><span data-stu-id="cd339-126">String</span></span>                      | <span data-ttu-id="cd339-127">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="cd339-127">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="cd339-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd339-128">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cd339-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="cd339-129">Relationships</span></span>
<span data-ttu-id="cd339-130">Нет</span><span class="sxs-lookup"><span data-stu-id="cd339-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd339-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd339-131">JSON representation</span></span>

<span data-ttu-id="cd339-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd339-132">The following is a JSON representation of the resource.</span></span>

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
