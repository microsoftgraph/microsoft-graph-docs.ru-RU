---
title: Тип ресурса Едукатионкаурсе
description: Представляет сведения о курсе для класса.
author: mlafleur
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: eac609f787621e30d4707d477296fc53af77dad0
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764779"
---
# <a name="educationcourse-resource-type"></a><span data-ttu-id="a3058-103">Тип ресурса Едукатионкаурсе</span><span class="sxs-lookup"><span data-stu-id="a3058-103">educationCourse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3058-104">Представляет сведения о курсе для класса.</span><span class="sxs-lookup"><span data-stu-id="a3058-104">Represents the course information for a class.</span></span> <span data-ttu-id="a3058-105">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="a3058-105">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a3058-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3058-106">Properties</span></span>

| <span data-ttu-id="a3058-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3058-107">Property</span></span>     | <span data-ttu-id="a3058-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a3058-108">Type</span></span>   | <span data-ttu-id="a3058-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a3058-109">Description</span></span>                               |
| :----------- | :----- | :---------------------------------------- |
| <span data-ttu-id="a3058-110">Каурсенумбер</span><span class="sxs-lookup"><span data-stu-id="a3058-110">courseNumber</span></span> | <span data-ttu-id="a3058-111">String</span><span class="sxs-lookup"><span data-stu-id="a3058-111">String</span></span> | <span data-ttu-id="a3058-112">Уникальный идентификатор курса.</span><span class="sxs-lookup"><span data-stu-id="a3058-112">Unique identifier for the course.</span></span>         |
| <span data-ttu-id="a3058-113">description</span><span class="sxs-lookup"><span data-stu-id="a3058-113">description</span></span>  | <span data-ttu-id="a3058-114">Строка</span><span class="sxs-lookup"><span data-stu-id="a3058-114">String</span></span> | <span data-ttu-id="a3058-115">Описание курса.</span><span class="sxs-lookup"><span data-stu-id="a3058-115">Description of the course.</span></span>                |
| <span data-ttu-id="a3058-116">displayName</span><span class="sxs-lookup"><span data-stu-id="a3058-116">displayName</span></span>  | <span data-ttu-id="a3058-117">Строка</span><span class="sxs-lookup"><span data-stu-id="a3058-117">String</span></span> | <span data-ttu-id="a3058-118">Название курса.</span><span class="sxs-lookup"><span data-stu-id="a3058-118">Name of the course.</span></span>                       |
| <span data-ttu-id="a3058-119">externalId</span><span class="sxs-lookup"><span data-stu-id="a3058-119">externalId</span></span>   | <span data-ttu-id="a3058-120">String</span><span class="sxs-lookup"><span data-stu-id="a3058-120">String</span></span> | <span data-ttu-id="a3058-121">ИДЕНТИФИКАТОР курса из системы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a3058-121">ID of the course from the syncing system.</span></span> |
| <span data-ttu-id="a3058-122">subject</span><span class="sxs-lookup"><span data-stu-id="a3058-122">subject</span></span>      | <span data-ttu-id="a3058-123">String</span><span class="sxs-lookup"><span data-stu-id="a3058-123">String</span></span> | <span data-ttu-id="a3058-124">Тема курса.</span><span class="sxs-lookup"><span data-stu-id="a3058-124">Subject of the course.</span></span>                    |

## <a name="json-representation"></a><span data-ttu-id="a3058-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3058-125">JSON representation</span></span>

<span data-ttu-id="a3058-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3058-126">The following is a JSON representation of the resource.</span></span>

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
