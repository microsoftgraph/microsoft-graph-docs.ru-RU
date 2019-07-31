---
title: Тип ресурса FormatProtection
description: Представляет защиту формата объекта Range.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 036c09c1d5e4dfec043e6a1dc612aa728d6588f4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973544"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="b2a81-103">Тип ресурса FormatProtection</span><span class="sxs-lookup"><span data-stu-id="b2a81-103">FormatProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2a81-104">Представляет защиту формата объекта Range.</span><span class="sxs-lookup"><span data-stu-id="b2a81-104">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="b2a81-105">Методы</span><span class="sxs-lookup"><span data-stu-id="b2a81-105">Methods</span></span>

| <span data-ttu-id="b2a81-106">Метод</span><span class="sxs-lookup"><span data-stu-id="b2a81-106">Method</span></span>           | <span data-ttu-id="b2a81-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b2a81-107">Return Type</span></span>    |<span data-ttu-id="b2a81-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b2a81-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b2a81-109">Получение объекта FormatProtection</span><span class="sxs-lookup"><span data-stu-id="b2a81-109">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="b2a81-110">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="b2a81-110">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="b2a81-111">Чтение свойств и связей объекта formatProtection.</span><span class="sxs-lookup"><span data-stu-id="b2a81-111">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="b2a81-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="b2a81-112">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="b2a81-113">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="b2a81-113">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="b2a81-114">Обновление объекта FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="b2a81-114">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b2a81-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2a81-115">Properties</span></span>
| <span data-ttu-id="b2a81-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2a81-116">Property</span></span>     | <span data-ttu-id="b2a81-117">Тип</span><span class="sxs-lookup"><span data-stu-id="b2a81-117">Type</span></span>   |<span data-ttu-id="b2a81-118">Описание</span><span class="sxs-lookup"><span data-stu-id="b2a81-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2a81-119">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="b2a81-119">formulaHidden</span></span>|<span data-ttu-id="b2a81-120">boolean</span><span class="sxs-lookup"><span data-stu-id="b2a81-120">boolean</span></span>|<span data-ttu-id="b2a81-p101">Указывает, скрывает ли Excel формулу для ячеек в диапазоне. Значение NULL указывает, что для всего диапазона не задан единый параметр скрытия формулы.</span><span class="sxs-lookup"><span data-stu-id="b2a81-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="b2a81-123">locked</span><span class="sxs-lookup"><span data-stu-id="b2a81-123">locked</span></span>|<span data-ttu-id="b2a81-124">boolean</span><span class="sxs-lookup"><span data-stu-id="b2a81-124">boolean</span></span>|<span data-ttu-id="b2a81-p102">Указывает, блокирует ли Excel ячейки в объекте. Значение NULL указывает, что для всего диапазона не задан единый параметр блокировки.</span><span class="sxs-lookup"><span data-stu-id="b2a81-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2a81-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="b2a81-127">Relationships</span></span>
<span data-ttu-id="b2a81-128">Нет</span><span class="sxs-lookup"><span data-stu-id="b2a81-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b2a81-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2a81-129">JSON representation</span></span>

<span data-ttu-id="b2a81-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2a81-130">Here is a JSON representation of the resource.</span></span>

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
