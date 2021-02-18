---
title: Тип ресурса print
description: При подписке на универсальную печать функция печати позволяет управлять принтерами и обнаруживать точки printServiceEndpoints, которые можно использовать для управления принтерами и заданиями печати в универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 0604044824d153c9e6d39586c2ca58ee9ca893ea
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292261"
---
# <a name="print-resource-type"></a><span data-ttu-id="c674a-103">Тип ресурса print</span><span class="sxs-lookup"><span data-stu-id="c674a-103">print resource type</span></span>

<span data-ttu-id="c674a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c674a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c674a-105">При подписке на универсальную печать функция печати позволяет управлять принтерами и обнаруживать точки [printServiceEndpoints,](printserviceendpoint.md) которые можно использовать для управления принтерами и заданиями печати в универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="c674a-105">When accompanied by a Universal Print subscription, the Print feature enables management of printers and discovery of [printServiceEndpoints](printserviceendpoint.md) that can be used to manage printers and print jobs within Universal Print.</span></span>

## <a name="methods"></a><span data-ttu-id="c674a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="c674a-106">Methods</span></span>
| <span data-ttu-id="c674a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="c674a-107">Method</span></span>       | <span data-ttu-id="c674a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c674a-108">Return Type</span></span> | <span data-ttu-id="c674a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c674a-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c674a-110">Перечисление соединителей</span><span class="sxs-lookup"><span data-stu-id="c674a-110">List connectors</span></span>](../api/print-list-connectors.md) | <span data-ttu-id="c674a-111">[Коллекция printConnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="c674a-111">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="c674a-112">Получите список соединители печати.</span><span class="sxs-lookup"><span data-stu-id="c674a-112">Get a list of print connectors.</span></span> |
| [<span data-ttu-id="c674a-113">Перечисление принтеров</span><span class="sxs-lookup"><span data-stu-id="c674a-113">List printers</span></span>](../api/print-list-printers.md) | <span data-ttu-id="c674a-114">[коллекция принтеров](printer.md)</span><span class="sxs-lookup"><span data-stu-id="c674a-114">[printer](printer.md) collection</span></span> | <span data-ttu-id="c674a-115">Получите список принтеров.</span><span class="sxs-lookup"><span data-stu-id="c674a-115">Get a list of printers.</span></span> |
| [<span data-ttu-id="c674a-116">Перечисление общих ресурсов</span><span class="sxs-lookup"><span data-stu-id="c674a-116">List shares</span></span>](../api/print-list-shares.md) | <span data-ttu-id="c674a-117">[Коллекция printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="c674a-117">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="c674a-118">Получите список обетов принтеров.</span><span class="sxs-lookup"><span data-stu-id="c674a-118">Get a list of printer shares.</span></span> |
| [<span data-ttu-id="c674a-119">Список служб</span><span class="sxs-lookup"><span data-stu-id="c674a-119">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="c674a-120">[Коллекция printService](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="c674a-120">[printService](printservice.md) collection</span></span> | <span data-ttu-id="c674a-121">Получите список служб.</span><span class="sxs-lookup"><span data-stu-id="c674a-121">Get a list of services.</span></span> |
| [<span data-ttu-id="c674a-122">Создание printerShare</span><span class="sxs-lookup"><span data-stu-id="c674a-122">Create printerShare</span></span>](../api/print-post-shares.md) | [<span data-ttu-id="c674a-123">printerShare</span><span class="sxs-lookup"><span data-stu-id="c674a-123">printerShare</span></span>](printershare.md) | <span data-ttu-id="c674a-124">Создание новой обоймы принтера путем публикации в **коллекции.**</span><span class="sxs-lookup"><span data-stu-id="c674a-124">Create a new printer share by posting to the **shares** collection.</span></span> |
| [<span data-ttu-id="c674a-125">Создание принтера</span><span class="sxs-lookup"><span data-stu-id="c674a-125">Create printer</span></span>](../api/printer-create.md) | [<span data-ttu-id="c674a-126">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="c674a-126">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="c674a-127">Создайте (зарегистрируйте) новый принтер с помощью универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="c674a-127">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="c674a-128">Обновление параметров</span><span class="sxs-lookup"><span data-stu-id="c674a-128">Update settings</span></span>](../api/print-update-settings.md) |  [<span data-ttu-id="c674a-129">printSettings</span><span class="sxs-lookup"><span data-stu-id="c674a-129">printSettings</span></span>](printsettings.md) | <span data-ttu-id="c674a-130">Обновляет параметры службы универсальной печати на всем клиенте.</span><span class="sxs-lookup"><span data-stu-id="c674a-130">Updates tenant-wide settings for the Universal Print service.</span></span> |
| [<span data-ttu-id="c674a-131">Перечисление taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="c674a-131">List taskDefinitions</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="c674a-132">[Коллекция printTaskDefinition](printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c674a-132">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="c674a-133">Получите список printTaskDefinitions на всем клиенте, созданный в универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="c674a-133">Get a tenant-wide list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="c674a-134">Создание taskDefinition</span><span class="sxs-lookup"><span data-stu-id="c674a-134">Create taskDefinition</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="c674a-135">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="c674a-135">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="c674a-136">Создайте новый printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="c674a-136">Create a new printTaskDefinition.</span></span> |
| [<span data-ttu-id="c674a-137">Обновление taskDefinition</span><span class="sxs-lookup"><span data-stu-id="c674a-137">Update taskDefinition</span></span>](../api/print-update-taskdefinition.md) | [<span data-ttu-id="c674a-138">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="c674a-138">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="c674a-139">Обновление printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="c674a-139">Update a printTaskDefinition.</span></span> |
| [<span data-ttu-id="c674a-140">Удаление taskDefinition</span><span class="sxs-lookup"><span data-stu-id="c674a-140">Delete taskDefinition</span></span>](../api/print-delete-taskdefinition.md) | <span data-ttu-id="c674a-141">Нет</span><span class="sxs-lookup"><span data-stu-id="c674a-141">None</span></span> | <span data-ttu-id="c674a-142">Удаление printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="c674a-142">Delete a printTaskDefinition.</span></span> |

## <a name="properties"></a><span data-ttu-id="c674a-143">Свойства</span><span class="sxs-lookup"><span data-stu-id="c674a-143">Properties</span></span>
| <span data-ttu-id="c674a-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="c674a-144">Property</span></span>     | <span data-ttu-id="c674a-145">Тип</span><span class="sxs-lookup"><span data-stu-id="c674a-145">Type</span></span>        | <span data-ttu-id="c674a-146">Описание</span><span class="sxs-lookup"><span data-stu-id="c674a-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c674a-147">параметры</span><span class="sxs-lookup"><span data-stu-id="c674a-147">settings</span></span>|[<span data-ttu-id="c674a-148">printSettings</span><span class="sxs-lookup"><span data-stu-id="c674a-148">printSettings</span></span>](printsettings.md)|<span data-ttu-id="c674a-149">Параметры универсальной печати на всем клиенте.</span><span class="sxs-lookup"><span data-stu-id="c674a-149">Tenant-wide settings for the Universal Print service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c674a-150">Связи</span><span class="sxs-lookup"><span data-stu-id="c674a-150">Relationships</span></span>
| <span data-ttu-id="c674a-151">Связь</span><span class="sxs-lookup"><span data-stu-id="c674a-151">Relationship</span></span> | <span data-ttu-id="c674a-152">Тип</span><span class="sxs-lookup"><span data-stu-id="c674a-152">Type</span></span>        | <span data-ttu-id="c674a-153">Описание</span><span class="sxs-lookup"><span data-stu-id="c674a-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c674a-154">services</span><span class="sxs-lookup"><span data-stu-id="c674a-154">services</span></span>|<span data-ttu-id="c674a-155">[Коллекция printService](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="c674a-155">[printService](printservice.md) collection</span></span>|<span data-ttu-id="c674a-156">Список доступных конечных точек службы универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="c674a-156">The list of available Universal Print service endpoints.</span></span>|
|<span data-ttu-id="c674a-157">printers</span><span class="sxs-lookup"><span data-stu-id="c674a-157">printers</span></span>|<span data-ttu-id="c674a-158">[коллекция принтеров](printer.md)</span><span class="sxs-lookup"><span data-stu-id="c674a-158">[printer](printer.md) collection</span></span>|<span data-ttu-id="c674a-159">Список принтеров, зарегистрированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c674a-159">The list of printers registered in the tenant.</span></span>|
|<span data-ttu-id="c674a-160">shares</span><span class="sxs-lookup"><span data-stu-id="c674a-160">shares</span></span>|<span data-ttu-id="c674a-161">[Коллекция printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="c674a-161">[printerShare](printershare.md) collection</span></span>|<span data-ttu-id="c674a-162">Список акций принтера, зарегистрированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c674a-162">The list of printer shares registered in the tenant.</span></span>|
|<span data-ttu-id="c674a-163">соединители</span><span class="sxs-lookup"><span data-stu-id="c674a-163">connectors</span></span>|<span data-ttu-id="c674a-164">[Коллекция printConnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="c674a-164">[printConnector](printconnector.md) collection</span></span>|<span data-ttu-id="c674a-165">Список доступных соединители печати.</span><span class="sxs-lookup"><span data-stu-id="c674a-165">The list of available print connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c674a-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c674a-166">JSON representation</span></span>

<span data-ttu-id="c674a-167">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c674a-167">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.print",
  "keyProperty": "settings"
}-->

```json
{
  "settings": {"@odata.type": "microsoft.graph.printSettings"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "print resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [ 
  ]
}-->


