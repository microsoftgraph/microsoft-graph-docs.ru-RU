---
title: Тип ресурса Operation
description: Состояние длительной операции.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 237e16373db30db9f4a9ed61c6182f6dd826d956
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966365"
---
# <a name="operation-resource-type"></a><span data-ttu-id="40368-103">Тип ресурса Operation</span><span class="sxs-lookup"><span data-stu-id="40368-103">operation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40368-104">Состояние длительной операции.</span><span class="sxs-lookup"><span data-stu-id="40368-104">The status of a long-running operation.</span></span>

## <a name="methods"></a><span data-ttu-id="40368-105">Методы</span><span class="sxs-lookup"><span data-stu-id="40368-105">Methods</span></span>

<span data-ttu-id="40368-106">Нет</span><span class="sxs-lookup"><span data-stu-id="40368-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="40368-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="40368-107">Properties</span></span>

| <span data-ttu-id="40368-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="40368-108">Property</span></span>           | <span data-ttu-id="40368-109">Тип</span><span class="sxs-lookup"><span data-stu-id="40368-109">Type</span></span>            | <span data-ttu-id="40368-110">Описание</span><span class="sxs-lookup"><span data-stu-id="40368-110">Description</span></span>                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="40368-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40368-111">createdDateTime</span></span>    | <span data-ttu-id="40368-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40368-112">DateTimeOffset</span></span>  | <span data-ttu-id="40368-113">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="40368-113">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="40368-114">id</span><span class="sxs-lookup"><span data-stu-id="40368-114">id</span></span>                 | <span data-ttu-id="40368-115">Строка</span><span class="sxs-lookup"><span data-stu-id="40368-115">String</span></span>          | <span data-ttu-id="40368-116">Идентификатор операции. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="40368-116">The operation id. Read-only.</span></span> <span data-ttu-id="40368-117">Создается сервером.</span><span class="sxs-lookup"><span data-stu-id="40368-117">Server generated.</span></span>                                  |
| <span data-ttu-id="40368-118">Ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="40368-118">lastActionDateTime</span></span> | <span data-ttu-id="40368-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40368-119">DateTimeOffset</span></span>  | <span data-ttu-id="40368-120">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="40368-120">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="40368-121">status</span><span class="sxs-lookup"><span data-stu-id="40368-121">status</span></span>             | <span data-ttu-id="40368-122">String</span><span class="sxs-lookup"><span data-stu-id="40368-122">String</span></span>          | <span data-ttu-id="40368-123">Возможные значения: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="40368-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="40368-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="40368-124">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="40368-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="40368-125">Relationships</span></span>

<span data-ttu-id="40368-126">Нет</span><span class="sxs-lookup"><span data-stu-id="40368-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40368-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40368-127">JSON representation</span></span>

<span data-ttu-id="40368-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40368-128">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="40368-129">Пример</span><span class="sxs-lookup"><span data-stu-id="40368-129">Example</span></span>

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
