---
title: Тип ресурса Едукатионкаурсе
description: Представляет сведения о курсе для класса.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 80128524160a5f01806d36f52531383d5ab469a5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095516"
---
# <a name="educationcourse-resource-type"></a><span data-ttu-id="5b40e-103">Тип ресурса Едукатионкаурсе</span><span class="sxs-lookup"><span data-stu-id="5b40e-103">educationCourse resource type</span></span>

<span data-ttu-id="5b40e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b40e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b40e-105">Представляет сведения о курсе для класса.</span><span class="sxs-lookup"><span data-stu-id="5b40e-105">Represents the course information for a class.</span></span> <span data-ttu-id="5b40e-106">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="5b40e-106">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5b40e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b40e-107">Properties</span></span>

| <span data-ttu-id="5b40e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b40e-108">Property</span></span>     | <span data-ttu-id="5b40e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5b40e-109">Type</span></span>   | <span data-ttu-id="5b40e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5b40e-110">Description</span></span>                               |
| :----------- | :----- | :---------------------------------------- |
| <span data-ttu-id="5b40e-111">каурсенумбер</span><span class="sxs-lookup"><span data-stu-id="5b40e-111">courseNumber</span></span> | <span data-ttu-id="5b40e-112">Строка</span><span class="sxs-lookup"><span data-stu-id="5b40e-112">String</span></span> | <span data-ttu-id="5b40e-113">Уникальный идентификатор курса.</span><span class="sxs-lookup"><span data-stu-id="5b40e-113">Unique identifier for the course.</span></span>         |
| <span data-ttu-id="5b40e-114">description</span><span class="sxs-lookup"><span data-stu-id="5b40e-114">description</span></span>  | <span data-ttu-id="5b40e-115">Строка</span><span class="sxs-lookup"><span data-stu-id="5b40e-115">String</span></span> | <span data-ttu-id="5b40e-116">Описание курса.</span><span class="sxs-lookup"><span data-stu-id="5b40e-116">Description of the course.</span></span>                |
| <span data-ttu-id="5b40e-117">displayName</span><span class="sxs-lookup"><span data-stu-id="5b40e-117">displayName</span></span>  | <span data-ttu-id="5b40e-118">Строка</span><span class="sxs-lookup"><span data-stu-id="5b40e-118">String</span></span> | <span data-ttu-id="5b40e-119">Название курса.</span><span class="sxs-lookup"><span data-stu-id="5b40e-119">Name of the course.</span></span>                       |
| <span data-ttu-id="5b40e-120">externalId</span><span class="sxs-lookup"><span data-stu-id="5b40e-120">externalId</span></span>   | <span data-ttu-id="5b40e-121">String</span><span class="sxs-lookup"><span data-stu-id="5b40e-121">String</span></span> | <span data-ttu-id="5b40e-122">ИДЕНТИФИКАТОР курса из системы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="5b40e-122">ID of the course from the syncing system.</span></span> |
| <span data-ttu-id="5b40e-123">subject</span><span class="sxs-lookup"><span data-stu-id="5b40e-123">subject</span></span>      | <span data-ttu-id="5b40e-124">String</span><span class="sxs-lookup"><span data-stu-id="5b40e-124">String</span></span> | <span data-ttu-id="5b40e-125">Тема курса.</span><span class="sxs-lookup"><span data-stu-id="5b40e-125">Subject of the course.</span></span>                    |

## <a name="json-representation"></a><span data-ttu-id="5b40e-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5b40e-126">JSON representation</span></span>

<span data-ttu-id="5b40e-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b40e-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCourse"
}-->

```json
{
  "courseNumber": "String",
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationCourse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


