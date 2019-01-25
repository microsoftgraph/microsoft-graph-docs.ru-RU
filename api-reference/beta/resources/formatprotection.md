---
title: Тип ресурса FormatProtection
description: Представляет защиту формата объекта Range.
localization_priority: Normal
ms.openlocfilehash: 7bc27060567136386ef1f08e6fe46e95980788a9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509191"
---
# <a name="formatprotection-resource-type"></a><span data-ttu-id="87818-103">Тип ресурса FormatProtection</span><span class="sxs-lookup"><span data-stu-id="87818-103">FormatProtection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87818-104">Представляет защиту формата объекта Range.</span><span class="sxs-lookup"><span data-stu-id="87818-104">Represents the format protection of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="87818-105">Методы</span><span class="sxs-lookup"><span data-stu-id="87818-105">Methods</span></span>

| <span data-ttu-id="87818-106">Метод</span><span class="sxs-lookup"><span data-stu-id="87818-106">Method</span></span>           | <span data-ttu-id="87818-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="87818-107">Return Type</span></span>    |<span data-ttu-id="87818-108">Описание</span><span class="sxs-lookup"><span data-stu-id="87818-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87818-109">Получение объекта FormatProtection</span><span class="sxs-lookup"><span data-stu-id="87818-109">[Get FormatProtection](../api/formatprotection-get.md)</span></span> | [<span data-ttu-id="87818-110">formatProtection</span><span class="sxs-lookup"><span data-stu-id="87818-110">FormatProtection</span></span>](formatprotection.md) |<span data-ttu-id="87818-111">Чтение свойств и связей объекта formatProtection.</span><span class="sxs-lookup"><span data-stu-id="87818-111">Read properties and relationships of formatProtection object.</span></span>|
|[<span data-ttu-id="87818-112">Update</span><span class="sxs-lookup"><span data-stu-id="87818-112">Update</span></span>](../api/formatprotection-update.md) | <span data-ttu-id="87818-113">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="87818-113">[FormatProtection](formatprotection.md)</span></span>  |<span data-ttu-id="87818-114">Обновление объекта FormatProtection.</span><span class="sxs-lookup"><span data-stu-id="87818-114">Update FormatProtection object.</span></span> |

## <a name="properties"></a><span data-ttu-id="87818-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="87818-115">Properties</span></span>
| <span data-ttu-id="87818-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="87818-116">Property</span></span>     | <span data-ttu-id="87818-117">Тип</span><span class="sxs-lookup"><span data-stu-id="87818-117">Type</span></span>   |<span data-ttu-id="87818-118">Описание</span><span class="sxs-lookup"><span data-stu-id="87818-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87818-119">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="87818-119">formulaHidden</span></span>|<span data-ttu-id="87818-120">boolean</span><span class="sxs-lookup"><span data-stu-id="87818-120">boolean</span></span>|<span data-ttu-id="87818-p101">Указывает, скрывает ли Excel формулу для ячеек в диапазоне. Значение NULL указывает, что для всего диапазона не задан единый параметр скрытия формулы.</span><span class="sxs-lookup"><span data-stu-id="87818-p101">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="87818-123">locked</span><span class="sxs-lookup"><span data-stu-id="87818-123">locked</span></span>|<span data-ttu-id="87818-124">boolean</span><span class="sxs-lookup"><span data-stu-id="87818-124">boolean</span></span>|<span data-ttu-id="87818-p102">Указывает, блокирует ли Excel ячейки в объекте. Значение NULL указывает, что для всего диапазона не задан единый параметр блокировки.</span><span class="sxs-lookup"><span data-stu-id="87818-p102">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87818-127">Связи</span><span class="sxs-lookup"><span data-stu-id="87818-127">Relationships</span></span>
<span data-ttu-id="87818-128">Нет</span><span class="sxs-lookup"><span data-stu-id="87818-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="87818-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87818-129">JSON representation</span></span>

<span data-ttu-id="87818-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87818-130">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/formatprotection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
