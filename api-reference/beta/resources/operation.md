---
title: Тип ресурса Operation
description: Состояние длительной операции.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 44d1bdfdca902652d77d978b0eae4cffdf359f39
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522161"
---
# <a name="operation-resource-type"></a><span data-ttu-id="b6783-103">Тип ресурса Operation</span><span class="sxs-lookup"><span data-stu-id="b6783-103">operation resource type</span></span>

<span data-ttu-id="b6783-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b6783-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6783-105">Состояние длительной операции.</span><span class="sxs-lookup"><span data-stu-id="b6783-105">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="b6783-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b6783-106">Methods</span></span>

<span data-ttu-id="b6783-107">Нет</span><span class="sxs-lookup"><span data-stu-id="b6783-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="b6783-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6783-108">Properties</span></span>

| <span data-ttu-id="b6783-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6783-109">Property</span></span>           | <span data-ttu-id="b6783-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b6783-110">Type</span></span>            | <span data-ttu-id="b6783-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b6783-111">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="b6783-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6783-112">createdDateTime</span></span>    | <span data-ttu-id="b6783-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6783-113">DateTimeOffset</span></span>  | <span data-ttu-id="b6783-114">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="b6783-114">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="b6783-115">id</span><span class="sxs-lookup"><span data-stu-id="b6783-115">id</span></span>                 | <span data-ttu-id="b6783-116">Строка</span><span class="sxs-lookup"><span data-stu-id="b6783-116">String</span></span>          | <span data-ttu-id="b6783-117">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6783-117">The operation id. Read-only.</span></span> <span data-ttu-id="b6783-118">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="b6783-118">Server generated.</span></span>                                  |
| <span data-ttu-id="b6783-119">ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="b6783-119">lastActionDateTime</span></span> | <span data-ttu-id="b6783-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6783-120">DateTimeOffset</span></span>  | <span data-ttu-id="b6783-121">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="b6783-121">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="b6783-122">status</span><span class="sxs-lookup"><span data-stu-id="b6783-122">status</span></span>             | <span data-ttu-id="b6783-123">String</span><span class="sxs-lookup"><span data-stu-id="b6783-123">String</span></span>          | <span data-ttu-id="b6783-124">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="b6783-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="b6783-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b6783-125">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b6783-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="b6783-126">Relationships</span></span>

<span data-ttu-id="b6783-127">Нет</span><span class="sxs-lookup"><span data-stu-id="b6783-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6783-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b6783-128">JSON representation</span></span>

<span data-ttu-id="b6783-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6783-129">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="b6783-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b6783-130">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "status": "completed"
}
```

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
