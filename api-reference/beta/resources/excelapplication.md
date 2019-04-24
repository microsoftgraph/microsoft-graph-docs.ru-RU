---
title: Тип ресурса приложения
description: Представляет приложение Excel, которое управляет книгой.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 48ee13a67d97f9c5c1a96a6ef6e104c5629f4108
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506533"
---
# <a name="application-resource-type"></a><span data-ttu-id="73e93-103">Тип ресурса приложения</span><span class="sxs-lookup"><span data-stu-id="73e93-103">Application resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73e93-104">Представляет приложение Excel, которое управляет книгой.</span><span class="sxs-lookup"><span data-stu-id="73e93-104">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="73e93-105">Методы</span><span class="sxs-lookup"><span data-stu-id="73e93-105">Methods</span></span>

| <span data-ttu-id="73e93-106">Метод</span><span class="sxs-lookup"><span data-stu-id="73e93-106">Method</span></span>           | <span data-ttu-id="73e93-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="73e93-107">Return Type</span></span>    |<span data-ttu-id="73e93-108">Описание</span><span class="sxs-lookup"><span data-stu-id="73e93-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="73e93-109">Получение приложения</span><span class="sxs-lookup"><span data-stu-id="73e93-109">Get Application</span></span>](../api/excelapplication-get.md) | [<span data-ttu-id="73e93-110">Приложение</span><span class="sxs-lookup"><span data-stu-id="73e93-110">Application</span></span>](application.md) |<span data-ttu-id="73e93-111">Считывание свойств и связей объекта application.</span><span class="sxs-lookup"><span data-stu-id="73e93-111">Read properties and relationships of application object.</span></span>|
|[<span data-ttu-id="73e93-112">Calculate</span><span class="sxs-lookup"><span data-stu-id="73e93-112">Calculate</span></span>](../api/excelapplication-calculate.md)|<span data-ttu-id="73e93-113">Отсутствует</span><span class="sxs-lookup"><span data-stu-id="73e93-113">None</span></span>|<span data-ttu-id="73e93-114">Пересчитывает данные во всех открытых в текущий момент книгах Excel.</span><span class="sxs-lookup"><span data-stu-id="73e93-114">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="73e93-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="73e93-115">Properties</span></span>
| <span data-ttu-id="73e93-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="73e93-116">Property</span></span>     | <span data-ttu-id="73e93-117">Тип</span><span class="sxs-lookup"><span data-stu-id="73e93-117">Type</span></span>   |<span data-ttu-id="73e93-118">Описание</span><span class="sxs-lookup"><span data-stu-id="73e93-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73e93-119">Калкулатионмоде</span><span class="sxs-lookup"><span data-stu-id="73e93-119">calculationMode</span></span>|<span data-ttu-id="73e93-120">string</span><span class="sxs-lookup"><span data-stu-id="73e93-120">string</span></span>|<span data-ttu-id="73e93-121">Возвращает режим вычисления, который используется в книге.</span><span class="sxs-lookup"><span data-stu-id="73e93-121">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="73e93-122">Возможные значения: `Automatic`, `AutomaticExceptTables`, `Manual`.</span><span class="sxs-lookup"><span data-stu-id="73e93-122">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span> <span data-ttu-id="73e93-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="73e93-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73e93-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="73e93-124">Relationships</span></span>
<span data-ttu-id="73e93-125">Нет</span><span class="sxs-lookup"><span data-stu-id="73e93-125">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="73e93-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="73e93-126">JSON representation</span></span>

<span data-ttu-id="73e93-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73e93-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "calculationMode": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/excelapplication.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
