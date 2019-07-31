---
title: Тип ресурса Едукатионкаурсе
description: Представляет сведения о курсе для класса.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c160f9bd20f7dfccfa19dbf4d466dd967fde9c2c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972763"
---
# <a name="educationcourse-resource-type"></a><span data-ttu-id="fb4e8-103">Тип ресурса Едукатионкаурсе</span><span class="sxs-lookup"><span data-stu-id="fb4e8-103">educationCourse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb4e8-104">Представляет сведения о курсе для класса.</span><span class="sxs-lookup"><span data-stu-id="fb4e8-104">Represents the course information for a class.</span></span> <span data-ttu-id="fb4e8-105">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="fb4e8-105">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fb4e8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb4e8-106">Properties</span></span>

| <span data-ttu-id="fb4e8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb4e8-107">Property</span></span>     | <span data-ttu-id="fb4e8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fb4e8-108">Type</span></span>   | <span data-ttu-id="fb4e8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fb4e8-109">Description</span></span>                               |
| :----------- | :----- | :---------------------------------------- |
| <span data-ttu-id="fb4e8-110">Каурсенумбер</span><span class="sxs-lookup"><span data-stu-id="fb4e8-110">courseNumber</span></span> | <span data-ttu-id="fb4e8-111">String</span><span class="sxs-lookup"><span data-stu-id="fb4e8-111">String</span></span> | <span data-ttu-id="fb4e8-112">Уникальный идентификатор курса.</span><span class="sxs-lookup"><span data-stu-id="fb4e8-112">Unique identifier for the course.</span></span>         |
| <span data-ttu-id="fb4e8-113">description</span><span class="sxs-lookup"><span data-stu-id="fb4e8-113">description</span></span>  | <span data-ttu-id="fb4e8-114">Строка</span><span class="sxs-lookup"><span data-stu-id="fb4e8-114">String</span></span> | <span data-ttu-id="fb4e8-115">Описание курса.</span><span class="sxs-lookup"><span data-stu-id="fb4e8-115">Description of the course.</span></span>                |
| <span data-ttu-id="fb4e8-116">displayName</span><span class="sxs-lookup"><span data-stu-id="fb4e8-116">displayName</span></span>  | <span data-ttu-id="fb4e8-117">Строка</span><span class="sxs-lookup"><span data-stu-id="fb4e8-117">String</span></span> | <span data-ttu-id="fb4e8-118">Название курса.</span><span class="sxs-lookup"><span data-stu-id="fb4e8-118">Name of the course.</span></span>                       |
| <span data-ttu-id="fb4e8-119">externalId</span><span class="sxs-lookup"><span data-stu-id="fb4e8-119">externalId</span></span>   | <span data-ttu-id="fb4e8-120">String</span><span class="sxs-lookup"><span data-stu-id="fb4e8-120">String</span></span> | <span data-ttu-id="fb4e8-121">ИДЕНТИФИКАТОР курса из системы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="fb4e8-121">ID of the course from the syncing system.</span></span> |
| <span data-ttu-id="fb4e8-122">subject</span><span class="sxs-lookup"><span data-stu-id="fb4e8-122">subject</span></span>      | <span data-ttu-id="fb4e8-123">String</span><span class="sxs-lookup"><span data-stu-id="fb4e8-123">String</span></span> | <span data-ttu-id="fb4e8-124">Тема курса.</span><span class="sxs-lookup"><span data-stu-id="fb4e8-124">Subject of the course.</span></span>                    |

## <a name="json-representation"></a><span data-ttu-id="fb4e8-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb4e8-125">JSON representation</span></span>

<span data-ttu-id="fb4e8-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb4e8-126">The following is a JSON representation of the resource.</span></span>

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
