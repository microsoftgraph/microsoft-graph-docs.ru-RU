---
title: Тип ресурса Print
description: С помощью универсальной подписки на печать функция печати позволяет управлять принтерами и обнаруживать Принтсервицеендпоинтс, которые можно использовать для управления принтерами и заданиями печати в универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 309b7c8e62b94703bb00e21fb8c8ed2a2e917efe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985890"
---
# <a name="print-resource-type"></a><span data-ttu-id="c90e2-103">Тип ресурса Print</span><span class="sxs-lookup"><span data-stu-id="c90e2-103">print resource type</span></span>

<span data-ttu-id="c90e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c90e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c90e2-105">С помощью универсальной подписки на печать функция печати позволяет управлять принтерами и обнаруживать [принтсервицеендпоинтс](printserviceendpoint.md) , которые можно использовать для управления принтерами и заданиями печати в универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="c90e2-105">When accompanied by a Universal Print subscription, the Print feature enables management of printers and discovery of [printServiceEndpoints](printserviceendpoint.md) that can be used to manage printers and print jobs within Universal Print.</span></span>

## <a name="methods"></a><span data-ttu-id="c90e2-106">Методы</span><span class="sxs-lookup"><span data-stu-id="c90e2-106">Methods</span></span>
| <span data-ttu-id="c90e2-107">Метод</span><span class="sxs-lookup"><span data-stu-id="c90e2-107">Method</span></span>       | <span data-ttu-id="c90e2-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c90e2-108">Return Type</span></span> | <span data-ttu-id="c90e2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c90e2-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c90e2-110">Перечисление соединителей</span><span class="sxs-lookup"><span data-stu-id="c90e2-110">List connectors</span></span>](../api/print-list-connectors.md) | <span data-ttu-id="c90e2-111">Коллекция [принтконнектор](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="c90e2-111">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="c90e2-112">Получение списка соединителей печати.</span><span class="sxs-lookup"><span data-stu-id="c90e2-112">Get a list of print connectors.</span></span> |
| [<span data-ttu-id="c90e2-113">Перечисление принтеров</span><span class="sxs-lookup"><span data-stu-id="c90e2-113">List printers</span></span>](../api/print-list-printers.md) | <span data-ttu-id="c90e2-114">Коллекция [принтеров](printer.md)</span><span class="sxs-lookup"><span data-stu-id="c90e2-114">[printer](printer.md) collection</span></span> | <span data-ttu-id="c90e2-115">Получение списка принтеров.</span><span class="sxs-lookup"><span data-stu-id="c90e2-115">Get a list of printers.</span></span> |
| [<span data-ttu-id="c90e2-116">Перечисление общих ресурсов</span><span class="sxs-lookup"><span data-stu-id="c90e2-116">List shares</span></span>](../api/print-list-shares.md) | <span data-ttu-id="c90e2-117">Коллекция [принтершаре](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="c90e2-117">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="c90e2-118">Получение списка общих принтеров.</span><span class="sxs-lookup"><span data-stu-id="c90e2-118">Get a list of printer shares.</span></span> |
| [<span data-ttu-id="c90e2-119">Список служб</span><span class="sxs-lookup"><span data-stu-id="c90e2-119">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="c90e2-120">Коллекция [принтсервице](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="c90e2-120">[printService](printservice.md) collection</span></span> | <span data-ttu-id="c90e2-121">Получение списка служб.</span><span class="sxs-lookup"><span data-stu-id="c90e2-121">Get a list of services.</span></span> |
| [<span data-ttu-id="c90e2-122">Создание printerShare</span><span class="sxs-lookup"><span data-stu-id="c90e2-122">Create printerShare</span></span>](../api/print-post-shares.md) | [<span data-ttu-id="c90e2-123">принтершаре</span><span class="sxs-lookup"><span data-stu-id="c90e2-123">printerShare</span></span>](printershare.md) | <span data-ttu-id="c90e2-124">Создайте новый общий ресурс для принтера, отправив его в коллекцию **shares** .</span><span class="sxs-lookup"><span data-stu-id="c90e2-124">Create a new printer share by posting to the **shares** collection.</span></span> |
| [<span data-ttu-id="c90e2-125">Создание принтера</span><span class="sxs-lookup"><span data-stu-id="c90e2-125">Create printer</span></span>](../api/printer-create.md) | [<span data-ttu-id="c90e2-126">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="c90e2-126">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="c90e2-127">Создание (регистрация) нового принтера с универсальной печатью.</span><span class="sxs-lookup"><span data-stu-id="c90e2-127">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="c90e2-128">Обновление параметров</span><span class="sxs-lookup"><span data-stu-id="c90e2-128">Update settings</span></span>](../api/print-update-settings.md) |  [<span data-ttu-id="c90e2-129">принтсеттингс</span><span class="sxs-lookup"><span data-stu-id="c90e2-129">printSettings</span></span>](printsettings.md) | <span data-ttu-id="c90e2-130">Обновляет параметры на уровне клиента для универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="c90e2-130">Updates tenant-wide settings for the Universal Print service.</span></span> |
| [<span data-ttu-id="c90e2-131">Перечисление taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="c90e2-131">List taskDefinitions</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="c90e2-132">Коллекция [принттаскдефинитион](printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c90e2-132">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="c90e2-133">Получение общего для клиента списка Принттаскдефинитионс, созданного в универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="c90e2-133">Get a tenant-wide list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="c90e2-134">Создание taskDefinition</span><span class="sxs-lookup"><span data-stu-id="c90e2-134">Create taskDefinition</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="c90e2-135">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="c90e2-135">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="c90e2-136">Создание нового Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="c90e2-136">Create a new printTaskDefinition.</span></span> |
| [<span data-ttu-id="c90e2-137">Обновление taskDefinition</span><span class="sxs-lookup"><span data-stu-id="c90e2-137">Update taskDefinition</span></span>](../api/print-update-taskdefinition.md) | [<span data-ttu-id="c90e2-138">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="c90e2-138">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="c90e2-139">Обновление Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="c90e2-139">Update a printTaskDefinition.</span></span> |
| [<span data-ttu-id="c90e2-140">Удаление taskDefinition</span><span class="sxs-lookup"><span data-stu-id="c90e2-140">Delete taskDefinition</span></span>](../api/print-delete-taskdefinition.md) | <span data-ttu-id="c90e2-141">Нет</span><span class="sxs-lookup"><span data-stu-id="c90e2-141">None</span></span> | <span data-ttu-id="c90e2-142">Удаление объекта Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="c90e2-142">Delete a printTaskDefinition.</span></span> |

## <a name="properties"></a><span data-ttu-id="c90e2-143">Свойства</span><span class="sxs-lookup"><span data-stu-id="c90e2-143">Properties</span></span>
| <span data-ttu-id="c90e2-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="c90e2-144">Property</span></span>     | <span data-ttu-id="c90e2-145">Тип</span><span class="sxs-lookup"><span data-stu-id="c90e2-145">Type</span></span>        | <span data-ttu-id="c90e2-146">Описание</span><span class="sxs-lookup"><span data-stu-id="c90e2-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c90e2-147">параметры</span><span class="sxs-lookup"><span data-stu-id="c90e2-147">settings</span></span>|[<span data-ttu-id="c90e2-148">принтсеттингс</span><span class="sxs-lookup"><span data-stu-id="c90e2-148">printSettings</span></span>](printsettings.md)|<span data-ttu-id="c90e2-149">Параметры на уровне клиента для универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="c90e2-149">Tenant-wide settings for the Universal Print service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c90e2-150">Связи</span><span class="sxs-lookup"><span data-stu-id="c90e2-150">Relationships</span></span>
| <span data-ttu-id="c90e2-151">Связь</span><span class="sxs-lookup"><span data-stu-id="c90e2-151">Relationship</span></span> | <span data-ttu-id="c90e2-152">Тип</span><span class="sxs-lookup"><span data-stu-id="c90e2-152">Type</span></span>        | <span data-ttu-id="c90e2-153">Описание</span><span class="sxs-lookup"><span data-stu-id="c90e2-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c90e2-154">служб</span><span class="sxs-lookup"><span data-stu-id="c90e2-154">services</span></span>|<span data-ttu-id="c90e2-155">Коллекция [принтсервице](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="c90e2-155">[printService](printservice.md) collection</span></span>|<span data-ttu-id="c90e2-156">Список доступных конечных точек универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="c90e2-156">The list of available Universal Print service endpoints.</span></span>|
|<span data-ttu-id="c90e2-157">типографи</span><span class="sxs-lookup"><span data-stu-id="c90e2-157">printers</span></span>|<span data-ttu-id="c90e2-158">Коллекция [принтеров](printer.md)</span><span class="sxs-lookup"><span data-stu-id="c90e2-158">[printer](printer.md) collection</span></span>|<span data-ttu-id="c90e2-159">Список принтеров, зарегистрированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c90e2-159">The list of printers registered in the tenant.</span></span>|
|<span data-ttu-id="c90e2-160">shares</span><span class="sxs-lookup"><span data-stu-id="c90e2-160">shares</span></span>|<span data-ttu-id="c90e2-161">Коллекция [принтершаре](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="c90e2-161">[printerShare](printershare.md) collection</span></span>|<span data-ttu-id="c90e2-162">Список общих принтеров, зарегистрированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c90e2-162">The list of printer shares registered in the tenant.</span></span>|
|<span data-ttu-id="c90e2-163">аудиовыход</span><span class="sxs-lookup"><span data-stu-id="c90e2-163">connectors</span></span>|<span data-ttu-id="c90e2-164">Коллекция [принтконнектор](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="c90e2-164">[printConnector](printconnector.md) collection</span></span>|<span data-ttu-id="c90e2-165">Список доступных соединителей печати.</span><span class="sxs-lookup"><span data-stu-id="c90e2-165">The list of available print connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c90e2-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c90e2-166">JSON representation</span></span>

<span data-ttu-id="c90e2-167">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c90e2-167">The following is a JSON representation of the resource.</span></span>

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
    "Error: Resource print has documented navigation properties, but we thought it was a complex type!",
    "Resource print has documented navigation properties, but we thought it was a complex type!"
}-->


