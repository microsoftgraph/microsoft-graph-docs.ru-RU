---
title: Тип ресурса FormatProtection
description: Представляет защиту формата объекта Range.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e474a29e657d19e06aa35fbebffeee85d855acfa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531380"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="5a94b-103">Тип ресурса FormatProtection</span><span class="sxs-lookup"><span data-stu-id="5a94b-103">FormatProtection resource type</span></span>

<span data-ttu-id="5a94b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a94b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a94b-105">Представляет защиту формата объекта Range.</span><span class="sxs-lookup"><span data-stu-id="5a94b-105">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="5a94b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="5a94b-106">Methods</span></span>

| <span data-ttu-id="5a94b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="5a94b-107">Method</span></span>           | <span data-ttu-id="5a94b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5a94b-108">Return Type</span></span>    |<span data-ttu-id="5a94b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5a94b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5a94b-110">Получение объекта FormatProtection</span><span class="sxs-lookup"><span data-stu-id="5a94b-110">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="5a94b-111">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="5a94b-111">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="5a94b-112">Чтение свойств и связей объекта formatProtection.</span><span class="sxs-lookup"><span data-stu-id="5a94b-112">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="5a94b-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="5a94b-113">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="5a94b-114">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="5a94b-114">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="5a94b-115">Обновление объекта FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="5a94b-115">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5a94b-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a94b-116">Properties</span></span>
| <span data-ttu-id="5a94b-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a94b-117">Property</span></span>     | <span data-ttu-id="5a94b-118">Тип</span><span class="sxs-lookup"><span data-stu-id="5a94b-118">Type</span></span>   |<span data-ttu-id="5a94b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5a94b-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a94b-120">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="5a94b-120">formulaHidden</span></span>|<span data-ttu-id="5a94b-121">boolean</span><span class="sxs-lookup"><span data-stu-id="5a94b-121">boolean</span></span>|<span data-ttu-id="5a94b-p101">Указывает, скрывает ли Excel формулу для ячеек в диапазоне. Значение NULL указывает, что для всего диапазона не задан единый параметр скрытия формулы.</span><span class="sxs-lookup"><span data-stu-id="5a94b-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="5a94b-124">locked</span><span class="sxs-lookup"><span data-stu-id="5a94b-124">locked</span></span>|<span data-ttu-id="5a94b-125">boolean</span><span class="sxs-lookup"><span data-stu-id="5a94b-125">boolean</span></span>|<span data-ttu-id="5a94b-p102">Указывает, блокирует ли Excel ячейки в объекте. Значение NULL указывает, что для всего диапазона не задан единый параметр блокировки.</span><span class="sxs-lookup"><span data-stu-id="5a94b-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a94b-128">Связи</span><span class="sxs-lookup"><span data-stu-id="5a94b-128">Relationships</span></span>
<span data-ttu-id="5a94b-129">Нет</span><span class="sxs-lookup"><span data-stu-id="5a94b-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5a94b-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a94b-130">JSON representation</span></span>

<span data-ttu-id="5a94b-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a94b-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFormatProtection"
}-->

```json
{
  "formulaHidden": true,
  "locked": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
