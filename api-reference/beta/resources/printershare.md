---
title: Тип ресурса Принтершаре
description: Представляет принтер, предназначенный для обнаружения пользователями и приложениями печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: a44cac259e9be653ca0e7b21c81b6c72224268b1
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896017"
---
# <a name="printershare-resource-type"></a><span data-ttu-id="d9472-103">Тип ресурса Принтершаре</span><span class="sxs-lookup"><span data-stu-id="d9472-103">printerShare resource type</span></span>

<span data-ttu-id="d9472-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9472-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9472-105">Представляет принтер, предназначенный для обнаружения пользователями и приложениями печати.</span><span class="sxs-lookup"><span data-stu-id="d9472-105">Represents a printer that is intended to be discoverable by users and printing applications.</span></span>

## <a name="methods"></a><span data-ttu-id="d9472-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d9472-106">Methods</span></span>

| <span data-ttu-id="d9472-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d9472-107">Method</span></span>       | <span data-ttu-id="d9472-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d9472-108">Return Type</span></span> | <span data-ttu-id="d9472-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d9472-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d9472-110">Список Принтершарес</span><span class="sxs-lookup"><span data-stu-id="d9472-110">List printerShares</span></span>](../api/print-list-printershares.md) | <span data-ttu-id="d9472-111">Коллекция [принтершаре](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="d9472-111">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="d9472-112">Получение списка общих принтеров в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d9472-112">Get a list of printer shares in the tenant.</span></span> |
| [<span data-ttu-id="d9472-113">Получение Принтершаре</span><span class="sxs-lookup"><span data-stu-id="d9472-113">Get printerShare</span></span>](../api/printershare-get.md) | [<span data-ttu-id="d9472-114">принтершаре</span><span class="sxs-lookup"><span data-stu-id="d9472-114">printerShare</span></span>](printershare.md) | <span data-ttu-id="d9472-115">Чтение свойств и связей объекта Принтершаре.</span><span class="sxs-lookup"><span data-stu-id="d9472-115">Read properties and relationships of a printerShare object.</span></span> |
| <span data-ttu-id="d9472-116">[обновление](../api/printershare-update.md).</span><span class="sxs-lookup"><span data-stu-id="d9472-116">[Update](../api/printershare-update.md)</span></span> | [<span data-ttu-id="d9472-117">принтершаре</span><span class="sxs-lookup"><span data-stu-id="d9472-117">printerShare</span></span>](printershare.md) | <span data-ttu-id="d9472-118">Обновление объекта Принтершаре.</span><span class="sxs-lookup"><span data-stu-id="d9472-118">Update a printerShare object.</span></span> |
| <span data-ttu-id="d9472-119">[удаление](../api/printershare-delete.md);</span><span class="sxs-lookup"><span data-stu-id="d9472-119">[Delete](../api/printershare-delete.md)</span></span> | <span data-ttu-id="d9472-120">Нет</span><span class="sxs-lookup"><span data-stu-id="d9472-120">None</span></span> | <span data-ttu-id="d9472-121">Отменяет общий доступ к принтеру.</span><span class="sxs-lookup"><span data-stu-id="d9472-121">Unshare a printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="d9472-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9472-122">Properties</span></span>
| <span data-ttu-id="d9472-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9472-123">Property</span></span>     | <span data-ttu-id="d9472-124">Тип</span><span class="sxs-lookup"><span data-stu-id="d9472-124">Type</span></span>        | <span data-ttu-id="d9472-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d9472-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d9472-126">id</span><span class="sxs-lookup"><span data-stu-id="d9472-126">id</span></span>|<span data-ttu-id="d9472-127">Строка</span><span class="sxs-lookup"><span data-stu-id="d9472-127">String</span></span>| <span data-ttu-id="d9472-128">Идентификатор Принтершаре.</span><span class="sxs-lookup"><span data-stu-id="d9472-128">The printerShare's identifier.</span></span> <span data-ttu-id="d9472-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d9472-129">Read-only.</span></span>|
|<span data-ttu-id="d9472-130">name</span><span class="sxs-lookup"><span data-stu-id="d9472-130">name</span></span>|<span data-ttu-id="d9472-131">String</span><span class="sxs-lookup"><span data-stu-id="d9472-131">String</span></span>|<span data-ttu-id="d9472-132">Имя общего принтера, который должен отображаться клиентами печати.</span><span class="sxs-lookup"><span data-stu-id="d9472-132">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="d9472-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9472-133">createdDateTime</span></span>|<span data-ttu-id="d9472-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9472-134">DateTimeOffset</span></span>|<span data-ttu-id="d9472-135">Значение DateTimeOffset при создании общего ресурса принтера.</span><span class="sxs-lookup"><span data-stu-id="d9472-135">The DateTimeOffset when the printer share was created.</span></span> <span data-ttu-id="d9472-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d9472-136">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9472-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="d9472-137">Relationships</span></span>
| <span data-ttu-id="d9472-138">Связь</span><span class="sxs-lookup"><span data-stu-id="d9472-138">Relationship</span></span> | <span data-ttu-id="d9472-139">Тип</span><span class="sxs-lookup"><span data-stu-id="d9472-139">Type</span></span>        | <span data-ttu-id="d9472-140">Описание</span><span class="sxs-lookup"><span data-stu-id="d9472-140">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d9472-141">Printer</span><span class="sxs-lookup"><span data-stu-id="d9472-141">printer</span></span>|[<span data-ttu-id="d9472-142">Printer</span><span class="sxs-lookup"><span data-stu-id="d9472-142">printer</span></span>](printer.md)|<span data-ttu-id="d9472-143">Принтер, с которым связан этот общий принтер.</span><span class="sxs-lookup"><span data-stu-id="d9472-143">The printer that this printer share is related to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d9472-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9472-144">JSON representation</span></span>

<span data-ttu-id="d9472-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9472-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerShare",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerShare resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->