---
title: Тип ресурса FormatProtection
description: Представляет защиту формата объекта Range.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c574ceefd33131562a0df504fad26bb225056ce7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497820"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="a38af-103">Тип ресурса FormatProtection</span><span class="sxs-lookup"><span data-stu-id="a38af-103">FormatProtection resource type</span></span>

<span data-ttu-id="a38af-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a38af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a38af-105">Представляет защиту формата объекта Range.</span><span class="sxs-lookup"><span data-stu-id="a38af-105">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="a38af-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a38af-106">Methods</span></span>

| <span data-ttu-id="a38af-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a38af-107">Method</span></span>           | <span data-ttu-id="a38af-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a38af-108">Return Type</span></span>    |<span data-ttu-id="a38af-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a38af-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a38af-110">Получение объекта FormatProtection</span><span class="sxs-lookup"><span data-stu-id="a38af-110">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="a38af-111">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="a38af-111">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="a38af-112">Чтение свойств и связей объекта formatProtection.</span><span class="sxs-lookup"><span data-stu-id="a38af-112">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="a38af-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="a38af-113">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="a38af-114">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="a38af-114">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="a38af-115">Обновление объекта FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="a38af-115">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a38af-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="a38af-116">Properties</span></span>
| <span data-ttu-id="a38af-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="a38af-117">Property</span></span>     | <span data-ttu-id="a38af-118">Тип</span><span class="sxs-lookup"><span data-stu-id="a38af-118">Type</span></span>   |<span data-ttu-id="a38af-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a38af-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a38af-120">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="a38af-120">formulaHidden</span></span>|<span data-ttu-id="a38af-121">boolean</span><span class="sxs-lookup"><span data-stu-id="a38af-121">boolean</span></span>|<span data-ttu-id="a38af-p101">Указывает, скрывает ли Excel формулу для ячеек в диапазоне. Значение NULL указывает, что для всего диапазона не задан единый параметр скрытия формулы.</span><span class="sxs-lookup"><span data-stu-id="a38af-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="a38af-124">locked</span><span class="sxs-lookup"><span data-stu-id="a38af-124">locked</span></span>|<span data-ttu-id="a38af-125">boolean</span><span class="sxs-lookup"><span data-stu-id="a38af-125">boolean</span></span>|<span data-ttu-id="a38af-p102">Указывает, блокирует ли Excel ячейки в объекте. Значение NULL указывает, что для всего диапазона не задан единый параметр блокировки.</span><span class="sxs-lookup"><span data-stu-id="a38af-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a38af-128">Связи</span><span class="sxs-lookup"><span data-stu-id="a38af-128">Relationships</span></span>
<span data-ttu-id="a38af-129">Нет</span><span class="sxs-lookup"><span data-stu-id="a38af-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a38af-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a38af-130">JSON representation</span></span>

<span data-ttu-id="a38af-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a38af-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.formatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
