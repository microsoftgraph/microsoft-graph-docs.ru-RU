---
title: Тип ресурса Едукатионкаурсе
description: Представляет сведения о курсе для класса.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9ba29e98150db6ffa9938585540d9b77f8a755cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502272"
---
# <a name="educationcourse-resource-type"></a><span data-ttu-id="02043-103">Тип ресурса Едукатионкаурсе</span><span class="sxs-lookup"><span data-stu-id="02043-103">educationCourse resource type</span></span>

<span data-ttu-id="02043-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02043-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02043-105">Представляет сведения о курсе для класса.</span><span class="sxs-lookup"><span data-stu-id="02043-105">Represents the course information for a class.</span></span> <span data-ttu-id="02043-106">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="02043-106">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="02043-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="02043-107">Properties</span></span>

| <span data-ttu-id="02043-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="02043-108">Property</span></span>     | <span data-ttu-id="02043-109">Тип</span><span class="sxs-lookup"><span data-stu-id="02043-109">Type</span></span>   | <span data-ttu-id="02043-110">Описание</span><span class="sxs-lookup"><span data-stu-id="02043-110">Description</span></span>                               |
| :----------- | :----- | :---------------------------------------- |
| <span data-ttu-id="02043-111">каурсенумбер</span><span class="sxs-lookup"><span data-stu-id="02043-111">courseNumber</span></span> | <span data-ttu-id="02043-112">String</span><span class="sxs-lookup"><span data-stu-id="02043-112">String</span></span> | <span data-ttu-id="02043-113">Уникальный идентификатор курса.</span><span class="sxs-lookup"><span data-stu-id="02043-113">Unique identifier for the course.</span></span>         |
| <span data-ttu-id="02043-114">description</span><span class="sxs-lookup"><span data-stu-id="02043-114">description</span></span>  | <span data-ttu-id="02043-115">Строка</span><span class="sxs-lookup"><span data-stu-id="02043-115">String</span></span> | <span data-ttu-id="02043-116">Описание курса.</span><span class="sxs-lookup"><span data-stu-id="02043-116">Description of the course.</span></span>                |
| <span data-ttu-id="02043-117">displayName</span><span class="sxs-lookup"><span data-stu-id="02043-117">displayName</span></span>  | <span data-ttu-id="02043-118">Строка</span><span class="sxs-lookup"><span data-stu-id="02043-118">String</span></span> | <span data-ttu-id="02043-119">Название курса.</span><span class="sxs-lookup"><span data-stu-id="02043-119">Name of the course.</span></span>                       |
| <span data-ttu-id="02043-120">externalId</span><span class="sxs-lookup"><span data-stu-id="02043-120">externalId</span></span>   | <span data-ttu-id="02043-121">String</span><span class="sxs-lookup"><span data-stu-id="02043-121">String</span></span> | <span data-ttu-id="02043-122">ИДЕНТИФИКАТОР курса из системы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="02043-122">ID of the course from the syncing system.</span></span> |
| <span data-ttu-id="02043-123">subject</span><span class="sxs-lookup"><span data-stu-id="02043-123">subject</span></span>      | <span data-ttu-id="02043-124">String</span><span class="sxs-lookup"><span data-stu-id="02043-124">String</span></span> | <span data-ttu-id="02043-125">Тема курса.</span><span class="sxs-lookup"><span data-stu-id="02043-125">Subject of the course.</span></span>                    |

## <a name="json-representation"></a><span data-ttu-id="02043-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02043-126">JSON representation</span></span>

<span data-ttu-id="02043-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02043-127">The following is a JSON representation of the resource.</span></span>

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
