---
title: Тип ресурса Принтоператион
description: Представляет длительную универсальную операцию печати. Базовый класс для типов операций, например Принтеркреатеоператион.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7b8f147106c6914fe8fbbb404ca0c78210c02026
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007236"
---
# <a name="printoperation-resource-type"></a><span data-ttu-id="b66b7-104">Тип ресурса Принтоператион</span><span class="sxs-lookup"><span data-stu-id="b66b7-104">printOperation resource type</span></span>

<span data-ttu-id="b66b7-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b66b7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b66b7-106">Представляет длительную универсальную операцию печати.</span><span class="sxs-lookup"><span data-stu-id="b66b7-106">Represents a long-running Universal Print operation.</span></span> <span data-ttu-id="b66b7-107">Базовый класс для типов операций, например [принтеркреатеоператион](printercreateoperation.md).</span><span class="sxs-lookup"><span data-stu-id="b66b7-107">Base class for operation types such as [printerCreateOperation](printercreateoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b66b7-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b66b7-108">Methods</span></span>

| <span data-ttu-id="b66b7-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b66b7-109">Method</span></span>       | <span data-ttu-id="b66b7-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b66b7-110">Return Type</span></span> | <span data-ttu-id="b66b7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b66b7-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b66b7-112">Получение операции</span><span class="sxs-lookup"><span data-stu-id="b66b7-112">Get operation</span></span>](../api/printoperation-get.md) | [<span data-ttu-id="b66b7-113">принтоператион</span><span class="sxs-lookup"><span data-stu-id="b66b7-113">printOperation</span></span>](printoperation.md) | <span data-ttu-id="b66b7-114">Получение длительной операции в текущем пользователе или клиенте приложения.</span><span class="sxs-lookup"><span data-stu-id="b66b7-114">Retrieve a long-running operation within current user or app's tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="b66b7-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="b66b7-115">Properties</span></span>
| <span data-ttu-id="b66b7-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="b66b7-116">Property</span></span>     | <span data-ttu-id="b66b7-117">Тип</span><span class="sxs-lookup"><span data-stu-id="b66b7-117">Type</span></span>        | <span data-ttu-id="b66b7-118">Описание</span><span class="sxs-lookup"><span data-stu-id="b66b7-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b66b7-119">id</span><span class="sxs-lookup"><span data-stu-id="b66b7-119">id</span></span>|<span data-ttu-id="b66b7-120">String</span><span class="sxs-lookup"><span data-stu-id="b66b7-120">String</span></span>|<span data-ttu-id="b66b7-121">Идентификатор операции.</span><span class="sxs-lookup"><span data-stu-id="b66b7-121">The operation's identifier.</span></span> <span data-ttu-id="b66b7-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b66b7-122">Read-only.</span></span>|
|<span data-ttu-id="b66b7-123">status</span><span class="sxs-lookup"><span data-stu-id="b66b7-123">status</span></span>|[<span data-ttu-id="b66b7-124">принтоператионстатус</span><span class="sxs-lookup"><span data-stu-id="b66b7-124">printOperationStatus</span></span>](printoperationstatus.md)|<span data-ttu-id="b66b7-125">Состояние операции.</span><span class="sxs-lookup"><span data-stu-id="b66b7-125">The status of the operation.</span></span> <span data-ttu-id="b66b7-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b66b7-126">Read-only.</span></span>|
|<span data-ttu-id="b66b7-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b66b7-127">createdDateTime</span></span>|<span data-ttu-id="b66b7-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b66b7-128">DateTimeOffset</span></span>|<span data-ttu-id="b66b7-129">Значение DateTimeOffset при создании операции.</span><span class="sxs-lookup"><span data-stu-id="b66b7-129">The DateTimeOffset when the operation was created.</span></span> <span data-ttu-id="b66b7-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b66b7-130">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b66b7-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b66b7-131">JSON representation</span></span>

<span data-ttu-id="b66b7-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b66b7-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printOperation",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
    "id": "String (identifier)",
    "status": {"@odata.type": "microsoft.graph.printOperationStatus"},
    "createdDateTime": "2020-06-15T19:54:14.853Z"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->