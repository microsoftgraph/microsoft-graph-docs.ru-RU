---
title: Тип ресурса Print
description: С помощью универсальной подписки на печать функция печати позволяет управлять принтерами и обнаруживать Принтсервицеендпоинтс, которые можно использовать для управления принтерами и заданиями печати в универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: b32ebb749b3b13ee1d468de69b0724fe281e6793
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091503"
---
# <a name="print-resource-type"></a><span data-ttu-id="ce684-103">Тип ресурса Print</span><span class="sxs-lookup"><span data-stu-id="ce684-103">print resource type</span></span>

<span data-ttu-id="ce684-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce684-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce684-105">С помощью универсальной подписки на печать функция печати позволяет управлять принтерами и обнаруживать [принтсервицеендпоинтс](printserviceendpoint.md) , которые можно использовать для управления принтерами и заданиями печати в универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="ce684-105">When accompanied by a Universal Print subscription, the Print feature enables management of printers and discovery of [printServiceEndpoints](printserviceendpoint.md) that can be used to manage printers and print jobs within Universal Print.</span></span>

## <a name="methods"></a><span data-ttu-id="ce684-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ce684-106">Methods</span></span>
| <span data-ttu-id="ce684-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ce684-107">Method</span></span>       | <span data-ttu-id="ce684-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ce684-108">Return Type</span></span> | <span data-ttu-id="ce684-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ce684-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ce684-110">Список соединителей</span><span class="sxs-lookup"><span data-stu-id="ce684-110">List connectors</span></span>](../api/print-list-connectors.md) | <span data-ttu-id="ce684-111">Коллекция [принтконнектор](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="ce684-111">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="ce684-112">Получение списка соединителей печати.</span><span class="sxs-lookup"><span data-stu-id="ce684-112">Get a list of print connectors.</span></span> |
| [<span data-ttu-id="ce684-113">Список принтеров</span><span class="sxs-lookup"><span data-stu-id="ce684-113">List printers</span></span>](../api/print-list-printers.md) | <span data-ttu-id="ce684-114">Коллекция [принтеров](printer.md)</span><span class="sxs-lookup"><span data-stu-id="ce684-114">[printer](printer.md) collection</span></span> | <span data-ttu-id="ce684-115">Получение списка принтеров.</span><span class="sxs-lookup"><span data-stu-id="ce684-115">Get a list of printers.</span></span> |
| [<span data-ttu-id="ce684-116">Список общих папок</span><span class="sxs-lookup"><span data-stu-id="ce684-116">List shares</span></span>](../api/print-list-shares.md) | <span data-ttu-id="ce684-117">Коллекция [принтершаре](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="ce684-117">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="ce684-118">Получение списка общих принтеров.</span><span class="sxs-lookup"><span data-stu-id="ce684-118">Get a list of printer shares.</span></span> |
| [<span data-ttu-id="ce684-119">Список служб</span><span class="sxs-lookup"><span data-stu-id="ce684-119">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="ce684-120">Коллекция [принтсервице](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="ce684-120">[printService](printservice.md) collection</span></span> | <span data-ttu-id="ce684-121">Получение списка служб.</span><span class="sxs-lookup"><span data-stu-id="ce684-121">Get a list of services.</span></span> |
| [<span data-ttu-id="ce684-122">Создание Принтершаре</span><span class="sxs-lookup"><span data-stu-id="ce684-122">Create printerShare</span></span>](../api/print-post-shares.md) | [<span data-ttu-id="ce684-123">принтершаре</span><span class="sxs-lookup"><span data-stu-id="ce684-123">printerShare</span></span>](printershare.md) | <span data-ttu-id="ce684-124">Создайте новый общий ресурс для принтера, отправив его в коллекцию **shares** .</span><span class="sxs-lookup"><span data-stu-id="ce684-124">Create a new printer share by posting to the **shares** collection.</span></span> |
| [<span data-ttu-id="ce684-125">Создание принтера</span><span class="sxs-lookup"><span data-stu-id="ce684-125">Create printer</span></span>](../api/printer-create.md) | [<span data-ttu-id="ce684-126">принтеркреатеоператион</span><span class="sxs-lookup"><span data-stu-id="ce684-126">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="ce684-127">Создание (регистрация) нового принтера с универсальной печатью.</span><span class="sxs-lookup"><span data-stu-id="ce684-127">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="ce684-128">Обновление параметров</span><span class="sxs-lookup"><span data-stu-id="ce684-128">Update settings</span></span>](../api/print-update-settings.md) |  [<span data-ttu-id="ce684-129">принтсеттингс</span><span class="sxs-lookup"><span data-stu-id="ce684-129">printSettings</span></span>](printsettings.md) | <span data-ttu-id="ce684-130">Обновляет параметры на уровне клиента для универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="ce684-130">Updates tenant-wide settings for the Universal Print service.</span></span> |
| [<span data-ttu-id="ce684-131">Список Таскдефинитионс</span><span class="sxs-lookup"><span data-stu-id="ce684-131">List taskDefinitions</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="ce684-132">Коллекция [принттаскдефинитион](printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ce684-132">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="ce684-133">Получение общего для клиента списка Принттаскдефинитионс, созданного в универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="ce684-133">Get a tenant-wide list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="ce684-134">Создание Таскдефинитион</span><span class="sxs-lookup"><span data-stu-id="ce684-134">Create taskDefinition</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="ce684-135">принттаскдефинитион</span><span class="sxs-lookup"><span data-stu-id="ce684-135">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="ce684-136">Создание нового Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="ce684-136">Create a new printTaskDefinition.</span></span> |
| [<span data-ttu-id="ce684-137">Обновление Таскдефинитион</span><span class="sxs-lookup"><span data-stu-id="ce684-137">Update taskDefinition</span></span>](../api/print-update-taskdefinition.md) | [<span data-ttu-id="ce684-138">принттаскдефинитион</span><span class="sxs-lookup"><span data-stu-id="ce684-138">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="ce684-139">Обновление Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="ce684-139">Update a printTaskDefinition.</span></span> |
| [<span data-ttu-id="ce684-140">Удаление Таскдефинитион</span><span class="sxs-lookup"><span data-stu-id="ce684-140">Delete taskDefinition</span></span>](../api/print-delete-taskdefinition.md) | <span data-ttu-id="ce684-141">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="ce684-141">None</span></span> | <span data-ttu-id="ce684-142">Удаление объекта Принттаскдефинитион.</span><span class="sxs-lookup"><span data-stu-id="ce684-142">Delete a printTaskDefinition.</span></span> |

## <a name="properties"></a><span data-ttu-id="ce684-143">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce684-143">Properties</span></span>
| <span data-ttu-id="ce684-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce684-144">Property</span></span>     | <span data-ttu-id="ce684-145">Тип</span><span class="sxs-lookup"><span data-stu-id="ce684-145">Type</span></span>        | <span data-ttu-id="ce684-146">Описание</span><span class="sxs-lookup"><span data-stu-id="ce684-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ce684-147">settings</span><span class="sxs-lookup"><span data-stu-id="ce684-147">settings</span></span>|[<span data-ttu-id="ce684-148">принтсеттингс</span><span class="sxs-lookup"><span data-stu-id="ce684-148">printSettings</span></span>](printsettings.md)|<span data-ttu-id="ce684-149">Параметры на уровне клиента для универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="ce684-149">Tenant-wide settings for the Universal Print service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce684-150">Связи</span><span class="sxs-lookup"><span data-stu-id="ce684-150">Relationships</span></span>
| <span data-ttu-id="ce684-151">Связь</span><span class="sxs-lookup"><span data-stu-id="ce684-151">Relationship</span></span> | <span data-ttu-id="ce684-152">Тип</span><span class="sxs-lookup"><span data-stu-id="ce684-152">Type</span></span>        | <span data-ttu-id="ce684-153">Описание</span><span class="sxs-lookup"><span data-stu-id="ce684-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ce684-154">служб</span><span class="sxs-lookup"><span data-stu-id="ce684-154">services</span></span>|<span data-ttu-id="ce684-155">Коллекция [принтсервице](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="ce684-155">[printService](printservice.md) collection</span></span>|<span data-ttu-id="ce684-156">Список доступных конечных точек универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="ce684-156">The list of available Universal Print service endpoints.</span></span>|
|<span data-ttu-id="ce684-157">типографи</span><span class="sxs-lookup"><span data-stu-id="ce684-157">printers</span></span>|<span data-ttu-id="ce684-158">Коллекция [принтеров](printer.md)</span><span class="sxs-lookup"><span data-stu-id="ce684-158">[printer](printer.md) collection</span></span>|<span data-ttu-id="ce684-159">Список принтеров, зарегистрированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="ce684-159">The list of printers registered in the tenant.</span></span>|
|<span data-ttu-id="ce684-160">shares</span><span class="sxs-lookup"><span data-stu-id="ce684-160">shares</span></span>|<span data-ttu-id="ce684-161">Коллекция [принтершаре](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="ce684-161">[printerShare](printershare.md) collection</span></span>|<span data-ttu-id="ce684-162">Список общих принтеров, зарегистрированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="ce684-162">The list of printer shares registered in the tenant.</span></span>|
|<span data-ttu-id="ce684-163">аудиовыход</span><span class="sxs-lookup"><span data-stu-id="ce684-163">connectors</span></span>|<span data-ttu-id="ce684-164">Коллекция [принтконнектор](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="ce684-164">[printConnector](printconnector.md) collection</span></span>|<span data-ttu-id="ce684-165">Список доступных соединителей печати.</span><span class="sxs-lookup"><span data-stu-id="ce684-165">The list of available print connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ce684-166">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ce684-166">JSON representation</span></span>

<span data-ttu-id="ce684-167">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce684-167">The following is a JSON representation of the resource.</span></span>

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
