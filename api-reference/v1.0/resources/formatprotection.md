---
title: Тип ресурса FormatProtection
description: Представляет защиту формата объекта Range.
ms.openlocfilehash: b3954763d7c611c0db90008ff7aa74f672c51a4d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025575"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="d64dd-103">Тип ресурса FormatProtection</span><span class="sxs-lookup"><span data-stu-id="d64dd-103">FormatProtection resource type</span></span>

<span data-ttu-id="d64dd-104">Представляет защиту формата объекта Range.</span><span class="sxs-lookup"><span data-stu-id="d64dd-104">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="d64dd-105">Методы</span><span class="sxs-lookup"><span data-stu-id="d64dd-105">Methods</span></span>

| <span data-ttu-id="d64dd-106">Метод</span><span class="sxs-lookup"><span data-stu-id="d64dd-106">Method</span></span>           | <span data-ttu-id="d64dd-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d64dd-107">Return Type</span></span>    |<span data-ttu-id="d64dd-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d64dd-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d64dd-109">Получение объекта FormatProtection</span><span class="sxs-lookup"><span data-stu-id="d64dd-109">Get FormatProtection</span></span>](../api/formatprotection-get.md) | [<span data-ttu-id="d64dd-110">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="d64dd-110">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="d64dd-111">Чтение свойств и связей объекта formatProtection.</span><span class="sxs-lookup"><span data-stu-id="d64dd-111">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="d64dd-112">Update</span><span class="sxs-lookup"><span data-stu-id="d64dd-112">Update</span></span>](../api/formatprotection-update.md) | [<span data-ttu-id="d64dd-113">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="d64dd-113">FormatProtection</span></span>](formatprotection.md)  |<span data-ttu-id="d64dd-114">Обновление объекта FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="d64dd-114">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d64dd-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="d64dd-115">Properties</span></span>
| <span data-ttu-id="d64dd-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="d64dd-116">Property</span></span>     | <span data-ttu-id="d64dd-117">Тип</span><span class="sxs-lookup"><span data-stu-id="d64dd-117">Type</span></span>   |<span data-ttu-id="d64dd-118">Описание</span><span class="sxs-lookup"><span data-stu-id="d64dd-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d64dd-119">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="d64dd-119">formulaHidden</span></span>|<span data-ttu-id="d64dd-120">boolean</span><span class="sxs-lookup"><span data-stu-id="d64dd-120">boolean</span></span>|<span data-ttu-id="d64dd-p101">Указывает, скрывает ли Excel формулу для ячеек в диапазоне. Значение NULL указывает, что для всего диапазона не задан единый параметр скрытия формулы.</span><span class="sxs-lookup"><span data-stu-id="d64dd-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="d64dd-123">locked</span><span class="sxs-lookup"><span data-stu-id="d64dd-123">locked</span></span>|<span data-ttu-id="d64dd-124">boolean</span><span class="sxs-lookup"><span data-stu-id="d64dd-124">boolean</span></span>|<span data-ttu-id="d64dd-p102">Указывает, блокирует ли Excel ячейки в объекте. Значение NULL указывает, что для всего диапазона не задан единый параметр блокировки.</span><span class="sxs-lookup"><span data-stu-id="d64dd-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d64dd-127">Связи</span><span class="sxs-lookup"><span data-stu-id="d64dd-127">Relationships</span></span>
<span data-ttu-id="d64dd-128">Нет</span><span class="sxs-lookup"><span data-stu-id="d64dd-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d64dd-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d64dd-129">JSON representation</span></span>

<span data-ttu-id="d64dd-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d64dd-130">Here is a JSON representation of the resource.</span></span>

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