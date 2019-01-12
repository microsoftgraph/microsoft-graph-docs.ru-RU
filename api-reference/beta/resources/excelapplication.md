---
title: Тип ресурса приложения
description: Представляет приложение Excel, которое управляет книгой.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 250141ff6c6da3a81a1b3492908bc2e04b5a0605
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921978"
---
# <a name="application-resource-type"></a><span data-ttu-id="44f92-103">Тип ресурса приложения</span><span class="sxs-lookup"><span data-stu-id="44f92-103">Application resource type</span></span>

> <span data-ttu-id="44f92-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="44f92-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44f92-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44f92-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44f92-106">Представляет приложение Excel, которое управляет книгой.</span><span class="sxs-lookup"><span data-stu-id="44f92-106">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="44f92-107">Методы</span><span class="sxs-lookup"><span data-stu-id="44f92-107">Methods</span></span>

| <span data-ttu-id="44f92-108">Метод</span><span class="sxs-lookup"><span data-stu-id="44f92-108">Method</span></span>           | <span data-ttu-id="44f92-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="44f92-109">Return Type</span></span>    |<span data-ttu-id="44f92-110">Описание</span><span class="sxs-lookup"><span data-stu-id="44f92-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="44f92-111">Получение приложения</span><span class="sxs-lookup"><span data-stu-id="44f92-111">Get Application</span></span>](../api/excelapplication-get.md) | [<span data-ttu-id="44f92-112">Application</span><span class="sxs-lookup"><span data-stu-id="44f92-112">Application</span></span>](application.md) |<span data-ttu-id="44f92-113">Чтение свойства и связи объекта приложения.</span><span class="sxs-lookup"><span data-stu-id="44f92-113">Read properties and relationships of application object.</span></span>|
|[<span data-ttu-id="44f92-114">Calculate</span><span class="sxs-lookup"><span data-stu-id="44f92-114">Calculate</span></span>](../api/excelapplication-calculate.md)|<span data-ttu-id="44f92-115">Нет</span><span class="sxs-lookup"><span data-stu-id="44f92-115">None</span></span>|<span data-ttu-id="44f92-116">Пересчитывает данные во всех открытых в текущий момент книгах Excel.</span><span class="sxs-lookup"><span data-stu-id="44f92-116">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="44f92-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="44f92-117">Properties</span></span>
| <span data-ttu-id="44f92-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="44f92-118">Property</span></span>     | <span data-ttu-id="44f92-119">Тип</span><span class="sxs-lookup"><span data-stu-id="44f92-119">Type</span></span>   |<span data-ttu-id="44f92-120">Описание</span><span class="sxs-lookup"><span data-stu-id="44f92-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44f92-121">calculationMode</span><span class="sxs-lookup"><span data-stu-id="44f92-121">calculationMode</span></span>|<span data-ttu-id="44f92-122">строка</span><span class="sxs-lookup"><span data-stu-id="44f92-122">string</span></span>|<span data-ttu-id="44f92-123">Возвращает режим вычисления, используемый в книге.</span><span class="sxs-lookup"><span data-stu-id="44f92-123">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="44f92-124">Возможные значения: `Automatic`, `AutomaticExceptTables`, `Manual`.</span><span class="sxs-lookup"><span data-stu-id="44f92-124">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span> <span data-ttu-id="44f92-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="44f92-125">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44f92-126">Связи</span><span class="sxs-lookup"><span data-stu-id="44f92-126">Relationships</span></span>
<span data-ttu-id="44f92-127">Нет</span><span class="sxs-lookup"><span data-stu-id="44f92-127">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="44f92-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44f92-128">JSON representation</span></span>

<span data-ttu-id="44f92-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44f92-129">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
