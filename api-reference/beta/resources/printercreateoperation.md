---
title: Тип ресурса Принтеркреатеоператион
description: Представляет длительную операцию регистрации принтеров. Производный от Принтоператион.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 54f458e14cbda209d9c2d85f08df4c106db6ab00
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007244"
---
# <a name="printercreateoperation-resource-type"></a><span data-ttu-id="4f03d-104">Тип ресурса Принтеркреатеоператион</span><span class="sxs-lookup"><span data-stu-id="4f03d-104">printerCreateOperation resource type</span></span>

<span data-ttu-id="4f03d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f03d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f03d-106">Представляет длительную операцию регистрации принтеров.</span><span class="sxs-lookup"><span data-stu-id="4f03d-106">Represents a long-running printer registration operation.</span></span> <span data-ttu-id="4f03d-107">Производный от [принтоператион](printoperation.md).</span><span class="sxs-lookup"><span data-stu-id="4f03d-107">Derived from [printOperation](printoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4f03d-108">Методы</span><span class="sxs-lookup"><span data-stu-id="4f03d-108">Methods</span></span>

| <span data-ttu-id="4f03d-109">Метод</span><span class="sxs-lookup"><span data-stu-id="4f03d-109">Method</span></span>       | <span data-ttu-id="4f03d-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4f03d-110">Return Type</span></span> | <span data-ttu-id="4f03d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4f03d-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4f03d-112">Получение операции</span><span class="sxs-lookup"><span data-stu-id="4f03d-112">Get operation</span></span>](../api/printoperation-get.md) | [<span data-ttu-id="4f03d-113">принтоператион</span><span class="sxs-lookup"><span data-stu-id="4f03d-113">printOperation</span></span>](printoperation.md) | <span data-ttu-id="4f03d-114">Получение длительной операции в текущем пользователе или клиенте приложения.</span><span class="sxs-lookup"><span data-stu-id="4f03d-114">Retrieve a long-running operation within current user or app's tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="4f03d-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f03d-115">Properties</span></span>
| <span data-ttu-id="4f03d-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f03d-116">Property</span></span>     | <span data-ttu-id="4f03d-117">Тип</span><span class="sxs-lookup"><span data-stu-id="4f03d-117">Type</span></span>        | <span data-ttu-id="4f03d-118">Описание</span><span class="sxs-lookup"><span data-stu-id="4f03d-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4f03d-119">id</span><span class="sxs-lookup"><span data-stu-id="4f03d-119">id</span></span>|<span data-ttu-id="4f03d-120">String</span><span class="sxs-lookup"><span data-stu-id="4f03d-120">String</span></span>|<span data-ttu-id="4f03d-121">Идентификатор операции.</span><span class="sxs-lookup"><span data-stu-id="4f03d-121">The operation's identifier.</span></span> <span data-ttu-id="4f03d-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f03d-122">Read-only.</span></span>|
|<span data-ttu-id="4f03d-123">status</span><span class="sxs-lookup"><span data-stu-id="4f03d-123">status</span></span>|[<span data-ttu-id="4f03d-124">принтоператионстатус</span><span class="sxs-lookup"><span data-stu-id="4f03d-124">printOperationStatus</span></span>](printoperationstatus.md)|<span data-ttu-id="4f03d-125">Состояние операции регистрации.</span><span class="sxs-lookup"><span data-stu-id="4f03d-125">The status of the registration operation.</span></span> <span data-ttu-id="4f03d-126">Содержит ход выполнения операции, а также сведения о ее успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="4f03d-126">Contains the operation's progress and whether it completed successfully.</span></span> <span data-ttu-id="4f03d-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f03d-127">Read-only.</span></span>|
|<span data-ttu-id="4f03d-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f03d-128">createdDateTime</span></span>|<span data-ttu-id="4f03d-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f03d-129">DateTimeOffset</span></span>|<span data-ttu-id="4f03d-130">Значение DateTimeOffset при создании операции.</span><span class="sxs-lookup"><span data-stu-id="4f03d-130">The DateTimeOffset when the operation was created.</span></span> <span data-ttu-id="4f03d-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f03d-131">Read-only.</span></span>|
|<span data-ttu-id="4f03d-132">certificate</span><span class="sxs-lookup"><span data-stu-id="4f03d-132">certificate</span></span>|<span data-ttu-id="4f03d-133">String</span><span class="sxs-lookup"><span data-stu-id="4f03d-133">String</span></span>|<span data-ttu-id="4f03d-134">Подписанный сертификат, созданный в процессе регистрации.</span><span class="sxs-lookup"><span data-stu-id="4f03d-134">The signed certificate created during the registration process.</span></span> <span data-ttu-id="4f03d-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f03d-135">Read-only.</span></span>|
|<span data-ttu-id="4f03d-136">Printer</span><span class="sxs-lookup"><span data-stu-id="4f03d-136">printer</span></span>|[<span data-ttu-id="4f03d-137">Printer</span><span class="sxs-lookup"><span data-stu-id="4f03d-137">printer</span></span>](printer.md)|<span data-ttu-id="4f03d-138">Созданная сущность принтера.</span><span class="sxs-lookup"><span data-stu-id="4f03d-138">The created printer entity.</span></span> <span data-ttu-id="4f03d-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f03d-139">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f03d-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f03d-140">JSON representation</span></span>

<span data-ttu-id="4f03d-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f03d-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerCreateOperation",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
    "id": "String (identifier)",
    "status": {"@odata.type": "microsoft.graph.printOperationStatus"},
    "createdDateTime": "2020-06-15T19:54:14.853Z",
    "certificate": "",
    "printer": {"@odata.type": "microsoft.graph.printer"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerCreateOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->