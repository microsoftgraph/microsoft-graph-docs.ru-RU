---
title: Тип ресурса FormatProtection
description: Представляет защиту формата объекта Range.
localization_priority: Normal
ms.openlocfilehash: e4c32c8be8f6ef3aeaaf763ee88998bcbe235503
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542055"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="e1a44-103">Тип ресурса FormatProtection</span><span class="sxs-lookup"><span data-stu-id="e1a44-103">FormatProtection resource type</span></span>

<span data-ttu-id="e1a44-104">Представляет защиту формата объекта Range.</span><span class="sxs-lookup"><span data-stu-id="e1a44-104">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="e1a44-105">Методы</span><span class="sxs-lookup"><span data-stu-id="e1a44-105">Methods</span></span>

| <span data-ttu-id="e1a44-106">Метод</span><span class="sxs-lookup"><span data-stu-id="e1a44-106">Method</span></span>           | <span data-ttu-id="e1a44-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e1a44-107">Return Type</span></span>    |<span data-ttu-id="e1a44-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e1a44-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e1a44-109">Получение объекта FormatProtection</span><span class="sxs-lookup"><span data-stu-id="e1a44-109">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="e1a44-110">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="e1a44-110">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="e1a44-111">Чтение свойств и связей объекта formatProtection.</span><span class="sxs-lookup"><span data-stu-id="e1a44-111">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="e1a44-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="e1a44-112">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="e1a44-113">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="e1a44-113">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="e1a44-114">Обновление объекта FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="e1a44-114">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e1a44-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1a44-115">Properties</span></span>
| <span data-ttu-id="e1a44-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1a44-116">Property</span></span>     | <span data-ttu-id="e1a44-117">Тип</span><span class="sxs-lookup"><span data-stu-id="e1a44-117">Type</span></span>   |<span data-ttu-id="e1a44-118">Описание</span><span class="sxs-lookup"><span data-stu-id="e1a44-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1a44-119">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="e1a44-119">formulaHidden</span></span>|<span data-ttu-id="e1a44-120">логический</span><span class="sxs-lookup"><span data-stu-id="e1a44-120">boolean</span></span>|<span data-ttu-id="e1a44-p101">Указывает, скрывает ли Excel формулу для ячеек в диапазоне. Значение NULL указывает, что для всего диапазона не задан единый параметр скрытия формулы.</span><span class="sxs-lookup"><span data-stu-id="e1a44-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="e1a44-123">locked</span><span class="sxs-lookup"><span data-stu-id="e1a44-123">locked</span></span>|<span data-ttu-id="e1a44-124">boolean</span><span class="sxs-lookup"><span data-stu-id="e1a44-124">boolean</span></span>|<span data-ttu-id="e1a44-p102">Указывает, блокирует ли Excel ячейки в объекте. Значение NULL указывает, что для всего диапазона не задан единый параметр блокировки.</span><span class="sxs-lookup"><span data-stu-id="e1a44-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1a44-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="e1a44-127">Relationships</span></span>
<span data-ttu-id="e1a44-128">Нет</span><span class="sxs-lookup"><span data-stu-id="e1a44-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e1a44-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e1a44-129">JSON representation</span></span>

<span data-ttu-id="e1a44-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1a44-130">Here is a JSON representation of the resource.</span></span>

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
