---
title: тип ресурса печати
description: В сопровождении подписки универсальной печати функция Print позволяет управлять принтерами и открывать печатные точки, которые можно использовать для управления принтерами и заданиями печати в Universal Print.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: db532fed1bcdeeec749d59c8297fc36d836aed78
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517956"
---
# <a name="print-resource-type"></a><span data-ttu-id="0d298-103">тип ресурса печати</span><span class="sxs-lookup"><span data-stu-id="0d298-103">print resource type</span></span>

<span data-ttu-id="0d298-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d298-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="0d298-105">В сопровождении подписки универсальной печати функция Print позволяет управлять принтерами и открывать печатные [точки,](printserviceendpoint.md) которые можно использовать для управления принтерами и заданиями печати в Universal Print.</span><span class="sxs-lookup"><span data-stu-id="0d298-105">When accompanied by a Universal Print subscription, the Print feature enables management of printers and discovery of [printServiceEndpoints](printserviceendpoint.md) that can be used to manage printers and print jobs within Universal Print.</span></span>

## <a name="methods"></a><span data-ttu-id="0d298-106">Методы</span><span class="sxs-lookup"><span data-stu-id="0d298-106">Methods</span></span>
|<span data-ttu-id="0d298-107">Метод</span><span class="sxs-lookup"><span data-stu-id="0d298-107">Method</span></span>|<span data-ttu-id="0d298-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="0d298-108">Return type</span></span>|<span data-ttu-id="0d298-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0d298-109">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="0d298-110">Перечисление соединителей</span><span class="sxs-lookup"><span data-stu-id="0d298-110">List connectors</span></span>](../api/print-list-connectors.md) | <span data-ttu-id="0d298-111">[коллекция printConnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="0d298-111">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="0d298-112">Получите список соединители печати.</span><span class="sxs-lookup"><span data-stu-id="0d298-112">Get a list of print connectors.</span></span> |
| [<span data-ttu-id="0d298-113">Перечисление принтеров</span><span class="sxs-lookup"><span data-stu-id="0d298-113">List printers</span></span>](../api/print-list-printers.md) | <span data-ttu-id="0d298-114">[коллекция принтеров](printer.md)</span><span class="sxs-lookup"><span data-stu-id="0d298-114">[printer](printer.md) collection</span></span> | <span data-ttu-id="0d298-115">Получите список принтеров.</span><span class="sxs-lookup"><span data-stu-id="0d298-115">Get a list of printers.</span></span> |
| [<span data-ttu-id="0d298-116">Перечисление общих ресурсов</span><span class="sxs-lookup"><span data-stu-id="0d298-116">List shares</span></span>](../api/print-list-shares.md) | <span data-ttu-id="0d298-117">[коллекция printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="0d298-117">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="0d298-118">Получите список акций принтера.</span><span class="sxs-lookup"><span data-stu-id="0d298-118">Get a list of printer shares.</span></span> |
| [<span data-ttu-id="0d298-119">Службы списка</span><span class="sxs-lookup"><span data-stu-id="0d298-119">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="0d298-120">[коллекция printService](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="0d298-120">[printService](printservice.md) collection</span></span> | <span data-ttu-id="0d298-121">Получите список служб.</span><span class="sxs-lookup"><span data-stu-id="0d298-121">Get a list of services.</span></span> |
| [<span data-ttu-id="0d298-122">Создание printerShare</span><span class="sxs-lookup"><span data-stu-id="0d298-122">Create printerShare</span></span>](../api/print-post-shares.md) | [<span data-ttu-id="0d298-123">printerShare</span><span class="sxs-lookup"><span data-stu-id="0d298-123">printerShare</span></span>](printershare.md) | <span data-ttu-id="0d298-124">Создайте новую долю принтера, разместив в **коллекции акций.**</span><span class="sxs-lookup"><span data-stu-id="0d298-124">Create a new printer share by posting to the **shares** collection.</span></span> |
| [<span data-ttu-id="0d298-125">Создание принтера</span><span class="sxs-lookup"><span data-stu-id="0d298-125">Create printer</span></span>](../api/printer-create.md) | [<span data-ttu-id="0d298-126">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="0d298-126">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="0d298-127">Создание (регистрация) нового принтера с универсальной печатью.</span><span class="sxs-lookup"><span data-stu-id="0d298-127">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="0d298-128">Обновление параметров</span><span class="sxs-lookup"><span data-stu-id="0d298-128">Update settings</span></span>](../api/print-update-settings.md) |  [<span data-ttu-id="0d298-129">printSettings</span><span class="sxs-lookup"><span data-stu-id="0d298-129">printSettings</span></span>](printsettings.md) | <span data-ttu-id="0d298-130">Обновляет параметры для службы универсальной печати для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d298-130">Updates tenant-wide settings for the Universal Print service.</span></span> |
| [<span data-ttu-id="0d298-131">Перечисление taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="0d298-131">List taskDefinitions</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="0d298-132">[printTaskDefinition collection](printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0d298-132">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="0d298-133">Получите список распечатокTaskDefinitions, созданных в универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="0d298-133">Get a tenant-wide list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="0d298-134">Создание taskDefinition</span><span class="sxs-lookup"><span data-stu-id="0d298-134">Create taskDefinition</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="0d298-135">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="0d298-135">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="0d298-136">Создайте новый шрифтTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="0d298-136">Create a new printTaskDefinition.</span></span> |

## <a name="properties"></a><span data-ttu-id="0d298-137">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d298-137">Properties</span></span>
|<span data-ttu-id="0d298-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d298-138">Property</span></span>|<span data-ttu-id="0d298-139">Тип</span><span class="sxs-lookup"><span data-stu-id="0d298-139">Type</span></span>|<span data-ttu-id="0d298-140">Описание</span><span class="sxs-lookup"><span data-stu-id="0d298-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d298-141">параметры</span><span class="sxs-lookup"><span data-stu-id="0d298-141">settings</span></span>|[<span data-ttu-id="0d298-142">printSettings</span><span class="sxs-lookup"><span data-stu-id="0d298-142">printSettings</span></span>](../resources/printsettings.md)|<span data-ttu-id="0d298-143">Параметры для службы универсальной печати для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d298-143">Tenant-wide settings for the Universal Print service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d298-144">Отношения</span><span class="sxs-lookup"><span data-stu-id="0d298-144">Relationships</span></span>
|<span data-ttu-id="0d298-145">Связь</span><span class="sxs-lookup"><span data-stu-id="0d298-145">Relationship</span></span>|<span data-ttu-id="0d298-146">Тип</span><span class="sxs-lookup"><span data-stu-id="0d298-146">Type</span></span>|<span data-ttu-id="0d298-147">Описание</span><span class="sxs-lookup"><span data-stu-id="0d298-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d298-148">службы</span><span class="sxs-lookup"><span data-stu-id="0d298-148">services</span></span>|<span data-ttu-id="0d298-149">[коллекция printService](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="0d298-149">[printService](printservice.md) collection</span></span>|<span data-ttu-id="0d298-150">Список доступных конечных точек службы универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="0d298-150">The list of available Universal Print service endpoints.</span></span>|
|<span data-ttu-id="0d298-151">принтеры</span><span class="sxs-lookup"><span data-stu-id="0d298-151">printers</span></span>|<span data-ttu-id="0d298-152">[коллекция принтеров](printer.md)</span><span class="sxs-lookup"><span data-stu-id="0d298-152">[printer](printer.md) collection</span></span>|<span data-ttu-id="0d298-153">Список принтеров, зарегистрированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="0d298-153">The list of printers registered in the tenant.</span></span>|
|<span data-ttu-id="0d298-154">shares</span><span class="sxs-lookup"><span data-stu-id="0d298-154">shares</span></span>|<span data-ttu-id="0d298-155">[коллекция printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="0d298-155">[printerShare](printershare.md) collection</span></span>|<span data-ttu-id="0d298-156">Список акций принтера, зарегистрированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="0d298-156">The list of printer shares registered in the tenant.</span></span>|
|<span data-ttu-id="0d298-157">соединители</span><span class="sxs-lookup"><span data-stu-id="0d298-157">connectors</span></span>|<span data-ttu-id="0d298-158">[коллекция printConnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="0d298-158">[printConnector](printconnector.md) collection</span></span>|<span data-ttu-id="0d298-159">Список доступных соединители печати.</span><span class="sxs-lookup"><span data-stu-id="0d298-159">The list of available print connectors.</span></span>|
|<span data-ttu-id="0d298-160">operations</span><span class="sxs-lookup"><span data-stu-id="0d298-160">operations</span></span>|<span data-ttu-id="0d298-161">[коллекция printOperation](../resources/printoperation.md)</span><span class="sxs-lookup"><span data-stu-id="0d298-161">[printOperation](../resources/printoperation.md) collection</span></span>|<span data-ttu-id="0d298-162">Список длительных операций печати.</span><span class="sxs-lookup"><span data-stu-id="0d298-162">The list of print long running operations.</span></span>|
|<span data-ttu-id="0d298-163">службы</span><span class="sxs-lookup"><span data-stu-id="0d298-163">services</span></span>|<span data-ttu-id="0d298-164">[коллекция printService](../resources/printservice.md)</span><span class="sxs-lookup"><span data-stu-id="0d298-164">[printService](../resources/printservice.md) collection</span></span>|<span data-ttu-id="0d298-165">Список экземпляров служб печати для различных компонентов инфраструктуры печати.</span><span class="sxs-lookup"><span data-stu-id="0d298-165">The list of print service instances for various components of the printing infrastructure.</span></span>|
|<span data-ttu-id="0d298-166">taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="0d298-166">taskDefinitions</span></span>|<span data-ttu-id="0d298-167">[printTaskDefinition collection](../resources/printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0d298-167">[printTaskDefinition](../resources/printtaskdefinition.md) collection</span></span>|<span data-ttu-id="0d298-168">Список абстрактного определения задачи, которая может быть вызвана при различных событиях, происходящих в универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="0d298-168">List of abstract definition for a task that can be triggered when various events occur within Universal Print.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d298-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d298-169">JSON representation</span></span>
<span data-ttu-id="0d298-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d298-170">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.print",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.print",
  "settings": {
    "@odata.type": "microsoft.graph.printSettings"
  }
}
```

