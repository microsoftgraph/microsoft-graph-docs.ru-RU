---
title: Тип ресурса Аверажекомпаративескоре
description: Содержит различные оценки на основе разных областей.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f128fd22562889a5a537f3815a4003aec9bfc8a9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030018"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="19d75-103">Тип ресурса Аверажекомпаративескоре</span><span class="sxs-lookup"><span data-stu-id="19d75-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="19d75-104">Содержит различные оценки на основе различных областей (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="19d75-104">Contains various different scores based on different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

## <a name="properties"></a><span data-ttu-id="19d75-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="19d75-105">Properties</span></span>

|<span data-ttu-id="19d75-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="19d75-106">Property</span></span> |<span data-ttu-id="19d75-107">Тип</span><span class="sxs-lookup"><span data-stu-id="19d75-107">Type</span></span> |<span data-ttu-id="19d75-108">Описание</span><span class="sxs-lookup"><span data-stu-id="19d75-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="19d75-109">бы</span><span class="sxs-lookup"><span data-stu-id="19d75-109">basis</span></span>|<span data-ttu-id="19d75-110">String</span><span class="sxs-lookup"><span data-stu-id="19d75-110">String</span></span>|<span data-ttu-id="19d75-111">Тип области.</span><span class="sxs-lookup"><span data-stu-id="19d75-111">Scope type.</span></span> <span data-ttu-id="19d75-112">Допустимые значения: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span><span class="sxs-lookup"><span data-stu-id="19d75-112">The possible values are: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span></span>|
|<span data-ttu-id="19d75-113">Аверажескоре</span><span class="sxs-lookup"><span data-stu-id="19d75-113">averageScore</span></span>|<span data-ttu-id="19d75-114">Двойное</span><span class="sxs-lookup"><span data-stu-id="19d75-114">Double</span></span>|<span data-ttu-id="19d75-115">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="19d75-115">Average score within specified basis.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="19d75-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19d75-116">JSON representation</span></span>

<span data-ttu-id="19d75-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19d75-117">The following is a JSON representation of the resource.</span></span>

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
