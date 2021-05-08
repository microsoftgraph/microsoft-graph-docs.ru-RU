---
title: тип ресурса educationCourse
description: Представляет сведения о курсе для класса.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 347eb92cd0b36789cc7ecce1dea72af6985ea330
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232249"
---
# <a name="educationcourse-resource-type"></a><span data-ttu-id="4ff4f-103">тип ресурса educationCourse</span><span class="sxs-lookup"><span data-stu-id="4ff4f-103">educationCourse resource type</span></span>

<span data-ttu-id="4ff4f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ff4f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ff4f-105">Представляет сведения о курсе для класса.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-105">Represents the course information for a class.</span></span> <span data-ttu-id="4ff4f-106">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="4ff4f-106">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4ff4f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ff4f-107">Properties</span></span>

| <span data-ttu-id="4ff4f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ff4f-108">Property</span></span>     | <span data-ttu-id="4ff4f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4ff4f-109">Type</span></span>   | <span data-ttu-id="4ff4f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4ff4f-110">Description</span></span>                               |
| :----------- | :----- | :---------------------------------------- |
| <span data-ttu-id="4ff4f-111">courseNumber</span><span class="sxs-lookup"><span data-stu-id="4ff4f-111">courseNumber</span></span> | <span data-ttu-id="4ff4f-112">Строка</span><span class="sxs-lookup"><span data-stu-id="4ff4f-112">String</span></span> | <span data-ttu-id="4ff4f-113">Уникальный идентификатор для курса.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-113">Unique identifier for the course.</span></span>         |
| <span data-ttu-id="4ff4f-114">description</span><span class="sxs-lookup"><span data-stu-id="4ff4f-114">description</span></span>  | <span data-ttu-id="4ff4f-115">Строка</span><span class="sxs-lookup"><span data-stu-id="4ff4f-115">String</span></span> | <span data-ttu-id="4ff4f-116">Описание курса.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-116">Description of the course.</span></span>                |
| <span data-ttu-id="4ff4f-117">displayName</span><span class="sxs-lookup"><span data-stu-id="4ff4f-117">displayName</span></span>  | <span data-ttu-id="4ff4f-118">Строка</span><span class="sxs-lookup"><span data-stu-id="4ff4f-118">String</span></span> | <span data-ttu-id="4ff4f-119">Имя курса.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-119">Name of the course.</span></span>                       |
| <span data-ttu-id="4ff4f-120">externalId</span><span class="sxs-lookup"><span data-stu-id="4ff4f-120">externalId</span></span>   | <span data-ttu-id="4ff4f-121">String</span><span class="sxs-lookup"><span data-stu-id="4ff4f-121">String</span></span> | <span data-ttu-id="4ff4f-122">ID курса из системы синхронизации.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-122">ID of the course from the syncing system.</span></span> |
| <span data-ttu-id="4ff4f-123">subject</span><span class="sxs-lookup"><span data-stu-id="4ff4f-123">subject</span></span>      | <span data-ttu-id="4ff4f-124">String</span><span class="sxs-lookup"><span data-stu-id="4ff4f-124">String</span></span> | <span data-ttu-id="4ff4f-125">Тема курса.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-125">Subject of the course.</span></span>                    |

## <a name="relationships"></a><span data-ttu-id="4ff4f-126">Связи</span><span class="sxs-lookup"><span data-stu-id="4ff4f-126">Relationships</span></span>

<span data-ttu-id="4ff4f-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ff4f-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4ff4f-128">JSON representation</span></span>

<span data-ttu-id="4ff4f-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationCourse"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationCourse",
  "subject": "String",
  "courseNumber": "String",
  "description": "String",
  "displayName": "String",
  "externalId": "String"
}
```
