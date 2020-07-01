---
title: Тип ресурса Print
description: С помощью универсальной подписки на печать функция печати позволяет управлять принтерами и обнаруживать Принтсервицеендпоинтс, которые можно использовать для управления принтерами и заданиями печати в универсальной печати.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 551fa42736d6fa275a8f998274a6fccf55ac00b7
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006977"
---
# <a name="print-resource-type"></a><span data-ttu-id="2764e-103">Тип ресурса Print</span><span class="sxs-lookup"><span data-stu-id="2764e-103">print resource type</span></span>

<span data-ttu-id="2764e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2764e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2764e-105">С помощью универсальной подписки на печать функция печати позволяет управлять принтерами и обнаруживать [принтсервицеендпоинтс](printserviceendpoint.md) , которые можно использовать для управления принтерами и заданиями печати в универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="2764e-105">When accompanied by a Universal Print subscription, the Print feature enables management of printers and discovery of [printServiceEndpoints](printserviceendpoint.md) that can be used to manage printers and print jobs within Universal Print.</span></span>

## <a name="methods"></a><span data-ttu-id="2764e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="2764e-106">Methods</span></span>
| <span data-ttu-id="2764e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="2764e-107">Method</span></span>       | <span data-ttu-id="2764e-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2764e-108">Return Type</span></span> | <span data-ttu-id="2764e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2764e-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2764e-110">Список соединителей</span><span class="sxs-lookup"><span data-stu-id="2764e-110">List connectors</span></span>](../api/print-list-connectors.md) | <span data-ttu-id="2764e-111">Коллекция [принтконнектор](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="2764e-111">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="2764e-112">Получение списка соединителей печати.</span><span class="sxs-lookup"><span data-stu-id="2764e-112">Get a list of print connectors.</span></span> |
| [<span data-ttu-id="2764e-113">Список принтеров</span><span class="sxs-lookup"><span data-stu-id="2764e-113">List printers</span></span>](../api/print-list-printers.md) | <span data-ttu-id="2764e-114">Коллекция [принтеров](printer.md)</span><span class="sxs-lookup"><span data-stu-id="2764e-114">[printer](printer.md) collection</span></span> | <span data-ttu-id="2764e-115">Получение списка принтеров.</span><span class="sxs-lookup"><span data-stu-id="2764e-115">Get a list of printers.</span></span> |
| [<span data-ttu-id="2764e-116">Список общих папок</span><span class="sxs-lookup"><span data-stu-id="2764e-116">List shares</span></span>](../api/print-list-shares.md) | <span data-ttu-id="2764e-117">Коллекция [принтершаре](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="2764e-117">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="2764e-118">Получение списка общих принтеров.</span><span class="sxs-lookup"><span data-stu-id="2764e-118">Get a list of printer shares.</span></span> |
| [<span data-ttu-id="2764e-119">Список служб</span><span class="sxs-lookup"><span data-stu-id="2764e-119">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="2764e-120">Коллекция [принтсервице](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="2764e-120">[printService](printservice.md) collection</span></span> | <span data-ttu-id="2764e-121">Получение списка служб.</span><span class="sxs-lookup"><span data-stu-id="2764e-121">Get a list of services.</span></span> |
| [<span data-ttu-id="2764e-122">Создание Принтершаре</span><span class="sxs-lookup"><span data-stu-id="2764e-122">Create printerShare</span></span>](../api/print-post-shares.md) | [<span data-ttu-id="2764e-123">принтершаре</span><span class="sxs-lookup"><span data-stu-id="2764e-123">printerShare</span></span>](printershare.md) | <span data-ttu-id="2764e-124">Создайте новый общий ресурс для принтера, отправив его в коллекцию **shares** .</span><span class="sxs-lookup"><span data-stu-id="2764e-124">Create a new printer share by posting to the **shares** collection.</span></span> |
| [<span data-ttu-id="2764e-125">Создание принтера</span><span class="sxs-lookup"><span data-stu-id="2764e-125">Create printer</span></span>](../api/printer-create.md) | [<span data-ttu-id="2764e-126">принтеркреатеоператион</span><span class="sxs-lookup"><span data-stu-id="2764e-126">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="2764e-127">Создание (регистрация) нового принтера с универсальной печатью.</span><span class="sxs-lookup"><span data-stu-id="2764e-127">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="2764e-128">Обновление параметров</span><span class="sxs-lookup"><span data-stu-id="2764e-128">Update settings</span></span>](../api/print-update-settings.md) |  [<span data-ttu-id="2764e-129">принтсеттингс</span><span class="sxs-lookup"><span data-stu-id="2764e-129">printSettings</span></span>](printsettings.md) | <span data-ttu-id="2764e-130">Обновляет параметры на уровне клиента для универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="2764e-130">Updates tenant-wide settings for the Universal Print service.</span></span> |

## <a name="properties"></a><span data-ttu-id="2764e-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="2764e-131">Properties</span></span>
| <span data-ttu-id="2764e-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="2764e-132">Property</span></span>     | <span data-ttu-id="2764e-133">Тип</span><span class="sxs-lookup"><span data-stu-id="2764e-133">Type</span></span>        | <span data-ttu-id="2764e-134">Описание</span><span class="sxs-lookup"><span data-stu-id="2764e-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2764e-135">settings</span><span class="sxs-lookup"><span data-stu-id="2764e-135">settings</span></span>|[<span data-ttu-id="2764e-136">принтсеттингс</span><span class="sxs-lookup"><span data-stu-id="2764e-136">printSettings</span></span>](printsettings.md)|<span data-ttu-id="2764e-137">Параметры на уровне клиента для универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="2764e-137">Tenant-wide settings for the Universal Print service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2764e-138">Связи</span><span class="sxs-lookup"><span data-stu-id="2764e-138">Relationships</span></span>
| <span data-ttu-id="2764e-139">Связь</span><span class="sxs-lookup"><span data-stu-id="2764e-139">Relationship</span></span> | <span data-ttu-id="2764e-140">Тип</span><span class="sxs-lookup"><span data-stu-id="2764e-140">Type</span></span>        | <span data-ttu-id="2764e-141">Описание</span><span class="sxs-lookup"><span data-stu-id="2764e-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2764e-142">служб</span><span class="sxs-lookup"><span data-stu-id="2764e-142">services</span></span>|<span data-ttu-id="2764e-143">Коллекция [принтсервице](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="2764e-143">[printService](printservice.md) collection</span></span>|<span data-ttu-id="2764e-144">Список доступных конечных точек универсальной службы печати.</span><span class="sxs-lookup"><span data-stu-id="2764e-144">The list of available Universal Print service endpoints.</span></span>|
|<span data-ttu-id="2764e-145">типографи</span><span class="sxs-lookup"><span data-stu-id="2764e-145">printers</span></span>|<span data-ttu-id="2764e-146">Коллекция [принтеров](printer.md)</span><span class="sxs-lookup"><span data-stu-id="2764e-146">[printer](printer.md) collection</span></span>|<span data-ttu-id="2764e-147">Список принтеров, зарегистрированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2764e-147">The list of printers registered in the tenant.</span></span>|
|<span data-ttu-id="2764e-148">shares</span><span class="sxs-lookup"><span data-stu-id="2764e-148">shares</span></span>|<span data-ttu-id="2764e-149">Коллекция [принтершаре](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="2764e-149">[printerShare](printershare.md) collection</span></span>|<span data-ttu-id="2764e-150">Список общих принтеров, зарегистрированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2764e-150">The list of printer shares registered in the tenant.</span></span>|
|<span data-ttu-id="2764e-151">аудиовыход</span><span class="sxs-lookup"><span data-stu-id="2764e-151">connectors</span></span>|<span data-ttu-id="2764e-152">Коллекция [принтконнектор](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="2764e-152">[printConnector](printconnector.md) collection</span></span>|<span data-ttu-id="2764e-153">Список доступных соединителей печати.</span><span class="sxs-lookup"><span data-stu-id="2764e-153">The list of available print connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2764e-154">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2764e-154">JSON representation</span></span>

<span data-ttu-id="2764e-155">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2764e-155">The following is a JSON representation of the resource.</span></span>

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
