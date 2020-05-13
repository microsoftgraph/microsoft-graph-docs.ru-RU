---
title: Тип ресурса Print
description: С помощью универсальной подписки на печать функция печати позволяет управлять принтерами и обнаруживать Принтсервицеендпоинтс, которые можно использовать для управления принтерами и заданиями печати в универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: b0af3f7443b77920804f5868fe9ecc3f8b4cec41
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217089"
---
# <a name="print-resource-type"></a><span data-ttu-id="775e4-103">Тип ресурса Print</span><span class="sxs-lookup"><span data-stu-id="775e4-103">print resource type</span></span>

<span data-ttu-id="775e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="775e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="775e4-105">С помощью универсальной подписки на печать функция печати позволяет управлять принтерами и обнаруживать [принтсервицеендпоинтс](printserviceendpoint.md) , которые можно использовать для управления принтерами и заданиями печати в универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="775e4-105">When accompanied by a Universal Print subscription, the Print feature enables management of printers and discovery of [printServiceEndpoints](printserviceendpoint.md) that can be used to manage printers and print jobs within Universal Print.</span></span>

## <a name="methods"></a><span data-ttu-id="775e4-106">Методы</span><span class="sxs-lookup"><span data-stu-id="775e4-106">Methods</span></span>
| <span data-ttu-id="775e4-107">Метод</span><span class="sxs-lookup"><span data-stu-id="775e4-107">Method</span></span>       | <span data-ttu-id="775e4-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="775e4-108">Return Type</span></span> | <span data-ttu-id="775e4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="775e4-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="775e4-110">Список соединителей</span><span class="sxs-lookup"><span data-stu-id="775e4-110">List connectors</span></span>](../api/print-list-connectors.md) | <span data-ttu-id="775e4-111">Коллекция [принтконнектор](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="775e4-111">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="775e4-112">Получение списка соединителей печати.</span><span class="sxs-lookup"><span data-stu-id="775e4-112">Get a list of print connectors.</span></span> |
| [<span data-ttu-id="775e4-113">Список принтеров</span><span class="sxs-lookup"><span data-stu-id="775e4-113">List printers</span></span>](../api/print-list-printers.md) | <span data-ttu-id="775e4-114">Коллекция [принтеров](printer.md)</span><span class="sxs-lookup"><span data-stu-id="775e4-114">[printer](printer.md) collection</span></span> | <span data-ttu-id="775e4-115">Получение списка принтеров.</span><span class="sxs-lookup"><span data-stu-id="775e4-115">Get a list of printers.</span></span> |
| [<span data-ttu-id="775e4-116">Список общих папок</span><span class="sxs-lookup"><span data-stu-id="775e4-116">List shares</span></span>](../api/print-list-shares.md) | <span data-ttu-id="775e4-117">Коллекция [принтершаре](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="775e4-117">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="775e4-118">Получение списка общих принтеров.</span><span class="sxs-lookup"><span data-stu-id="775e4-118">Get a list of printer shares.</span></span> |
| [<span data-ttu-id="775e4-119">Список служб</span><span class="sxs-lookup"><span data-stu-id="775e4-119">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="775e4-120">Коллекция [принтсервице](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="775e4-120">[printService](printservice.md) collection</span></span> | <span data-ttu-id="775e4-121">Получение списка служб.</span><span class="sxs-lookup"><span data-stu-id="775e4-121">Get a list of services.</span></span> |
| [<span data-ttu-id="775e4-122">Создание Принтершаре</span><span class="sxs-lookup"><span data-stu-id="775e4-122">Create printerShare</span></span>](../api/print-post-shares.md) | [<span data-ttu-id="775e4-123">принтершаре</span><span class="sxs-lookup"><span data-stu-id="775e4-123">printerShare</span></span>](printershare.md) | <span data-ttu-id="775e4-124">Создайте новый общий ресурс для принтера, отправив его в коллекцию **shares** .</span><span class="sxs-lookup"><span data-stu-id="775e4-124">Create a new printer share by posting to the **shares** collection.</span></span> |
| [<span data-ttu-id="775e4-125">Обновление параметров</span><span class="sxs-lookup"><span data-stu-id="775e4-125">Update settings</span></span>](../api/print-update-settings.md) |  [<span data-ttu-id="775e4-126">принтсеттингс</span><span class="sxs-lookup"><span data-stu-id="775e4-126">printSettings</span></span>](printsettings.md) | <span data-ttu-id="775e4-127">Обновляет параметры на уровне клиента для универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="775e4-127">Updates tenant-wide settings for the Universal Print service.</span></span> |

## <a name="properties"></a><span data-ttu-id="775e4-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="775e4-128">Properties</span></span>
| <span data-ttu-id="775e4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="775e4-129">Property</span></span>     | <span data-ttu-id="775e4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="775e4-130">Type</span></span>        | <span data-ttu-id="775e4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="775e4-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="775e4-132">settings</span><span class="sxs-lookup"><span data-stu-id="775e4-132">settings</span></span>|[<span data-ttu-id="775e4-133">принтсеттингс</span><span class="sxs-lookup"><span data-stu-id="775e4-133">printSettings</span></span>](printsettings.md)|<span data-ttu-id="775e4-134">Параметры на уровне клиента для универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="775e4-134">Tenant-wide settings for the Universal Print service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="775e4-135">Связи</span><span class="sxs-lookup"><span data-stu-id="775e4-135">Relationships</span></span>
| <span data-ttu-id="775e4-136">Связь</span><span class="sxs-lookup"><span data-stu-id="775e4-136">Relationship</span></span> | <span data-ttu-id="775e4-137">Тип</span><span class="sxs-lookup"><span data-stu-id="775e4-137">Type</span></span>        | <span data-ttu-id="775e4-138">Описание</span><span class="sxs-lookup"><span data-stu-id="775e4-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="775e4-139">служб</span><span class="sxs-lookup"><span data-stu-id="775e4-139">services</span></span>|<span data-ttu-id="775e4-140">Коллекция [принтсервице](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="775e4-140">[printService](printservice.md) collection</span></span>|<span data-ttu-id="775e4-141">Список доступных конечных точек универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="775e4-141">The list of available Universal Print service endpoints.</span></span>|
|<span data-ttu-id="775e4-142">типографи</span><span class="sxs-lookup"><span data-stu-id="775e4-142">printers</span></span>|<span data-ttu-id="775e4-143">Коллекция [принтеров](printer.md)</span><span class="sxs-lookup"><span data-stu-id="775e4-143">[printer](printer.md) collection</span></span>|<span data-ttu-id="775e4-144">Список принтеров, зарегистрированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="775e4-144">The list of printers registered in the tenant.</span></span>|
|<span data-ttu-id="775e4-145">shares</span><span class="sxs-lookup"><span data-stu-id="775e4-145">shares</span></span>|<span data-ttu-id="775e4-146">Коллекция [принтершаре](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="775e4-146">[printerShare](printershare.md) collection</span></span>|<span data-ttu-id="775e4-147">Список общих принтеров, зарегистрированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="775e4-147">The list of printer shares registered in the tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="775e4-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="775e4-148">JSON representation</span></span>

<span data-ttu-id="775e4-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="775e4-149">The following is a JSON representation of the resource.</span></span>

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