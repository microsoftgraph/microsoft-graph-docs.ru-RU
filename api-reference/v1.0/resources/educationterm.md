---
title: Тип ресурса educationTerm
description: Срок. Представляет определенную часть учебного года. Используется в educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 41a878f58736f608cf9cc9f0c45867bf48669b1a
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231838"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="e3d32-105">Тип ресурса educationTerm</span><span class="sxs-lookup"><span data-stu-id="e3d32-105">educationTerm resource type</span></span>

<span data-ttu-id="e3d32-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3d32-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3d32-107">Срок.</span><span class="sxs-lookup"><span data-stu-id="e3d32-107">A term.</span></span> <span data-ttu-id="e3d32-108">Представляет определенную часть учебного года.</span><span class="sxs-lookup"><span data-stu-id="e3d32-108">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="e3d32-109">Используется в [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="e3d32-109">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e3d32-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3d32-110">Properties</span></span>

| <span data-ttu-id="e3d32-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3d32-111">Property</span></span>    | <span data-ttu-id="e3d32-112">Тип</span><span class="sxs-lookup"><span data-stu-id="e3d32-112">Type</span></span>   | <span data-ttu-id="e3d32-113">Описание</span><span class="sxs-lookup"><span data-stu-id="e3d32-113">Description</span></span>                       |
| :---------- | :----- | :-------------------------------- |
| <span data-ttu-id="e3d32-114">displayName</span><span class="sxs-lookup"><span data-stu-id="e3d32-114">displayName</span></span> | <span data-ttu-id="e3d32-115">Строка</span><span class="sxs-lookup"><span data-stu-id="e3d32-115">String</span></span> | <span data-ttu-id="e3d32-116">Отображаемое имя срока.</span><span class="sxs-lookup"><span data-stu-id="e3d32-116">Display name of the term.</span></span>         |
| <span data-ttu-id="e3d32-117">externalId</span><span class="sxs-lookup"><span data-stu-id="e3d32-117">externalId</span></span>  | <span data-ttu-id="e3d32-118">String</span><span class="sxs-lookup"><span data-stu-id="e3d32-118">String</span></span> | <span data-ttu-id="e3d32-119">Идентификатор срока в системе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="e3d32-119">ID of term in the syncing system.</span></span> |
| <span data-ttu-id="e3d32-120">startDate</span><span class="sxs-lookup"><span data-stu-id="e3d32-120">startDate</span></span>   | <span data-ttu-id="e3d32-121">Date</span><span class="sxs-lookup"><span data-stu-id="e3d32-121">Date</span></span>   | <span data-ttu-id="e3d32-122">Начало срока.</span><span class="sxs-lookup"><span data-stu-id="e3d32-122">Start of the term.</span></span>                |
| <span data-ttu-id="e3d32-123">endDate</span><span class="sxs-lookup"><span data-stu-id="e3d32-123">endDate</span></span>     | <span data-ttu-id="e3d32-124">Date</span><span class="sxs-lookup"><span data-stu-id="e3d32-124">Date</span></span>   | <span data-ttu-id="e3d32-125">Конец срока.</span><span class="sxs-lookup"><span data-stu-id="e3d32-125">End of the term.</span></span>                  |

## <a name="relationships"></a><span data-ttu-id="e3d32-126">Связи</span><span class="sxs-lookup"><span data-stu-id="e3d32-126">Relationships</span></span>

<span data-ttu-id="e3d32-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e3d32-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3d32-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e3d32-128">JSON representation</span></span>

<span data-ttu-id="e3d32-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3d32-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationTerm"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationTerm",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date",
  "displayName": "String"
}
```
