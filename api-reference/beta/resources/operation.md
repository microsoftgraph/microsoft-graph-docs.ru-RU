---
title: Тип ресурса Operation
description: Состояние длительной операции.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: billbliss
ms.openlocfilehash: e94970609c2ccfb99e61b254b080e1dbaa244ba6
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809315"
---
# <a name="operation-resource-type"></a><span data-ttu-id="acf7f-103">Тип ресурса Operation</span><span class="sxs-lookup"><span data-stu-id="acf7f-103">operation resource type</span></span>

<span data-ttu-id="acf7f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acf7f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acf7f-105">Состояние длительной операции.</span><span class="sxs-lookup"><span data-stu-id="acf7f-105">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="acf7f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="acf7f-106">Methods</span></span>

<span data-ttu-id="acf7f-107">Нет</span><span class="sxs-lookup"><span data-stu-id="acf7f-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="acf7f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="acf7f-108">Properties</span></span>

| <span data-ttu-id="acf7f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="acf7f-109">Property</span></span>           | <span data-ttu-id="acf7f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="acf7f-110">Type</span></span>            | <span data-ttu-id="acf7f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="acf7f-111">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="acf7f-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="acf7f-112">createdDateTime</span></span>    | <span data-ttu-id="acf7f-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acf7f-113">DateTimeOffset</span></span>  | <span data-ttu-id="acf7f-114">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="acf7f-114">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="acf7f-115">id</span><span class="sxs-lookup"><span data-stu-id="acf7f-115">id</span></span>                 | <span data-ttu-id="acf7f-116">String</span><span class="sxs-lookup"><span data-stu-id="acf7f-116">String</span></span>          | <span data-ttu-id="acf7f-117">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="acf7f-117">The operation id. Read-only.</span></span> <span data-ttu-id="acf7f-118">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="acf7f-118">Server generated.</span></span>                                  |
| <span data-ttu-id="acf7f-119">ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="acf7f-119">lastActionDateTime</span></span> | <span data-ttu-id="acf7f-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acf7f-120">DateTimeOffset</span></span>  | <span data-ttu-id="acf7f-121">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="acf7f-121">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="acf7f-122">status</span><span class="sxs-lookup"><span data-stu-id="acf7f-122">status</span></span>             | <span data-ttu-id="acf7f-123">String</span><span class="sxs-lookup"><span data-stu-id="acf7f-123">String</span></span>          | <span data-ttu-id="acf7f-124">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="acf7f-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="acf7f-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="acf7f-125">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="acf7f-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="acf7f-126">Relationships</span></span>

<span data-ttu-id="acf7f-127">Нет</span><span class="sxs-lookup"><span data-stu-id="acf7f-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="acf7f-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="acf7f-128">JSON representation</span></span>

<span data-ttu-id="acf7f-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="acf7f-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="acf7f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="acf7f-130">Example</span></span>

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
