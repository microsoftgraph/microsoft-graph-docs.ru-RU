---
title: Тип ресурса FormatProtection
description: Представляет защиту формата объекта Range.
localization_priority: Normal
ms.openlocfilehash: 0b4add2e30a1e475adcb162903f771ce760f9285
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805623"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="809d5-103">Тип ресурса FormatProtection</span><span class="sxs-lookup"><span data-stu-id="809d5-103">FormatProtection resource type</span></span>

> <span data-ttu-id="809d5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="809d5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="809d5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="809d5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="809d5-106">Представляет защиту формата объекта Range.</span><span class="sxs-lookup"><span data-stu-id="809d5-106">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="809d5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="809d5-107">Methods</span></span>

| <span data-ttu-id="809d5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="809d5-108">Method</span></span>           | <span data-ttu-id="809d5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="809d5-109">Return Type</span></span>    |<span data-ttu-id="809d5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="809d5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="809d5-111">Получение объекта FormatProtection</span><span class="sxs-lookup"><span data-stu-id="809d5-111">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="809d5-112">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="809d5-112">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="809d5-113">Чтение свойств и связей объекта formatProtection.</span><span class="sxs-lookup"><span data-stu-id="809d5-113">Read properties and relationships of formatProtection object.</span></span>|
|<span data-ttu-id="809d5-114">[обновление](../api/formatprotection-update.md).</span><span class="sxs-lookup"><span data-stu-id="809d5-114">[Update](../api/formatprotection-update.md)</span></span> | [<span data-ttu-id="809d5-115">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="809d5-115">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="809d5-116">Обновление объекта FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="809d5-116">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="809d5-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="809d5-117">Properties</span></span>
| <span data-ttu-id="809d5-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="809d5-118">Property</span></span>     | <span data-ttu-id="809d5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="809d5-119">Type</span></span>   |<span data-ttu-id="809d5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="809d5-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="809d5-121">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="809d5-121">formulaHidden</span></span>|<span data-ttu-id="809d5-122">boolean</span><span class="sxs-lookup"><span data-stu-id="809d5-122">boolean</span></span>|<span data-ttu-id="809d5-p102">Указывает, скрывает ли Excel формулу для ячеек в диапазоне. Значение NULL указывает, что для всего диапазона не задан единый параметр скрытия формулы.</span><span class="sxs-lookup"><span data-stu-id="809d5-p102">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="809d5-125">locked</span><span class="sxs-lookup"><span data-stu-id="809d5-125">locked</span></span>|<span data-ttu-id="809d5-126">boolean</span><span class="sxs-lookup"><span data-stu-id="809d5-126">boolean</span></span>|<span data-ttu-id="809d5-p103">Указывает, блокирует ли Excel ячейки в объекте. Значение NULL указывает, что для всего диапазона не задан единый параметр блокировки.</span><span class="sxs-lookup"><span data-stu-id="809d5-p103">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="809d5-129">Связи</span><span class="sxs-lookup"><span data-stu-id="809d5-129">Relationships</span></span>
<span data-ttu-id="809d5-130">Нет</span><span class="sxs-lookup"><span data-stu-id="809d5-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="809d5-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="809d5-131">JSON representation</span></span>

<span data-ttu-id="809d5-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="809d5-132">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "FormatProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
