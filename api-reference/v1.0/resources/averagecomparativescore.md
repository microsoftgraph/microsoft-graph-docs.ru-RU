---
title: Тип ресурса Аверажекомпаративескоре
description: Содержит различные оценки на основе разных областей.
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 59faa1c3dcf3f7f2b70807a74878dab796ae4d54
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629329"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="24787-103">Тип ресурса Аверажекомпаративескоре</span><span class="sxs-lookup"><span data-stu-id="24787-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="24787-104">Содержит различные оценки на основе различных областей (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="24787-104">Contains various different scores based on different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

## <a name="properties"></a><span data-ttu-id="24787-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="24787-105">Properties</span></span>

|<span data-ttu-id="24787-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="24787-106">Property</span></span> |<span data-ttu-id="24787-107">Тип</span><span class="sxs-lookup"><span data-stu-id="24787-107">Type</span></span> |<span data-ttu-id="24787-108">Описание</span><span class="sxs-lookup"><span data-stu-id="24787-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="24787-109">бы</span><span class="sxs-lookup"><span data-stu-id="24787-109">basis</span></span>|<span data-ttu-id="24787-110">String</span><span class="sxs-lookup"><span data-stu-id="24787-110">String</span></span>|<span data-ttu-id="24787-111">Тип области.</span><span class="sxs-lookup"><span data-stu-id="24787-111">Scope type.</span></span> <span data-ttu-id="24787-112">Допустимые значения: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span><span class="sxs-lookup"><span data-stu-id="24787-112">The possible values are: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span></span>|
|<span data-ttu-id="24787-113">Аверажескоре</span><span class="sxs-lookup"><span data-stu-id="24787-113">averageScore</span></span>|<span data-ttu-id="24787-114">Двойное</span><span class="sxs-lookup"><span data-stu-id="24787-114">Double</span></span>|<span data-ttu-id="24787-115">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="24787-115">Average score within specified basis.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24787-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="24787-116">JSON representation</span></span>

<span data-ttu-id="24787-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24787-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.averageComparativeScore"
}-->

```json
{
  "basis": "String",
  "averageScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
